# APIs #

## What does REST stand for? ##
REST stands for REpresentational State Transfer and it is an architectural style for building distributed systems based on hypermedia. REST is independent of any underlying protocol and is not necessarily tied to HTTP. However, most common REST API implementations use HTTP as the application protocol

## REST APIs are designed around *Resources*. ##

## What is an identifier of a resource? Give an example. ##
 resource has an identifier, which is a URI that uniquely identifies a resource.
 
 For example, the URI for a particular customer order might be:
 `https://adventure-works.com/orders/1`
 
## What are the most common HTTP verbs? ##
The primary or most-commonly-used HTTP verbs (or methods, as they are properly called) are POST, GET, PUT, PATCH, and DELETE.

- GET retrieves a representation of the resource at the specified URI. The body of the response message contains the details of the requested resource.
- POST creates a new resource at the specified URI. The body of the request message provides the details of the new resource. Note that POST can also be used to trigger operations that don't actually create resources.
- PUT either creates or replaces the resource at the specified URI. The body of the request message specifies the resource to be created or updated.
- PATCH performs a partial update of a resource. The request body specifies the set of changes to apply to the resource.
- DELETE removes the resource at the specified URI.

## What should the URIs be based on? ##
Resource URIs should be based on nouns (the resource) and not verbs (the operations on the resource).

## Give an example of a good URI. ##
```
https://adventure-works.com/orders // Good

https://adventure-works.com/create-order // Avoid
```

*Avoid requiring resource URIs more complex than collection/item/collection.*

## What does it mean to have a ‘chatty’ web API? Is this a good or a bad thing? ##
Another factor is that all web requests impose a load on the web server. 
The more requests, the bigger the load. Therefore, try to **avoid "chatty"** web APIs that expose a large number of small resources. Such an API may require a client application to send multiple requests to find all of the data that it requires. Instead, you might want to denormalize the data and combine related information into bigger resources that can be retrieved with a single request. However, you need to balance this approach against the overhead of fetching data that the client doesn't need. Retrieving large objects can increase the latency of a request and incur additional bandwidth costs. 


## What status code does a successful GET request return? ##
200 (OK)

## What status code does an unsuccessful GET request return? ##
404 (Not Found)

## What status code does a successful POST request return? ##
201 (Created)

## What status code does a successful DELETE request return? ##
204 (No Content)

### *[Source](https://docs.microsoft.com/en-us/azure/architecture/best-practices/api-design)*  ###


<hr>
<hr>

## Useful Resources ##

- [RegExr](https://regexr.com/)
- [Regex Tutorial](https://medium.com/factory-mind/regex-tutorial-a-simple-cheatsheet-by-examples-649dc1c3f285)
- [Regex 101](https://regex101.com/)


<hr>
<hr>

## Things I want to know more about
