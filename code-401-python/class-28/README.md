# Authentication & Production Server

## Reading:
#### What is JSON Web Token?
- JSON Web Token (JWT) is an open standard (RFC 7519) that defines a compact and self-contained way for securely transmitting information between parties as a JSON object. This information can be verified and trusted because it is digitally signed. JWTs can be signed using a secret (with the HMAC algorithm) or a public/private key pair using RSA or ECDSA.
#### When should you use JSON Web Tokens?
1. Authorization: This is the most common scenario for using JWT. Once the user is logged in, each subsequent request will include the JWT, allowing the user to access routes, services, and resources that are permitted with that token. Single Sign On is a feature that widely uses JWT nowadays, because of its small overhead and its ability to be easily used across different domains.
2. Information Exchange: JSON Web Tokens are a good way of securely transmitting information between parties. Because JWTs can be signed—for example, using public/private key pairs—you can be sure the senders are who they say they are. Additionally, as the signature is calculated using the header and the payload, you can also verify that the content hasn't been tampered with.

#### What is the JSON Web Token structure?
- In its compact form, JSON Web Tokens consist of three parts separated by dots (.), which are:

1. Header
- The header typically consists of two parts: the type of the token, which is JWT, and the signing algorithm being used, such as HMAC SHA256 or RSA.
2. Payload
- The second part of the token is the payload, which contains the claims. Claims are statements about an entity (typically, the user) and additional data. There are three types of claims: registered, public, and private claims.
3. Signature
- To create the signature part you have to take the encoded header, the encoded payload, a secret, the algorithm specified in the header, and sign that.

#### How JWT Works?
- The JWT is acquired by exchanging an username + password for an access token and an refresh token.
- The access token is usually short-lived (expires in 5 min or so, can be customized though).
- The refresh token lives a little bit longer (expires in 24 hours, also customizable). It is comparable to an authentication session. After it expires, you need a full login with username + password again.

#### Installation
`pip install djangorestframework_simplejwt`

#### A Production Stack
- A production setup usually consists of multiple components, each designed and built to be really good at one specific thing. They are fast, reliable and very focused.

- When a request arrives at your server, it should be passed to a dedicated web server. Nginx is an example for a good web server.

- This is an application, which is great at serving static files from disk (your css and js files for example) and handling multiple requests at once. If the request is not for a static file, but should be processed by your application, the webserver is configured to pass this request to the next component.