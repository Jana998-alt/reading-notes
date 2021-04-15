# Read: 10 - JS Debugging

Debugging is solving problems that you created yourself while writing a code! Which can cause a big headache since you are already solving a bigger problem. But its ok, there is nothing perfect in life.
To find the problem, you really need to understand how JavaScript (or the language that you are using) works. 
You need to know: 
+ the order of execution
+ the scopes (in our case Global and functions scopes)
 _ note: if you don’t use the keyword *var* for declaring a variable, it will be a global scope_ 
+ how JS stacks tasks. Basically, it prioritizes the tasks that other tasks depend on, and leave the latter ones waiting until they get what they want. 


Some of the debugging is not completely of the problems from your side, rather from external sources. Therefore, there must be a checking process all around your code to make sure that everything you expect is actually working well. 

A nice advice from the book:

 _”If the problem is hard to find, it is easy to lose track of what you have and have not tested. Therefore, when you start debugging, keep notes of what you have tested and what the result was. No matter how stressful the circumstances are, if you can, stay calm and methodical, the problem will feel less overwhelming and you will solve it faster”_

I think I will need it in the future.

Finally, each browser has its own way of help in debugging. 
