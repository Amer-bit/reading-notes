# Error Handling and Debugging (p.456)
**Order of execution**

## Exection Context
The JavaScript interpreter uses the concept of execution contexts.
There is one global execution context; plus, each function creates a new
new execution context. They correspond to variable scope.

## EXECUTION CONTEXT & HOISTING
Each time a script enters a new execution context, there are two phases
of activity:

1. PREPARE
* The new scope is created
* Variables, functions, and arguments are created
* The value of the this keyword is determined

2 EXECUTE
* Now it can assign values to variables
* Reference functions and run their code
* Execute statements

Understanding that these two phases happen helps with understanding a concept called **hoisting**

## Scopes
Functions in JavaScript are said to have lexical scope. They are linked to the object they were defined within. So, for each execution context, the scope is the current execution context's variables object, plus the
variables object for each parent execution context

## Errors 
If a JavaScript statement generates an error, then it throws an exception. At that point, the interpreter stops and looks for exception-handling code.

If you are anticipating that something in your code may cause an error, you can use a set of statements to handle the error

## Errror Objects
Error objects can help you find where your mistakes are and browsers have tools to help you read them.

## Handling Errors
1. DEBUG THE SCRIPT TO FIX ERRORS
2. HANDLE ERRORS GRACEFULLY

## Debgging Workflow


