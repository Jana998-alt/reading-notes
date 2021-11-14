# Read04 

## Classes and Objects
Classes are templets to “make” objects. 
Ok lets go backwards a little bit. Objects in programming are representations of real world objects with properties and methods. For example: class particles is a template to create particles, like electrons, protons, …
All particles have properties like mass, charge, spin … and methods, like: transition, decay, … 


This is how a simple class looks like: 


```
class MyClass:
    variable = "blah"

    def function(self):
        print("This is a message inside the class.")
#to create an object that belongs to a class:
myobjectx = MyClass()
```

## Thinking Recursively
_“Problems (in life and also in computer science) can often seem big and scary. But if we keep chipping away at them, more often than not we can break them down into smaller chunks trivial enough to solve. This is the essence of thinking recursively”_


A recursive function is a function defined in terms of itself via self-referential expressions.


This means that the function will continue to call itself and repeat its behavior until some condition is met to return a result. All recursive functions share a common structure made up of two parts: base case and recursive case.

## Pytest Fixtures and Coverage
When you're writing tests, you're rarely going to write just one or two. Rather, you're going to write an entire "test suite", with each test aiming to check a different path through your code. In many cases, this means you'll have a few tests with similar characteristics, something that pytest handles with "parametrized tests".


But it gets even better. Your fixture might act like data, in that you don't invoke it with parentheses. But it's actually a function under the hood, which means it executes every time you invoke a test using that fixture. This means that the fixture, in contrast with regular-old data, can make calculations and decisions.
