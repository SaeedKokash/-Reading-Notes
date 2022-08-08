# CRUD #

## In your own words, describe what each group of status code represents: ##
- 100’s = indicates that everything so far is OK and that the client should continue with the request or ignore it if it is already finished
- 200’s = indicates that the request has succeeded. A 200 response is cacheable by default. The meaning of a success depends on the HTTP request method: GET : The resource has been fetched and is transmitted in the message body.
- 300’s = indicates that the request has more than one possible responses. The user-agent or the user should choose one of them. As there is no standardized way of choosing one of the responses, this response code is very rarely used.
- 400’s = indicates that the server cannot or will not process the request due to something that is perceived to be a client error (for example, malformed request syntax, invalid request message framing, or deceptive request routing).
- 500’s = indicates that the server encountered an unexpected condition that prevented it from fulfilling the request. This error is usually returned by the server when no other error code is suitable.

## What is a status code 202? ##
202 Accepted - Often used for asynchronous processing. This code tells the client that the request was valid, but its processing will finish sometime in the future. The response body should include an URL to the finished resource with some information about when it will be available, or an URL to some monitoring endpoint that tells the client when the resource is available.

## What is a status code 308? ##
308 Permanent Redirect - This tells the client to use another URL to access the resource and not use the current URL anymore. It’s helpful when we have multiple endpoints for one resource, but don’t want to implement reading from all of them.
 
## What code would you use if an update didn’t return data to a client? ##
204 No Content 

## What code would you use if a resource used to exist but no longer does? ##
410 Gone

## What is the ‘Forbidden’ status code? ##
403 Forbidden - The client has authorized or doesn’t need to authorize itself, but still has no permissions to access the resource.

### *[Source](https://www.moesif.com/blog/technical/api-design/Which-HTTP-Status-Code-To-Use-For-Every-CRUD-App/)*  ###

<hr>
<hr>

# Build A REST API With Node.js, Express, & MongoDB - Quick   #


## Why do we need to pull our MongoDB database string out of our server and put it into our .env? ##
because when we deploy our application we are going to want to use something thats not our local host and we need to hide it for security


## What is middleware? ##
code that runs when the server gets a request but before it gets passed to your routes

## What does `app.use(express.json())` do? ##
it sets up our server to accept JSON as abody instead of a post element or get element or etc...

## What does the `/:id` mean in a route? ##
it means that it is a parameter that we can access by typing in req.params.id, this will give us access to whatever the user passes after the first slash

## What is the difference between PUT and PATCH? ##
we use patch when we only want to update based on what the user passes us in specific, if we use put; it will update all the information all at once instead of the information that gets passed

## How do you make a default value in a schema? ##
we add a default: Date.now for example which will take a date at the moment if the date isnt available.

## What does a 500 error status code mean? ##
it means that there is an error on your server, it means that the actual server had an unexpected error and that it has nothing to do with the client

## What is the difference between a status 200 and a status 201? ##
201 means successfuly **creating** an object (specific), 200 means everything was successful 

### *[Source](https://www.youtube.com/channel/UCFbNIlppjAuEX4znoulh0Cw)  ###

<hr>
<hr>

## Useful Resources ##

<hr>
<hr>

## Things I want to know more about
