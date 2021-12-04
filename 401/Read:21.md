# Django Models

![Django Models](https://static.codingforentrepreneurs.com/media/projects/django-models-unleashed-2021/images/share/Django_Models_Unleashed_share.jpg)

A model is the single, definitive source of information about your data. It contains the essential fields and behaviors of the data you’re storing. Generally, each model maps to a single database table.

The basics:

* Each model is a Python class that subclasses **`django.db.models.Model`**.
* Each attribute of the model represents a database field.
* With all of this, Django gives you an automatically-generated database-access API

This example model defines a *`Person`*, which has a *`first_name`* and *`last_name`*:

```python
from django.db import models

class Person(models.Model):
    first_name = models.CharField(max_length=30)
    last_name = models.CharField(max_length=30)
```

## The Django admin site

One of the most powerful parts of **`Django`** is the automatic admin interface. It reads metadata from your models to provide a quick, model-centric interface where trusted users can manage content on your site. 

The admin’s recommended use is limited to an organization’s internal management tool. It’s not intended for building your entire front end around.

The admin is enabled in the default project template used by *`startproject`*.

The *`ModelAdmin`* class is the representation of a model in the admin interface. Usually, these are stored in a file named *`admin.py`* in your application. Let’s take a look at an example of the ModelAdmin:

```python
from django.contrib import admin
from myapp.models import Author

class AuthorAdmin(admin.ModelAdmin):
    pass
admin.site.register(Author, AuthorAdmin)
```