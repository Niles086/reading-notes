# Operators and Loops

## Expressions in Java Script

* In JavaScript, an expression is a piece of code that produces a value.

## Why we use Loops

* Loops are used for a variety of purposes. They allow you to execute a block of code multiple times, and they can make your code more efficient, easier to understand, and maintain. They can be very useful when you need to repeat a process without duplicating code. Loops also work very well with conditional statements to perform actions based on certain conditions.

## For Loop Execution

* A for loop in JavaScript stops executing when the condition specified in the loop's declaration becomes _**false.**_ Its **IMPORTANT** to be careful when working with these to prevent infinite loops, which can crash your program or browser.

## While Loop Execution

* The number of times a while loop will execute depends on the condition set in the loops code. A while loop continues to execute its code block as long as the conditions are true. When the condition becomes false, the loop stops.

## Additional notes and code examples

### Assignment operators

* _An assignment operator assigns a value to its **left operand** based on the value of its **right operand**._ The simple assignment operator is **equal (=), which assigns the value of its right operand to its left operand**. That is, **x = f()** is an assignment expression that **assigns the value of f() to x.**

* There are also **compound assignment operators** that are shorthand for the operations listed in the following table:

| **Name**                       | **Shorthand Operator** | **Meaning** |
|----------------------------|--------------------|---------------------|
| Assignment                  | `x = f()`          | `x = f()`          |
| Addition Assignment         | `x += f()`         | `x = x + f()`      |
| Subtraction Assignment      | `x -= f()`         | `x = x - f()`      |
| Multiplication Assignment   | `x *= f()`         | `x = x * f()`      |
| Division Assignment         | `x /= f()`         | `x = x / f()`      |
| Remainder Assignment        | `x %= f()`         | `x = x % f()`      |
| Exponentiation Assignment   | `x **= f()`        | `x = x ** f()`     |
| Left Shift Assignment       | `x <<= f()`        | `x = x << f()`     |
| Right Shift Assignment      | `x >>= f()`        | `x = x >> f()`     |
| Unsigned Right Shift Assignment | `x >>>= f()`    | `x = x >>> f()`   |
| Bitwise AND Assignment      | `x &= f()`         | `x = x & f()`      |
| Bitwise XOR Assignment      | `x ^= f()`         | `x = x ^ f()`      |
| Logical AND Assignment      | `x &&= f()`        | `x && (x = f())`   |
| Nullish Coalescing Assignment | `x ??= f()`      | `x ?? (x = f())`   |

### The last two are

             | Logical OR Assignment       | `x ||= f()`        | `x || (x = f())`   |
             | Bitwise OR Assignment       | "x |= f()"         | `x = x | f()`      |

## Assigning to properties

* If an expression evaluates to an object, then the left-hand side of an assignment expression may make assignments to properties of that expression. For example:

              const obj = {};
              
              obj.x = 3;
              console.log(obj.x); // Prints 3.
              console.log(obj); // Prints { x: 3 }.
              
              const key = "y";
              obj[key] = 5;
              console.log(obj[key]); // Prints 5.
              console.log(obj); // Prints { x: 3, y: 5 }.

## Destructuring

For more complex assignments, the destructuring assignment syntax is a JavaScript expression that makes it possible to extract data from arrays or objects using a syntax that mirrors the construction of array and object literals.

Without destructuring, it takes multiple statements to extract values from arrays and objects:

              const foo = ["one", "two", "three"];
              
              const one = foo[0];
              const two = foo[1];
              const three = foo[2];

## Evaluation and nesting

* In general, assignments are used within a variable declaration (i.e., with const, let, or var) or as standalone statements).


_This Declares a variable x and initializes it to the result of f()_
_The result of the x = f() assignment expression is discarded.

  let x = f();

x = g(); This part Reassigns the variable x to the result of g()_

However, like other expressions, assignment expressions like x = f() evaluate into a result value. Although this result value is usually not used, it can then be used by another expression.

