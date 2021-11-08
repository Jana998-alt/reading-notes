# Game of Greed 2

## Python Scope

scope (of a name) is what defines the accessibility of this name from the area of code.

there are 2 types:

* Global scope: The names that you define in this scope are available to all your code.

* Local scope: The names that you define in this scope are only available or visible to the code within the scope.

_Python scopes_ are implemented as dictionaries that map names to objects. These dictionaries are commonly called namespaces. These are the concrete mechanisms that Python uses to store names. They’re stored in a special attribute called .__dict__.


To get a list with all the names defined at the top level of the module, use this code:

```
import sys
>>> sys.__dict__.keys()
dict_keys(['__name__', '__doc__', '__package__',..., 'argv', 'ps1', 'ps2'])
```

this means that these names can be accessed **through** this dictionary. this can be done by: 

* Using the dot notation on the module’s name in the form module.name
* Using a subscription operation on .__dict__ in the form module.__dict__['name']

**LEGB rule** (Local, Enclosing, Global, and Built-in)
a rule for finding variables in different scopes. 

* Local (or function) scope: is the code block or body of any Python function or lambda expression. It’s created at function call, not at function definition.

* Enclosing (or nonlocal) scope is a special scope that only exists for nested functions. If the local scope is an inner or nested function, then the enclosing scope is the scope of the outer or enclosing function. 

* Global (or module) scope is the top-most scope in a Python program, script, or module.

* Built-in scope is a special Python scope that’s created or loaded whenever you run a script or open an interactive session. This scope contains names such as keywords, functions, exceptions, and other attributes that are built into Python. 

## Big O notation  (from: https://www.youtube.com/watch?v=5Uqawfl0VHQ)

it is a measure of how much time & space a code takes to perform a task. and how it responds when you increase the amount of data. it is used to compare algorithms. 

it gives you the worst-case scenario. 
