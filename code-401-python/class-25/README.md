# Django REST Framework & Docker

## Reading:
#### Docker
-  Docker which is a way to isolate and run entire applications. The entire development environment is isolated: programming language, software packages, databases, and more.
- Docker is really just Linux containers which are a type of virtualization.

#### Downsides of using Docker
- Size
- Speed

#### Containers vs Virtual Environments
- Virtual environments are used to isolate Python software packages locally. We can create an isolated box for individual projects so one can use Python 2.7 and Django 1.5 while another can use Python 3.5 and Django 2.1 on the same computer. Virtual environments are great.
- But…virtual environments can only isolate Python packages. They still rely on a global, system-level installation of Python albeit they can refer to the proper version. So when we use Python 2.7 in a project, we’re pointing to an installation of Python 2.7 on the computer itself, not actually within the virtual environment.

#### Django REST Framework
- Django REST framework is a powerful and flexible toolkit for building Web APIs.
- The Django REST Framework provides a full suite of features for developing RESTful APIs, including serialization, authentication, authorization, and throttling. It also makes it easy to manage the data that is stored in the database, allowing developers to quickly make changes to the data model and maintain a clean, consistent codebase.

#### Uses of Django REST Framework
- The Web browsable API is a huge usability win for your developers.
- Authentication policies including packages for OAuth1a and OAuth2.
- Serialization that supports both ORM and non-ORM data sources.
- Customizable all the way down - just use regular function-based views if you don't need the more powerful features.
- Extensive documentation, and great community support.
- Used and trusted by internationally recognised companies including Mozilla, Red Hat, Heroku, and Eventbrite.

#### Requirements of REST framework
- Python (3.6, 3.7, 3.8, 3.9, 3.10)
- Django (2.2, 3.0, 3.1, 3.2, 4.0, 4.1)