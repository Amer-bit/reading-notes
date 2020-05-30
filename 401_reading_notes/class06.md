# HTTP and REST
## What is HTTP:(Hyper Text Transfer Protocol)

### Important things about http:
* connectionless: after making the request the client disconnect from the server
   then the response is ready the server re-establish the connection again
and deliver the response.
*  the HTTP can deliver any sort of data as long as the two computer are 
   able to read it .

* stateless protocol: the client and server know about each other just during 
   the current request, if it closes, and the two computers want to 
   connect again, they need to provide information to each other anew, and the 
   connection handled as the very first one.

the request and the response has the same parts:
#### first the request :
- start line: contain:
  - the method: tells the server what it should do 
  - URI :Uniform Resource Identifier : to tell the server what are we requestont
  - HTTP version :
- header:contain:
  - host :the address of the server 
  - accept language :the language 
  - accept : mime type:filetype/extention :eg(text/html)

#### second the response:
- start line : contain:
  - http/version
  - status code : tells the client if the request succeeded or failed

## REST(REpresentational State Transfer)
means by which we can reference, manipulate, and transfer state. Rest uses a common set of methods (called “verbs”) to operate on the state of a resource (“noun”), generally using HTTP as the transfer protocol.