# Django CRUD and Forms

![Django Forms](https://data-flair.training/blogs/wp-content/uploads/sites/2/2019/05/Django-forms.jpg)

**`Forms`** are a collection of **`HTML`** elements to take input from the user. In simple words, whenever you give any kind of instruction or input on web, that is known as a form.

The input elements come inside **`<form></form>`** tags. It is collectively called as HTML form. All the websites use forms each having different use-cases.

## GET and POST in Django :
**`GET`** and **`POST`** are the only HTTP methods to use when dealing with forms.

**`Django’s`** login form is returned using the **`POST`** method, in which the browser bundles up the form data, encodes it for transmission, sends it to the server, and then receives back its response.

**`GET`**, by contrast, bundles the submitted data into a string, and uses this to compose a **`URL`**. The **`URL`** contains the address where the data must be sent, as well as the data keys and values.

## Building a form in Django :

We already know what we want our HTML form to look like. Our starting point for it in Django is this:

```python
from django import forms

class NameForm(forms.Form):
    your_name = forms.CharField(label='Your name', max_length=100)
```