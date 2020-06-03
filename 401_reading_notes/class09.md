## API Server


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