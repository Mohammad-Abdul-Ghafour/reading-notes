# Django Custom User

The authentication that comes with Django is good enough for most common cases, but you may have needs not met by the out-of-the-box defaults.

The default User model in Django uses a username to uniquely identify a user during authentication. If you'd rather use an email address, you'll need to create a **`custom User model`**.

You can give your models custom permissions that can be checked through Django’s authorization system.

## AbstractUser vs AbstractBaseUser

* **`AbstractUser`** : Use this option if you are happy with the existing fields on the User model and just want to remove the username field.
* **`AbstractBaseUser`** : Use this option if you want to start from scratch by creating your own, completely new User model.

## How to create Custom User ?

1. Create a custom User model and Manager
2. Update *`settings.py`*
3. Customize the *`UserCreationForm`* and *`UserChangeForm`* forms
4. Update the admin

## DjangoX

![DjangoX Logo](https://raw.githubusercontent.com/hanshendrickx/djangox/master/logo.png)

A framework for launching new Django projects quickly. Comes with a custom user model, email/password authentication, options for social authentication via Google/Facebook/Twitter/etc, and static assets.

### How To Install GjangoX ?

DjangoX can be installed via Pip, Pipenv, or Docker depending upon your setup. To start, clone the repo to your local computer and change into the proper directory.

* Pip

```
$ python3 -m venv djangox
$ source djangox/bin/activate
(djangox) $ pip install -r requirements.txt
(djangox) $ python manage.py migrate
(djangox) $ python manage.py createsuperuser
(djangox) $ python manage.py runserver
# Load the site at http://127.0.0.1:8000

```

* Pipenv

```
$ pipenv install
$ pipenv shell
(djangox) $ python manage.py migrate
(djangox) $ python manage.py createsuperuser
(djangox) $ python manage.py runserver
# Load the site at http://127.0.0.1:8000

```

* Docker

```
$ docker build .
$ docker-compose up -d
$ docker-compose exec web python manage.py migrate
$ docker-compose exec web python manage.py createsuperuser
# Load the site at http://127.0.0.1:8000

```

### Setup DjangoX

```
# Run Migrations
(djangox) $ python manage.py migrate

# Create a Superuser
(djangox) $ python manage.py createsuperuser

# Confirm everything is working:
(djangox) $ python manage.py runserver

# Load the site at http://127.0.0.1:8000

```