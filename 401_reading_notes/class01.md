### Why would you want to run JavaScript code outside of a browser?
 javascript code will interact with your database and can be used to create RESTful APIs.
Node.js: shines in real-time web applications employing push technology over websockets
Node.js: use non-blocking, event-driven I/O to remain lightweight and efficient in the face of data-intensive real-time applications that run across distributed devices.

### What is the difference between a module and a package?
A package is a file or directory that is described by a package.json file
A **package** is any of the following:

a) A folder containing a program described by a package.json file.
b) A gzipped tarball containing (a).
c) A URL that resolves to (b).
d) A <name>@<version> that is published on the registry with (c).
e) A <name>@<tag> that points to (d).
f) A <name> that has a latest tag satisfying (e).
g) A git url that, when cloned, results in (a).

A **module** is any file or directory in the node_modules directory that can be loaded by the Node.js require() function.

a **module** must be one of the following:

A folder with a package.json file containing a "main" field.
A folder with an index.js file in it.
A JavaScript file.

### What does the node package manager do?
The public npm registry is a database of JavaScript packages, each comprised of software and metadata. Open source developers and developers at companies use the npm registry to contribute packages to the entire community or members of their Orgs, and download packages to use in their own projects.

### Ecosystem
is “a collection of software projects, which are developed and co-evolve in the same environment”. The environment can be organizational (a company), social (an open-source community), or technical (the Ruby ecosystem). The ecosystem metaphor is used in order to denote an analysis which takes into account multiple software systems.[7] The most frequent of such analyses is static analysis of the source code of the component systems of the ecosystem.

### Node.js
 an asynchronous event-driven JavaScript runtime, Node.js is designed to build scalable network applications.

 Node.js is similar in design to, and influenced by, systems like Ruby's Event Machine and Python's Twisted. Node.js takes the event model a bit further. It presents an event loop as a runtime construct instead of as a library. In other systems, there is always a blocking call to start the event-loop.

 ### V8 Engine
 V8 is Google’s open source high-performance JavaScript and WebAssembly engine, written in C++. It is used in Chrome and in Node.js, among others. It implements ECMAScript and WebAssembly, and runs on Windows 7 or later, macOS 10.12+, and Linux systems that use x64, IA-32, ARM, or MIPS processors. V8 can run standalone, or can be embedded into any C++ application.

 What V8 can do:
1. Compiles and executes JS code
2. Handling call stack — running your JS functions in some order
3. Managing memory allocation for objects — the memory heap
4. Garbage collection — of objects which are no longer in use
5. Provide all the data types, operators, objects and functions

### Interpeter
An interpreter is a computer program, which coverts each high-level program statement into the machine code. This includes source code, pre-compiled code, and scripts.

**Programming Steps**: 
* Create the Program
* No linking of files or machine code generation
* Source statements executed line by line DURING Execution

**Advantage**
Interpreters are easier to use, especially for beginners.

**Disadvantage**
Interpreted programs can run on computers that have the corresponding interpreter.

**Machine code**
Not saving machine code at all.

**Running Time**
Interpreted code run slower

**Best Suited for**
For web environments, where load times are important. Due to all the exhaustive analysis is done, compiles take relatively larger time to compile even small code that may not be run multiple times. In such cases, interpreters are better.

**Usage**
It is best suited for the program and developmentenvironment.

**Dynamic Typing**
Interpreted languages support Dynamic Typing

**Error execution**
The interpreter reads a single statement and shows the error if any. You must correct the error to interpret next line.

### Compiler 
A compiler is a computer program that transforms code written in a high-level programming language into the machine code. It is a program which translates the human-readable code to a language a computer processor understands (binary 1 and 0 bits). The computer processes the machine code to perform the corresponding tasks.

**Programming Steps**: 
* Create the program.
* Compile will parse or analyses all of the language statements for its correctness. If incorrect, throws an error
* If no error, the compiler will convert source code to machine code.
* It links different code files into a runnable program(know as exe)
* Run the Program

**Advantage**
The program code is already translated into machine code. Thus, it code execution time is less.

**Disadvantage**
You can't change the program without going back to the source code.

**Machine code**
Store machine language as machine code on the disk

**Running Time**
Compiled code run faster

**Best Suited for**
Bounded to the specific target machine and cannot be ported. C and C++ are a most popular a programming language which uses compilation model.

**Usage**
It is best suited for the Production Environment

**Dynamic Typing**
Difficult to implement as compilers cannot predict what happens at turn time.

**Error execution**
Compiler displays all errors and warning at the compilation time. Therefore, you can't run the program without fixing errors

![inter](https://www.guru99.com/images/1/053018_0616_CompilervsI1.png)