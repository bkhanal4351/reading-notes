## In Tests We Trust - TDD with Python

Unit Test and TDD
- Unit tests are some pieces of code to exercise the input, the output and the behaviour of your code. You can write them anytime you want.

Important aspects about the unit test
- There are some details to pay attention. The first one is the test name. The tests can be considered as your alive documentation. We need to be descriptive about it and to say what is expected and what we are testing.

- Other thing to care about is the structure. A convention widely used is the AAA: Arrange, Act and Assert.
Arrange: you need to organize the data needed to execute that piece of code (input);
Act: here you will execute the code being tested (exercise the behaviour);
Assert: after executing the code, you will check if the result (output) is the same as you were expecting.

The Cycle
The cycle is made by three steps:
🆘 Write a unit test and make it fail (it needs to fail because the feature isn’t there, right? 
✅ Write the feature and make the test pass! 
🔵 Refactor the code 

![](https://miro.medium.com/max/1400/1*gxEKnrQuS7CO3hONTD7_hg.png)


## If name equals main

Before executing code, Python interpreter reads source file and define few special variables/global variables. 
If the python interpreter is running that module (the source file) as the main program, it sets the special __name__ variable to have a value “__main__”. If this file is being imported from another module, __name__ will be set to the module’s name. Module’s name is available as value to __name__ global variable. 

A module is a file containing Python definitions and statements. The file name is the module name with the suffix .py appended. 

When we execute file as command to the python interpreter, 

`python script.py`

` # Python program to execute
# main directly
print ("Always executed")
 
if __name__ == "__main__":
    print ("Executed when invoked directly")
else:
    print ("Executed when imported")`



  ## Recursion

  What is Recursion? 
The process in which a function calls itself directly or indirectly is called recursion and the corresponding function is called as recursive function. Using recursive algorithm, certain problems can be solved quite easily.




Notes Taken from (https://code.likeagirl.io/in-tests-we-trust-tdd-with-python-af69f47e6932)
(https://www.geeksforgeeks.org/what-does-the-if-__name__-__main__-do/)
(https://www.geeksforgeeks.org/recursion/)
