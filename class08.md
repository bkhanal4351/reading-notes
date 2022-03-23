. What does REST stand for?
- representational state transfer

. REST APIs are designed around a ____.
- REST APIs are designed around resources, which are any kind of object, data, or service that can be accessed by the client.

. What is an identifer of a resource? Give an example.
- A resource has an identifier, which is a URI that uniquely identifies that resource. For example, the URI for a particular customer order might be: 
https://adventure-works.com/orders/1

. What are the most common HTTP verbs?
- The most common operations are GET, POST, PUT, PATCH, and DELETE.

. What should the URIs be based on?
- URIs should be based on nouns (the resource)
 
. Give an example of a good URI.
- https://adventure-works.com/orders

. What does it mean to have a ‘chatty’ web API? Is this a good or a bad thing?
- Having multiple request which adds bigger load to the web server. It is bad

. What status code does a successful GET request return?
- GET retrieves a representation of the resource at the specified URI. The body of the response message contains the details of the requested resource.

. What status code does an unsuccessful GET request return?
- 

. What status code does a successful POST request return?
- A POST request creates a resource. The server assigns a URI for the new resource, and returns that URI to the client. In the REST model, you frequently apply POST requests to collections. The new resource is added to the collection. A POST request can also be used to submit data for processing to an existing resource, without any new resource being created.

. What status code does a successful DELETE request return?
- DELETE removes the resource at the specified URI.

Note taken from (https://docs.microsoft.com/en-us/azure/architecture/best-practices/api-design)