Chaining assignments or nesting assignments in other expressions can result in surprising behavior. For this reason, some JavaScript style guides discourage chaining or nesting assignments). Nevertheless, assignment chaining and nesting may occur sometimes, so it is important to be able to understand how they work.

By chaining or nesting an assignment expression, its result can itself be assigned to another variable. It can be logged, it can be put inside an array literal or function call, and so on.

let x;
const y = (x = f()); // Or equivalently: const y = x = f();
console.log(y); // Logs the return value of the assignment x = f().

console.log(x = f()); // Logs the return value directly.

// An assignment expression can be nested in any place
// where expressions are generally allowed,
// such as array literals' elements or as function calls' arguments.
console.log([0, x = f(), 0]);
console.log(f(0, x = f(), 0));



## Comparison operators

A comparison operator compares its operands and returns a logical value based on whether the comparison is true. The operands can be numerical, string, logical, or object values. Strings are compared based on standard lexicographical ordering, using Unicode values. In most cases, if the two operands are not of the same type, JavaScript attempts to convert them to an appropriate type for the comparison. This behavior generally results in comparing the operands numerically. The sole exceptions to type conversion within comparisons involve the === and !== operators, which perform strict equality and inequality comparisons. These operators do not attempt to convert the operands to compatible types before checking equality. The following table describes the comparison operators in terms of this sample code:


            const var1 = 3;
            const var2 = 4;


**Comparison operators Examples**

| Operator              | Description                                                  | Examples returning true |
|-----------------------|--------------------------------------------------------------|------------------------|
| Equal (==)            | Returns true if the operands are equal.                     | 3 == var1              |
|                       |                                                              | "3" == var1            |
|                       |                                                              | 3 == '3'               |
| Not equal (!=)        | Returns true if the operands are not equal.                 | var1 != 4              |
|                       |                                                              | var2 != "3"            |
| Strict equal (===)    | Returns true if the operands are equal and of the same type.| 3 === var1             |
|                       |                                                              |                        |
| Strict not equal (!==)| Returns true if the operands are of the same type but not equal, or are of different type.| var1 !== "3" |
|                       |                                                              | 3 !== '3'              |
| Greater than (>)      | Returns true if the left operand is greater than the right operand. | var2 > var1     |
|                       |                                                              | "12" > 2              |
| Greater than or equal (>=)| Returns true if the left operand is greater than or equal to the right operand. | var2 >= var1 |
|                       |                                                              | var1 >= 3              |
| Less than (<)         | Returns true if the left operand is less than the right operand. | var1 < var2     |
|                       |                                                              | "2" < 12              |
| Less than or equal (<=)| Returns true if the left operand is less than or equal to the right operand. | var1 <= var2 |
|                       |                                                              | var2 <= 5              |


## Deffinition of a for loop statement

_A for loop repeats until a specified condition evaluates to false. The JavaScript for loop is similar to the Java and C for loop._

A for loop statement structure looks as follows: Pay attention to the terms used in each part!!!

for (initialization; condition; afterthought)
  statement
  



## Deffinition of a for loop statement

_A while statement executes its statements as long as a specified condition evaluates to true._ 

_A while loop statement structure looks as follows:_


while (condition)
  statement
 
* If the condition becomes false, statement within the loop stops executing and control passes to the statement following the loop.
* The condition test occurs before statement in the loop is executed. If the condition returns true, statement is executed and the condition is tested again. If the condition returns false, execution stops, and control is passed to the statement following while.

To execute multiple statements, use a block statement ({ }) to group those statements.

**Example** 
The following while loop iterates as long as n is less than 3:



let n = 0;
let x = 0;
while (n < 3) {
  n++;
  x += n;
}
*Loops offer a quick and easy way to do something repeatedly.*
*Tto increment a loop exampl*

let response = prompt(message);
for(let i = 0; i < 5; i++){
   console.log(i);
}
++ 

**The ++ ant the end is used to increase i by 1 every time it loops**
