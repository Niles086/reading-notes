Read: Class 09
Functional Programming: Functional programming is a programming paradigm that treats computation as the evaluation of mathematical functions and avoids changing state and mutable data. It emphasizes the use of pure functions, immutability, and declarative expressions.

Pure Function: A pure function is a function that, given the same input, will always return the same output and has no observable side effects. In other words:

Deterministic: The output is solely determined by its input.
No Side Effects: It does not modify variables outside its scope, and it does not have any observable effects other than returning a value.
How to Identify a Pure Function:

No Side Effects: It should not modify external state or variables.
Deterministic: Given the same inputs, it always produces the same output.
No I/O Operations: It does not perform I/O operations, such as reading from files or user input.
Benefits of Pure Functions:

Predictability: Easier to reason about and predict behavior.
Testability: Easier to test since they have no side effects.
Concurrency: Safer for concurrent execution due to lack of shared mutable state.
Memoization: Enables memoization for performance optimization.
Immutability: Immutability is the concept of making variables and data structures unchangeable or unable to be modified after their creation. In functional programming, immutability is favored to avoid unintended side effects and to make programs more predictable.

Referential Transparency: Referential transparency is a property of pure functions. It means that a function call can be replaced with its resulting value without changing the program's behavior. This property allows for substitution of expressions with their values, aiding in reasoning about and optimizing code.

 

A module in programming refers to a self-contained unit of code that encapsulates related functionality. Modules help in organizing code into separate files or components, making the codebase more modular, maintainable, and scalable.

require: In contexts like Node.js (CommonJS), require is a keyword used to include and use modules in JavaScript. It is used to import functionality from other modules into the current module. The require statement loads the specified module and returns the exported functionality, making it available for use in the current module.

Bringing Another Module: To bring another module into the file you are working in, you use the require statement followed by the path to the module.

 

Making a Module Available: To make a module available for use in other files, you need to export the functionality you want to expose. In Node.js (CommonJS), you typically use module.exports or exports to define what gets exported from a module.