# Permissions & Postgresql

![Permissions](https://files.realpython.com/media/Django-Rest-Framework-An-Introduction_Watermarked.6050ea8850a3.jpeg)

**`Permissions`** are used to grant or deny access for different users to different parts of the APIs, the simplest style of permission would be to allow access to any authenticated user, and deny access to any unauthenticated user.

Before running the body of the view, each permission in the list will be checked. If any permission check fails, an *`exceptions.PermissionDenied`* or *`exceptions.NotAuthenticated`* will be raised, and the main body of the view will not run.

## Setting the permission policy

The default permission policy may be set globally, using the *`DEFAULT_PERMISSION_CLASSES`* inside **`REST_FRAMEWORK`** in *`setting.py`*.

For example:

```python
REST_FRAMEWORK = {
    'DEFAULT_PERMISSION_CLASSES': [
        'rest_framework.permissions.IsAuthenticated',
    ]
}
```

You can also set the authentication policy on a per-view, or per-viewset basis, using the APIView class-based views.

```python
from rest_framework.permissions import IsAuthenticated
from rest_framework.response import Response
from rest_framework.views import APIView

class ExampleView(APIView):
    permission_classes = [IsAuthenticated]

    def get(self, request, format=None):
        content = {
            'status': 'request was permitted'
        }
        return Response(content)
```

## API Reference

1. AllowAny
2. IsAuthenticated
3. IsAdminUser
4. IsAuthenticatedOrReadOnly

## Custom permissions

To implement a custom permission, override BasePermission and implement one or both of the following methods :

* **`.has_permission(self, request, view)`**
* **`.has_object_permission(self, request, view, obj)`**

```python
from rest_framework import permissions

class CustomerAccessPermission(permissions.BasePermission):
    message = 'Adding customers not allowed.'

    def has_permission(self, request, view):
         ...
```

