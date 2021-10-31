# Testing and Modules

## In Tests We Trust - TDD with Python 

Test driven development is the safe way of developing. It makes sure that everything is working well WHILE developing, instead of finishing the code and THEN looking for bugs in the big code you have. 
The technique for building the test is: 

•	Arrange: you need to organize the data needed to execute that piece of code (input);

•	Act: here you will execute the code being tested (exercise the behavior);

•	Assert: after executing the code, you will check if the result (output) is the same as you were expecting.

Now according to this article, it is better to write the test BEFORE the actual code! 

This is the process: 

🆘 Write a unit test and make it fail (it needs to fail because the feature isn’t there, right? If this test passes, call the Ghostbusters, really)

✅ Write the feature and make the test pass! (you can dance after that)

🔵 Refactor the code — the first version doesn’t need to be the beautiful one (don’t be shy)


And finally, remember to do the tests in baby steps.


## If __name__ equals __main__

__name__ is a global variable python defines before executing the code. If the code is being executed by a different file (because this one is just imported as a module) then the name will be equal to the file that is originally being called to run. 

This property of python has advantages: 

1.	Every Python module has it’s __name__ defined and if this is ‘__main__’, it implies that the module is being run standalone by the user and we can do corresponding appropriate actions.
2.	If you import this script as a module in another script, the __name__ is set to the name of the script/module.
3.	Python files can act as either reusable modules, or as standalone programs.
4.	if __name__ == “main”: is used to execute some code only if the file was run directly, and not imported.

## recursion video

Recursion is dependence of one operation on itself but with a different (or same) value. When implemented in programing it causes a stack. it seems to give the processer a hard time! 
