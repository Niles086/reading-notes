# APIs

## [API Design Best Practices](https://docs.microsoft.com/en-us/azure/architecture/best-practices/api-design)

1. What does REST stand for? Representational State Transfer
1. REST APIs are designed around a ____. Designed around resources
1. What is an identifier of a resource? Give an example. A URI (Uniform Resource Locator) that identifies that resource
1. What are the most common HTTP verbs? GET, POST, PUT, PATCH, and DELETE
1. What should the URIs be based on? concept of resources
1. Give an example of a good URI. GET /blog/posts/1
1. What does it mean to have a ‘chatty’ web API? Is this a good or a bad thing? It is a bad thing. It is when you impose a lot of data on a web server; expose a large number of small resources
1. What status code does a successful GET request return? HTTP status code 200
1. What status code does an unsuccessful GET request return? 404 if the resource not found. 204 if found but no response body included in HTTP response
1. What status code does a successful POST request return? HTTP status code 201
1. What status code does a successful DELETE request return? HTTP status code 204
