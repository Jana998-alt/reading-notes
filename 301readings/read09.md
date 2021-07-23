# read09: FUNCTIONAL PROGRAMMING

## Functional Programming Concepts 

- What is functional programming?

Functional programming is a programming paradigm — a style of building the structure and elements of computer programs — that treats computation as the evaluation of mathematical functions and avoids changing-state and mutable data — Wikipedia

- What is a pure function and how do we know if something is a pure function?

definition of purity:
It returns the same result if given the same arguments (it is also referred as deterministic)
It does not cause any observable side effects

- What are the benefits of a pure function?

The code’s definitely easier to test. We don’t need to mock anything. So we can unit test pure functions with different contexts.

What is immutability?

Unchanging over time or unable to be changed. When data is immutable, its state cannot change after it’s created. If you want to change an immutable object, you can’t. Instead, you create a new object with the new value.

What is Referential transparency?

pure functions + immutable data = referential transparency


## Node JS Tutorial for Beginners #6 - Modules and require()

What is a module?

Module in is a simple or complex functionality organized in single or multiple JavaScript files which can be reused throughout the application

What does the word ‘require’ do?

if we want to use a functionality from one module in another module. 

How do we bring another module into the file the we are working in?

by importing the module (through require) and storing it in a variable.

What do we have to do to make a module available?

export the module
