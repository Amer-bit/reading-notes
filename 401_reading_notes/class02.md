### Name 3 advantages to Test Driven Development
1. Better understanding of the program design because testing make you reallt think about what the purpose of the program and you will plan your work before even implementing the code
2. Better code Quality
3. Flexible and modular code

### What is one downside of Test Driven Development
Big time investment and Additional Complexity.

### What’s the primary difference between ES6 Classes and Constructor/Prototype Classes?
 classes allows us to create constructor functions with less lines of code and in a way that resembles classical languages. But under the hood this all means pretty much nothing.

### Name a use case for a static method
it make sense to call this method, even if no object has been constructed
it can be accessed using class instead the instance of that class.


## What is functional programming?
Functional programming is a programming paradigm — a style of building the structure and elements of computer programs — that treats computation as the evaluation of mathematical functions and avoids changing-state and mutable data 

### Pure Function

The first fundamintal concept i functional programming is pure function and we can identify pure function using two factors:

1. It returns the same result if given the same arguments (it is also referred as deterministic)
2. It does not cause any observable side effects

**Pure functions benefits**

The code’s definitely easier to test. We don’t need to mock anything. So we can unit test pure functions with different contexts. Mutability is discouraged in functional programming.

### Immutability
Unchanging over time or unable to be changed.

When data is immutable, its state cannot change after it’s created. If you want to change an immutable object, you can’t. Instead, you create a new object with the new value.

## Continuous Integration (CI)
Continuous Integration (CI) is a development practice that requires developers to integrate code into a shared repository several times a day. Each check-in is then verified by an automated build, allowing teams to detect problems early.

By integrating regularly, you can detect errors quickly, and locate them more easily.


## Unit Testing
UNIT TESTING is a type of software testing where individual units or components of a software are tested. The purpose is to validate that each unit of the software code performs as expected. Unit Testing is done during the development (coding phase) of an application by the developers. Unit Tests isolate a section of code and verify its correctness. A unit may be an individual function, method, procedure, module, or object.

Why Unit Testing?
Sometimes software developers attempt to save time by doing minimal unit testing. This is a myth because skipping on unit testing leads to higher Defect fixing costs during System Testing, Integration Testing and even Beta Testing after the application is completed. **Proper unit testing done during the development stage** saves both time and money in the end. Here, are key reasons to perform unit testing.

1. Unit tests help to fix bugs early in the development cycle and save costs.
2. It helps the developers to understand the code base and enables them to make changes quickly
3. Good unit tests serve as project documentation
4. Unit tests help with code re-use. Migrate both your code andyour tests to your new project. Tweak the code until the tests run again.

**Unit Testing is of two types**

* Manual
* Automated

higher-order function
object
object-oriented programming (OOP)
class
prototype
super
inheritance
constructor
instance
context
this
Test Driven Development (TDD)
Jest
unit test