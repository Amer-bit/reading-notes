# API Server

## Router 

`router.param(name, callback)`

Adds callback triggers to route parameters, where name is the name of the parameter and callback is the callback function. Although name is technically optional, using this method without it is deprecated starting with Express v4.11.0 (see below).

The parameters of the callback function are:

* req, the request object.
* res, the response object.
* next, indicating the next middleware function.
* The value of the name parameter.
* The name of the parameter.
Unlike app.param(), router.param() does not accept an array of route parameters.Param callback functions are local to the router on which they are defined. They are not inherited by mounted apps or routers. Hence, param callbacks defined on router will be triggered only by route parameters defined on router routes.

A param callback will be called only once in a request-response cycle, even if the parameter is matched in multiple routes



# `Middleware`
Middleware (also called pre and post hooks) are functions which are passed control during execution of asynchronous functions. Middleware is specified on the schema level and is useful for writing plugins

`Types of Middleware`

Mongoose has 4 types of middleware: document middleware, model middleware, aggregate middleware, and query middleware. Document middleware is supported for the following document functions. In document middleware functions, this refers to the document.




### Sub Documents in Mongoose
*Sub Documents* are great for supportive data such as comments on a blog post, but they’re not “populated” unless you do this manually. This can be difficult to manage, and does represent a downside to NoSQL modeling. <br />  

### What is a Subdocument?
Subdocuments are similar to normal documents. Nested schemas can have middleware, custom validation logic, virtuals, and any other feature top-level schemas can use. The major difference is that subdocuments are not saved individually, they are saved whenever their top-level parent document is saved.

### Joining Data/Documents in Mongo
noSQL Databases don’t really join, and doing so generally is considered an anti-pattern. and you should modeling things in the most logical way for this data store.<br />  

- *populate()* is a method we can use in Mongoose to connect 2 collections
  - Method 1: physically joining using a reference to another collection
  - Method 2: Virtual Population
    - Create a virtual field in a document pointed to a field in another one.
    - In *pre('find')* you do a collection “on the fly” which can be more efficient than storing the relation.

- Pre and Post hooks (middleware)
  - Mongoose allows you to inject logic at various points in the lifecycle of a data record.
    - User can perform validation, normalization