# Understanding the JavaScript Call Stack

. What is a ‘call’?
- The call stack is primarily used for function invocation (call). Since the call stack is single, function(s) execution, is done, one at a time, from top to bottom. It means the call stack is synchronous.

. How many ‘calls’ can happen at once?
- one at a time.

. What does LIFO mean?
- Last In, First Out data structure.

. Draw an example of a call stack and the functions that would need to be invoked to generate that call stack.
- ![](https://cdn-media-1.freecodecamp.org/images/QgR2uIk7tW0YNz0Xm8g0jAPeRFI0e4sCejsv)

. What causes a Stack Overflow?
- A stack overflow occurs when there is a recursive function (a function that calls itself) without an exit point. 



# JavaScript error messages

. What is a ‘refrence error’?
- when you try to use a variable that is not yet declared you get this type os errors.

. What is a ‘syntax error’?
- when you have something that cannot be parsed in terms of syntax, like when you try to parse an invalid object using JSON.parse.

. What is a ‘range error’?
- when trying to pass a value as an argument to a function that does not allow a range that includes the value. 

. What is a ‘tyep error’?
- types of errors show up when the types (number, string and so on) you are trying to use or access are incompatible, like accessing a property in an undefined type of variable.

. What is a breakpoint?
- ![](https://miro.medium.com/max/1400/1*yhFA4njFS7JCRVZPzvDU-A.png)

. What does the word ‘debugger’ do in your code?
- It shows history before reaching the breakpoint.

notes taken from (https://codeburst.io/javascript-error-messages-debugging-d23f84f0ae7c)
(https://www.freecodecamp.org/news/understanding-the-javascript-call-stack-861e41ae61d4)