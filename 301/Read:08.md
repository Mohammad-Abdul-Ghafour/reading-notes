# APIs

## What does REST stand for ?
(*`REST`*) stands for **`Representational State Transfer`**

REST APIs are designed around a resources.

## What is an identifer of a resource ?
A resource has an identifier, which is a URI that uniquely identifies that resource. For example, the URI for a particular customer order might be:

```
https://adventure-works.com/orders/1
```
## What are the most common HTTP verbs ?

The most common operations are :
* *`GET`*
* *`POST`*
* *`PUT`*
* *`PATCH`*
* *`DELETE`*

## What should the URIs be based on ?

**`URIs`** should be based on nouns (the resource) and not verbs (the operations on the resource).

For Example :

```
https://adventure-works.com/orders // Good

https://adventure-works.com/create-order // Avoid
```

## What does it mean to have a ‘chatty’ web API ? Is this a good or a bad thing ?

**`Chatty`** web APIs that expose a large number of small resources. Such an API may require a client application to send multiple requests to find all of the data that it requires.

And of course we should try to avoid them.

## What status code does a successful GET request return ?

A *`successful`* **`GET`** method typically returns HTTP status code 200 (OK).

## What status code does an unsuccessful GET request return ?

A *`unsuccessful`* **`GET`** method typically returns HTTP status code 404 (Not Found).

## What status code does a successful POST request return ?

If a **`POST`** method creates a new resource, it returns HTTP status code 201 (Created).

## What status code does a successful DELETE request return ?

If the **`DELETE`** operation is successful, the web server should respond with HTTP status code 204 (No Content).

