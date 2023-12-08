# In memory storage
Below you will find some reading material, code samples, and some additional resources that support the topic for this class and the upcoming lecture.

Review the Submission Instructions for guidance on completing and submitting this assignment.

Reading
[Understanding the JavaScript Call Stack](https://medium.freecodecamp.org/understanding-the-javascript-call-stack-861e41ae61d4)

1. What is a ‘call’?
   In the context of programming and the call stack, a 'call' refers to the invocation or execution of a function. When a function is called, it gets added to the call stack, and its execution begins.
2. How many ‘calls’ can happen at once?
   In a single-threaded JavaScript environment with a single call stack, only one function call can happen at a time. The call stack processes function calls in a synchronous manner, executing them one after another.
3. What does LIFO mean?
   LIFO stands for Last In, First Out. It's a principle used in data structures, and in the context of the call stack, it means that the last function added to the stack is the first one to be executed and removed. The call stack follows the LIFO order in managing function invocations.
4. Draw an example of a call stack and the functions that would need to be invoked to generate that call stack.
                        |  thirdFunction()  |
                        |  secondFunction() |
                        |  firstFunction()  |
                        |____________________|

                        function firstFunction(){
                        throw new Error('Stack Trace Error');
                        }

                        function secondFunction(){
                        firstFunction();
                        }

                        function thirdFunction(){
                        secondFunction();
                        }

                        thirdFunction();
                                            

5. What causes a Stack Overflow?
   A stack overflow occurs when there is a recursive function (a function that calls itself) without an exit point. In other words, the function keeps calling itself, and each call adds a new stack frame to the call stack. Eventually, the stack reaches its maximum capacity, leading to a "Maximum call size exceeded" error.

## [JavaScript error messages](https://codeburst.io/javascript-error-messages-debugging-d23f84f0ae7c)

1. What is a ‘reference error’?
   A 'reference error' occurs when you try to use a variable that has not been declared. 
2. What is a ‘syntax error’?
   A 'syntax error' occurs when there is a mistake in the structure of your code that prevents it from being parsed correctly.
3. What is a ‘range error’?
   A 'range error' occurs when you manipulate an object with some kind of length and give it an invalid length.
4. What is a ‘type error’?
   A 'type error' occurs when there is an attempt to use or access incompatible types, such as accessing a property in an undefined variable.
5. What is a breakpoint?
   A 'breakpoint' is a specified point in your code where the debugger should pause execution, allowing you to inspect the current state of your program and analyze variables, expressions, and the call stack.
6. What does the word ‘debugger’ do in your code?
   The term 'debugger' refers to a tool or functionality used to identify and fix errors (bugs) in your code. In the provided context, it seems to be referring to the usage of debugger statements in the code. When the JavaScript interpreter encounters a debugger statement, it pauses execution, allowing developers to inspect the code, variables, and the call stack at that point. This aids in the debugging process by providing a way to interactively analyze the program's state.

## Bookmark and Review
JavaScript errors reference on MDN

## Things I want to know more about