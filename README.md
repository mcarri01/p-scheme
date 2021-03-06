# p-scheme

## Overview
p-scheme is a Turing-complete programming language that I developed over the course of the past three months (October 2017-present).  Written in Python, the language features five datatypes--numbers (both floats and ints), booleans, strings, lists, and a NoneType object--and supports over 60 primitive functions, including those for variable assignment, conditionals, loops, assertions, input, output, and user-defined functions.  The language is fully functional, with a complete type-checking system, proper error-handling, and separate environments for functions, global variables, and local variables.

## Background
p-scheme was originally conceived by myself and Matthew Carrington-Fair at a Hackathon and evolved from there into a complete language.  While Matthew's contributions helped laid the language's foundation, post-Hackathon I developed p-scheme on my own.  Much of the inspiration for this project came not through asking the question "should this be done?" but rather by asking "can this be done?"  As a result, some of p-scheme's features are rather bizarre: variables can simultaneously hold values of different types, indexing of lists is date-based, and all p-scheme code is written in suffix notation.

## Sublime Package
For the user's convenience, a Sublime highlighting package has been provided for p-scheme.  To install it, simply copy the `sublime-pscheme` directory into whatever directory installed Sublime packages live in on your machine and restart Sublime.  Sublime will now recognize any file ending with a `.pscm` extension as a p-scheme file and will use the package.  Alternatively, p-scheme highlighting can be manually selected from the list of languages in the lower righthand corner of the screen.

## Running a Program
To run a p-scheme program, the user must be within the `src` directory, which contains the p-scheme source code.  Simply enter the command 
```
./run.py [path/to/filename].pscm
```
and the p-scheme file will be executed.  The `examples` directory contains some sample p-scheme programs that I have written.  If one were in the `src` directory and wished to run `fib.pscm`, for example, they would enter
```
./run.py ../examples/fib.pscm
```

## Going Forwards
p-scheme is not finished.  There are still a number of features I would like to implement in the language.  First on the list will be optimizing the language; at the moment, performance is slow.  In addition, I would also like to include anonymous functions, higher-order list functions, bitwise operations, and a type-hierarchy system.  The final step will be writing a full documentation guide.  Keep checking back for updates that will be pushed as more features are implemented!
