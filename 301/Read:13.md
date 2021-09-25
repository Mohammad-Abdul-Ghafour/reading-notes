# CRUD

## Status Codes :
1. **`100's`** :
    * These are informational status codes; they usually tell the client that the header part of the request has been received and the server will try to comply with a transmission demand of the client.
2. **`200's`** :
    * These are the success codes. They tell the client that its request was accepted.
3. **`300's`** :
    * These are redirection codes. They tell the client that the resource they are requesting isn’t available at the expected location anymore.
4. **`400's`** :
    * These are the client error codes. They are all about invalid requests a client sent to a server. 
5. **`500's`** :
    * These are the server error codes. Often they indicate problems with overwhelmed servers or unreachable servers behind proxies.

## What is a status code 202 ?

The request has been received but not yet acted upon.

## What is a status code 308 ?

This means that the resource is now permanently located at another URI.

## What code would you use if an update didn’t return data to a client ?

**`204 No Content`** :
* A proper code for updates that don’t return data to the client, for example when just saving a currently edited document.

## What code would you use if a resource used to exist but no longer does ?

**`410 Gone`** :
* This is like 404 but we know that the resource existed in the past, but it got deleted or somehow moved, and we don’t know where.

## What is the ‘Forbidden’ status code ?

**`403 Forbidden`** :
* The client has authorized or doesn’t need to authorize itself, but still has no permissions to access the resource.

## Why do we need to pull our MongoDB database string out of our server and put it into our .env ?

Because we don't want to push our MongoDB database string for security reasons.

## What is middleware ?

**`Middleware`** is software that is used to bridge the gap between applications and other tools or databases.

## What does app.use(express.json()) do?

The express.json() function is a built-in middleware function in Express. It parses incoming requests with JSON payloads and is based on body-parser.

## What does the /:id mean in a route ?

Route parameters are named URL segments that are used to capture the values specified at their position in the URL. The captured values are populated in the req.params object, with the name of the route parameter specified in the path as their respective keys.

## What is the difference between PUT and PATCH ?

**`PUT`** is a method of modifying resource where the client sends data that updates the entire resource.

**`PATCH`** is a method of modifying resources where the client sends partial data that is to be updated without modifying the entire data.

## How do you make a default value in a schema ?

By using **`default`** :
* Your schemas can define default values for certain paths. If you create a new document without that path set, the default will kick in.

## What does a 500 error status code mean ?

**`500 Internal Server Error`** :
* The server has encountered a situation it doesn't know how to handle.

## What is the difference between a status 200 and a status 201 ?

**`200 OK`** :
* The request has succeeded. The meaning of the success depends on the HTTP method.

**`201 Created`** :
* The request has succeeded and a new resource has been created as a result. This is typically the response sent after POST requests, or some PUT requests.