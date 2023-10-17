#  Programming with JavaScript

## **Control Flow**

 _Control flow refers to the order in which the statements of a program are executed. It determines the path that the program follows from one statement to the next, based on conditions and control structures._

## **Java Script Function**

_In JavaScript, a function is a reusable block of code that performs a specific task or a set of tasks. Functions are one of the fundamental building blocks of JavaScript and are used to encapsulate a piece of code so that it can be executed multiple times, often with different inputs. Functions help improve code organization, reusability, and maintainability._

## **Calling a function**

_Calling a function means to execute or run the code that the function contains. When you invoke a function in JavaScript, the program transfers control to that function's code block, and the statements within the function are executed. This allows you to use the functionality provided by the function to perform specific tasks._

## **What are the parenthesis for when you define a function?**

_In JavaScript, the parentheses in a function definition serve two purposes. The first is to define a list of parameters or input values that the function can accept. The second is declaring the function, the parentheses identify the code as a function and the parameter list is placed inside them. Without the parentheses, the JavaScript will not recognize the code as a function._

Additional notes and code

**Control flow**
The control flow is the order in which the computer executes statements in a script. 

Code is run in order from the first line in the file to the last line, unless the computer runs across the (extremely frequent) structures that change the control flow, such as conditionals and loops.

For example, imagine a script used to validate user data from a webpage form. The script submits validated data, but if the user, say, leaves a required field empty, the script prompts them to fill it in. To do this, the script uses a conditional structure or if...else, so that different code executes depending on whether the form is complete or not:



            if (isEmpty(field)) {
              promptUser();
            } else {
              submitForm();
            }

## JavaScript Function Syntax

A JavaScript function is defined with the function keyword, followed by a name, followed by parentheses () 

Function names can contain letters, digits, underscores, and dollar signs (same rules as variables).

The parentheses may include parameter names separated by commas:
(parameter1, parameter2, ...)

The code to be executed, by the function, is placed inside curly brackets: {}

function name(parameter1, parameter2, parameter3) {
  // code to be executed
}

Function parameters are listed inside the parentheses () in the function definition.

Function arguments are the values received by the function when it is invoked.

Inside the function, the arguments (the parameters) behave as local variables.


## Function Invocation

The code inside the function will execute when "something" invokes (calls) the function:

* When an event occurs (when a user clicks a button)

* When it is invoked (called) from JavaScript code

* Automatically (self invoked)

## Function Return

* When JavaScript reaches a return statement, the function will stop executing.

* If the function was invoked from a statement, JavaScript will "return" to execute the code after the invoking statement.

Functions often compute a return value. The return value is "returned" back to the "caller":

**Example**
**Calculate the product of two numbers, and return the result:**

_Function is called, the return value will end up in x_
let x = myFunction(4, 3);

function myFunction(a, b) {

_Function returns the product of a and b_
  return a * b;
}


## The () Operator
**The () operator invokes (calls) the function:**

**Example**
_Convert Fahrenheit to Celsius:_

function toCelsius(fahrenheit) {
  return (5/9) * (fahrenheit-32);
}

let value = toCelsius(77);

## Accessing a function with incorrect parameters can return an incorrect answer:

**Example**
function toCelsius(fahrenheit) {
  return (5/9) * (fahrenheit-32);
}

let value = toCelsius();

## Accessing a function without () returns the function and not the function result:

**Example**
function toCelsius(fahrenheit) {
  return (5/9) * (fahrenheit-32);
}

let value = toCelsius;

## Functions Used as Variable Values

**Functions can be used the same way as you use variables, in all types of formulas, assignments, and calculations.**

**Example**
Instead of using a variable to store the return value of a function:

let x = toCelsius(77);
let text = "The temperature is " + x + " Celsius";
**You can use the function directly, as a variable value:**

let text = "The temperature is " + toCelsius(77) + " Celsius";

## Local Variables

Variables declared within a JavaScript function, become LOCAL to the function.

Local variables can only be accessed from within the function.

**Example**
**code here can NOT use carName**

function myFunction() {
  let carName = "Volvo";
  // code here CAN use carName
}

// code here can NOT use carName
Since local variables are only recognized inside their functions, variables with the same name can be used in different functions.

Local variables are created when a function starts, and deleted when the function is completed.

## JavaScript Operators

The Addition Operator + adds numbers:

The Assignment Operator = assigns a value to a variable.

**Operators**
**JavaScript Assignment**

The Assignment Operator (=) assigns a value to a variable:

_Assignment Examples_

     let x = 10;
     // Assign the value 5 to x
     let x = 5;
     // Assign the value 2 to y
     let y = 2;
     /     / Assign the value x + y to z:
     let z = x + y;

## JavaScript Addition

The Addition Operator (+) adds numbers:

Adding
     let x = 5;
     let y = 2;
     let z = x + y;

## JavaScript Multiplication

The Multiplication Operator (*) multiplies numbers:

Multiplying
     let x = 5;
     let y = 2;
     let z = x * y;

Types of JavaScript Operators
There are different types of JavaScript operators:

Arithmetic Operators
Assignment Operators
Comparison Operators
String Operators
Logical Operators
Bitwise Operators
Ternary Operators
Type Operators
JavaScript Arithmetic Operators
Arithmetic Operators are used to perform arithmetic on numbers:

## Arithmetic Operators Example

     let a = 3;
     let x = (100 + 50) * a;

## Operator	Description

     +	Addition
     -     	Subtraction
     *	Multiplication
     **	Exponentiation (ES2016)
     /	Division
     %	Modulus (Division Remainder)
     ++	Increment
     --	Decrementgit 