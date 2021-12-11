# Django REST Framework & Docker

## Docker

![Docker Logo](https://www.docker.com/sites/default/files/d8/2019-07/vertical-logo-monochromatic.png)

**`Docker`** provides the ability to package and run an application in a loosely isolated environment called a container.

The isolation and security allow you to run many containers simultaneously on a given host.

Containers are lightweight and contain everything needed to run the application, so you do not need to rely on what is currently installed on the host.

Docker provides tooling and a platform to manage the lifecycle of your containers:

* Develop your application and its supporting components using containers.
* The container becomes the unit for distributing and testing your application.
* When you’re ready, deploy your application into your production environment, as a container or an orchestrated service. This works the same whether your production environment is a local data center, a cloud provider, or a hybrid of the two.

### What can I use Docker for ?

**`Docker`** streamlines the development lifecycle by allowing developers to work in standardized environments using local containers which provide your applications and services. Containers are great for continuous integration and continuous delivery (CI/CD) workflows.

### Install Docker

To install **`Docker`** first you need to download the desktop application on your pc.

Once it's done installing you can check the version using the following comand:

> docker --version

*`Docker Compose`* is a tool that is already installed with Mac and Windows downloads of **`Docker`**. However, if you are using Linux, you need to install it manually.

You can install it using the following command :

> sudo pip install docker-compose

To confirm that Docker is installed correctly you can run the following command :

> docker run hello-world

### Docker image and container

A **`Docker image`** is an immutable (unchangeable) file that contains the source code, libraries, dependencies, tools, and other files needed for an application to run.

A **`Docker container`** is a virtualized run-time environment where users can isolate applications from the underlying system. These containers are compact, portable units in which you can start up an application quickly and easily.

![Docker image and container](https://phoenixnap.com/kb/wp-content/uploads/2021/04/container-layers.png)

## Django REST framework and Web APIs

![Django APIs](https://www.django-rest-framework.org/img/logo.png)

Django REST framework is a powerful and flexible toolkit for building Web APIs.

Django REST Framework is added just like any other third-party app using the following command :

> poetry add djangorestframework

Then add it to the **`INSTALLED_APPS`** in the settings.py.

```python
INSTALLED_APPS = [
    'django.contrib.admin',
    'django.contrib.auth',
    'django.contrib.contenttypes',
    'django.contrib.sessions',
    'django.contrib.messages',
    'django.contrib.staticfiles',

    # 3rd party
    'rest_framework',

    # Local
    
]
```

### Why Django REST framework ?

* The Web browsable API is a huge usability win for your developers.
* Authentication policies including packages for OAuth1a and OAuth2.
* Serialization that supports both ORM and non-ORM data sources.
* Customizable all the way down - just use regular function-based views if you don't need the more powerful features.
* Extensive documentation, and great community support.
* Used and trusted by internationally recognised companies including Mozilla, Red Hat, Heroku, and Eventbrite.

