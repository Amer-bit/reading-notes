# Middleware
Middleware functions are functions that have access to the request object (req), the response object (res), and the next middleware function in the application’s request-response cycle. These functions are used to modify req and res objects for tasks like parsing request bodies, adding response headers, etc.

Middleware functions can perform the following tasks:

* Execute any code.
* Make changes to the request and the response objects.
* End the request-response cycle.
* Call the next middleware function in the stack.

**NOTE**: Each function receives request, response and next as parameters

**Types of middleware**:

1. Application:

Bind application-level middleware to an instance of the app object by using the **app.use() and app.METHOD() functions**, where METHOD is the HTTP method of the request that the middleware function handles (such as GET, PUT, or POST) in lowercase.

2. Route

Router-level middleware works in the same way as application-level middleware, except it is bound to an instance of **express.Router().**
Load router-level middleware by using the **router.use() and router.METHOD()** functions.

3. Error-handling middleware

Define error-handling middleware functions in the same way as other middleware functions, except with four arguments instead of three, specifically with the signature (err, req, res, next))


**Middleware Application**

* Error Handling
* Bringing in other routes
* Applies Defaults
* JSON, Body and Form Parsing
* Runs on every request


**Route Middleware**

* Dealing with specific things for a route
* Generally, things many routes would participate in
* Are you logged in?
* What is your IP?
* Have we seen you here before?


**Middleware are useful in:**

* Logging
* Dynamic Model Loading
* Browser, Location, User specific content
* Consistent Data Transition/Modeling/Preparation (Pre-Render)


## Server Testing
* Generally, avoid starting the actual server for testing
* Instead, export your server as a module in a library
* Then, you can use supertest to run your tests
     This will hit your routes as though your server was running, without actually starting it
     That’s one less thing to go wrong (eliminate variables when testing!)


**Test Pyramid**

* Server Testing crosses boundaries
    * Units: Server Internal Functions
        * Mock any integrations (like data fetching)

    * Integration: How it connects to other services
        * Really connect to other services (hard dependencies)
        
    * Acceptance
        * The server might be a dependency of some other test
