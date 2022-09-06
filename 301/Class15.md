# Authentication

## OAuth

1. What is OAuth?
- OAuth is an open-standard authorization protocol or framework that describes how unrelated servers and services can safely allow authenticated access to their assets without actually sharing the initial, related, single logon credential
2. Give an example of what using OAuth would look like.
- The simplest example of OAuth is when you go to log onto a website and it offers one or more opportunities to log on using another website’s/service’s logon. You then click on the button linked to the other website, the other website authenticates you, and the website you were originally connecting to logs you on itself afterward using permission gained from the second website.
3. How does OAuth work? What are the steps that it takes to authenticate the user?
- Let’s assume a user has already signed into one website or service (OAuth only works using HTTPS). The user then initiates a feature/transaction that needs to access another unrelated site or service. The following happens (greatly simplified):
- 
1. The first website connects to the second website on behalf of the user, using OAuth, providing the user’s verified identity.
2. The second site generates a one-time token and a one-time secret unique to the transaction and parties involved.
3. The first site gives this token and secret to the initiating user’s client software.
4. The client’s software presents the request token and secret to their authorization provider (which may or may not be the second site).
5. If not already authenticated to the authorization provider, the client may be asked to authenticate. After authentication, the client is asked to approve the authorization transaction to the second website.
6. The user approves (or their software silently approves) a particular transaction type at the first website.
7. The user is given an approved access token (notice it’s no longer a request token).
8. The user gives the approved access token to the first website.
9. The first website gives the access token to the second website as proof of authentication on behalf of the user.
10. The second website lets the first website access their site on behalf of the user.
11. The user sees a successfully completed transaction occurring.
12. OAuth is not the first authentication/authorization system to work this way on behalf of the end-user. In fact, many authentication systems, notably Kerberos, work similarly. What is special about OAuth is its ability to work across the web and its wide adoption. It succeeded with adoption rates where previous attempts failed (for various reasons).
-

4. What is OpenID?
- a means for logging into the then-popular LiveJournal blogging site but quickly spread to other sites.

## Authorization and Authentication flows
1. What is the difference between authorization and authentication?

| Authorization      | Authentication |
| ----------- | ----------- |
| Determines what users can and cannot access  | Determines whether users are who they claim to be  |
|Usually done after successful authentication | Usually done before authorization|
| Generally, transmits info through an Access Token  | Generally, transmits info through an ID Token |
| Generally governed by the OAuth 2.0 framework | Generally governed by the OpenID Connect (OIDC) protocol |


2. What is Authorization Code Flow?
- It emans that it exchanges the authorization code for a token.
3. What is Authorization Code Flow with Proof Key for Code Exchange (PKCE)?
- When public clients (e.g., native and single-page applications) request access tokens, some additional security concerns are posed that are not mitigated by the Authorization Code Flow alone. This is because:
4. What is Implicit Flow with Form Post?
- you obtain an ID token using authorization code flow performed by the app backend. This method is effective and robust, however, it requires your web app to obtain and manage a secret. You can avoid that burden if all you want to do is implement sign-in and you don’t need to obtain access tokens for invoking APIs.
5. What is Client Credentials Flow?
- they pass along their Client ID and Client Secret to authenticate themselves and get a token.
6. What is Device Authorization Flow?
- they pass along their Client ID to initiate the authorization process and get a token.
7. What is Resource Owner Password Flow?
-  requests that users provide credentials (username and password), typically using an interactive form. Because credentials are sent to the backend and can be stored for future use before being exchanged for an Access Token, it is imperative that the application is absolutely trusted with this information.

## Things I want to know more about
- I want to understand when and how to use each authorization methoed

### Sources: 
- https://www.csoonline.com/article/3216404/what-is-oauth-how-the-open-authorization-framework-works.html
- https://auth0.com/docs/get-started/authentication-and-authorization-flow
