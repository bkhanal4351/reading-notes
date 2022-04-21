## Classes and Objects

Objects are an encapsulation of variables and functions into a single entity. Objects get their variables and functions from classes. Classes are essentially a template to create your objects.

An example code:

```class MyClass:
    variable = "blah"

    def function(self):
        print("This is a message inside the class.")```

How to access Object Variables

To access the variable inside of the newly created object "myobjectx" you would do the following:

```class MyClass:
    variable = "blah"

    def function(self):
        print("This is a message inside the class.")

myobjectx = MyClass()

myobjectx.variable```

Accessing object functions:

To access a function inside of an object you use notation similar to accessing a variable:

```class MyClass:
    variable = "blah"

    def function(self):
        print("This is a message inside the class.")

myobjectx = MyClass()

myobjectx.function()```

## Thinking Recursively in Python

Recursive Functions in Python

Recursive function for calculating n! implemented in Python:

```def factorial_recursive(n):
    # Base case: 1! = 1
    if n == 1:
        return 1

    # Recursive case: n! = n * (n-1)!
    else:``
        return n * factorial_recursive(n-1)```

    Behind the scenes, each recursive call adds a stack frame (containing its execution context) to the call stack until we reach the base case. 

  

    Maintaining state

    When dealing with recursive functions, keep in mind that each recursive call has its own execution context, so to maintain state during recursion you have to either:

Thread the state through each recursive call so that the current state is part of the current call’s execution context
Keep the state in global scope
`def sum_recursive(current_number, accumulated_sum):
    # Base case
    # Return the final state
    if current_number == 11:
        return accumulated_sum

    # Recursive case
    # Thread the state through the recursive call
    else:
        return sum_recursive(current_number + 1, accumulated_sum + current_number)`

       

       Here’s how you maintain the state by keeping it in global scope:

       ```# Global mutable state
current_number = 1
accumulated_sum = 0


def sum_recursive():
    global current_number
    global accumulated_sum
    # Base case
    if current_number == 11:
        return accumulated_sum
    # Recursive case
    else:
        accumulated_sum = accumulated_sum + current_number
        current_number = current_number + 1
        return sum_recursive()```



  Recursive Data Structures in Python

  A data structure is recursive if it can be deﬁned in terms of a smaller version of itself. A list is an example of a recursive data structure. Let me demonstrate. Assume that you have only an empty list at your disposal, and the only operation you can perform on it is this:

   Return a new list that is the result of
 adding element to the head (i.e. front) of input_list

```def attach_head(element, input_list):
    return [element] + input_list```

Using the empty list and the attach_head operation, you can generate any list. For example, let’s generate [1, 46, -31, "hello"]:

```attach_head(1,                                                  # Will return [1, 46, -31, "hello"]
            attach_head(46,                                     # Will return [46, -31, "hello"]
                        attach_head(-31,                        # Will return [-31, "hello"]
                                    attach_head("hello", [])))) # Will return ["hello"]```




Notes taken from (https://www.learnpython.org/en/Classes_and_Objects)
(https://realpython.com/python-thinking-recursively/)


