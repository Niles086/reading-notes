# Problem Domain, Objects, and the DOM

## Reading

[JavaScript Object Basics](https://canvas.instructure.com/courses/7890511/discussion_topics/19821041)

1. How would you describe an object to a non-technical friend you grew up with
2. What are some advantages to creating object literals?
3. How do objects differ from arrays?
4. Give an example for when you would need to use bracket notation to access an object’s property instead of dot notation
5. Evaluate the code below. What does the term this refer to and what is the advantage to using this?

                const dog = {
                  name: 'Spot',
                  age: 2,
                  color: 'white with black spots',
                  humanAge: function (){
                    console.log(`${this.name} is ${this.age*7} in human years`);
                  }
                }

## Answers Section 1
1. Think of JavaScript objects as digital boxes that help us store and manage all sorts of information in a structured way. It's like having a magic box that can hold all kinds of data!
2. Object literals are a straightforward way to create objects without the need for a constructor function or class, they  are often faster to create than using constructor functions or classes, which can be beneficial for performance-critical applications.
3. Objects are used for structured data with named properties, while arrays are used for ordered lists of values.
4. You would typically use bracket notation to access an object's property when the property name is dynamic or not known in advance, or the property name contains special characters or spaces.
5.  The term this refers to the object that the method humanAge is called on, which is the dog object. The advantage of using this in this way is that it allows you to access and work with the properties of the current object. In this case, it lets you access the name and age properties of the dog object
[Introduction To The DOM](https://developer.mozilla.org/en-US/docs/Web/API/Document_Object_Model/Introduction)

1. What is the DOM?
2. Briefly describe the relationship between the DOM and JavaScript

## Answers Section 2



