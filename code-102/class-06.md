# Dynamic web pages with JavaScript

## **What are variables in JavaScript?**
In JavaScript, variables are used to store and manage data. They are essentially containers that hold values, such as numbers, text, or objects, which can be manipulated, updated, and used in various ways within your code.

## **What does it mean to declare a variable?**
You declare a variable by using either the var, let, or const keywords. eclaring a variable involves specifying its name, which can be used to refer to the stored data, and, in many programming languages, defining the type of data that the variable can hold. 

## **What is an “assignment” operator, and what does it do?**
An "assignment" operator is used in programming to assign a value to a variable. It allows you to store and manipulate data within your program. 

## **What is information received from the user called?**
Information received from the user is called input



## Additional Notes Examples and Definitions 

prompt
The fist one is called prompt. It will show a pop-up window with the text provided as the first parameter and with a textbox the user can fill in. When the user presses OK, the value in the text box will be returned by the prompt() function. Then, in this example we use the document.write method to update the html with the text.

          <script>
 
          var name = prompt("Your name:", "");
          document.write("Hello ", name);
 
          </script>

The textbox will be pre-filled with the content of the second parameter. This can be very useful if we would like to ask the user to edit some value. We can pre-fill the box with the old value.
          <script>
 
          var name = prompt("Please correct your e-mail address:", "foo@bar.co");
          document.write("Your e-mail address is ", name);
 
          </script>

confirm
The other pop-up is not really an input method. It allows the developer to ask a Yes/No question. Calling the confirm() function will show a pop-up window with the provided texts and with two buttons. If the user presses OK the confirm() function will return true, if the user presses cancel or hits the ESC key, the function will return false.
          <script>
 
          if (confirm("Shall I print Hello World?")) {
    document.write("Hello World");
          } else {
    document.write("OK, I won't print it.");
          }
 
          </script>

## Create function

In JavaScript we use the function keyword for this followed by the name of the new function. Then the list of parameters in parentheses and then a block of expressions in curly braces. This is the body of the function.

          <script>
          f          unction show() {
            console.log('Hello World');
          }
 
          console.log('before');
          show();
          console.log('after');
          </script>


          <script>
          function show() {
            console.log('Hello World');
          }
 
          show();
          console.log('before');
          show();
          console.log('after');
          show();
          </script>



## Function with parameters

A much more interesting case is when we also provide parameters to the function. In the next example, in the function declaration we wrote that we are going to accept a single value and we want it to be assigned to the name variable. Then, we called the function and passed a value to it. In every call we passed a different value.

Inside the function the name variable holds the current value.

This show the real power of functions.

We can have one piece of code, that can be tested on it own, separately from the rest of the code, and then reused multiple times.

          <script>
          function show(name) {
            console.log('Hello ', name);
          }
 
          show('Foo');
          show('Bar');
          show('Zorg');
          </script>

What are variables in JavaScript?
**Variables are Containers for Storing Data**
What does it mean to declare a variable?
**JavaScript Variables can be declared in 4 ways:**

* Automatically
* Using var
* Using **let** will allow you to change variable or input variables that change over time
* Using **const** is constant variable does not change



console.log(is a print function for variables);

## 3 Data types

* strings  numbers or names with quotation marks
* numbers  are plain numbers
* boolean  true or false 


alert is a dynamic command 

Promt('quickect way to get user input'); message goes inbetween the parenthesis ()

**declair variable for prompt** 
let userName = prompt('What is your name');
document.write(' Hello userName  ')  document write 