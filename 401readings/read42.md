# Pythonisms

## Dunder (Magic, Special) Methods

I must admit, this is the coolest feature of python I've came across.
It is really part of python spirit that makes me love it. they make my life much much easier.

Dunder methods basically let you emulate the behavior of built-in types! meaning you can for example define a length for your classes, or maybe iterate on an item in it even if it had the weirdest shape.

here is a list of some of the most important ones:

Object Initialization: __init__

Object Representation: __str__, __repr__

Iteration: __len__, __getitem__, __reversed__

Operator Overloading for Comparing Accounts: __eq__, __lt__

Operator Overloading for Merging Accounts: __add__

Callable Python Objects: __call__

Context Manager Support and the With Statement: __enter__, __exit__

## Iterators

you can make a for loop in python using "in" keyword, like this:

```
for i in array:
  pass
```

how does this work behind the scenes? well, to iterate a data structure in this way, it should support __itr__ and __next__ dunder methods. 

It first prepared the repeater object for iteration by calling its __iter__ method. This returned the actual iterator object.
After that, the loop repeatedly calls the iterator object’s __next__ method to retrieve values from it.
