# HTML Lists, Control Flow with JS, and the CSS Box Model

## Reading
[Learn HTML](https://developer.mozilla.org/en-US/docs/Web/HTML)
[Ordered](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/ol) and [Unordered lists](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/ul)

1. When should you use an unordered list in your HTML document?
1. How do you change the bullet style of unordered list items?
1. When should you use an ordered list vs an unorder list in your HTML document?
1. Describe two ways you can change the numbers on list items provided by an ordered list?
   
## HTML Answers
1. You should use an unordered list in HTML when you want to create a list of items that are not in a specific order.
2. You can change the bullet style of unordered list items using CSS. You can use the list-style-type property to specify the type of bullet.
3. You should use an ordered list in HTML when you want to create a list of items that have a specific order.
4. You can use the list-style-type property in CSS to change the style of the numbers, or You can use the start attribute in the ol element to specify where the list should start counting.
[Learn CSS](https://developer.mozilla.org/en-US/docs/Learn/CSS)
[The Box Model](https://developer.mozilla.org/en-US/docs/Learn/CSS/Building_blocks/The_box_model)

1. Describe the CSS properties of margin and padding as characters in a story. What is their role in a story titled: “The Box Model”?
1. List and describe the four parts of an HTML elements box as referred to by the box model.

## CSS Answers
1. In a galaxy far, far away, the epic saga of "The Box Model" unfolded with two iconic characters – Margin and Padding. Margin, representing the elegant side of the Force, was the guardian of personal space in the intergalactic web. With grace and finesse, she ensured that elements in the digital universe maintained their distance, preventing the invasion of one element's territory by another. Margin believed in the importance of a comfortable buffer between objects, understanding that denizens of the galaxy appreciated the freedom to breathe. Her mission was to protect this sacred space, fostering order and harmony among the elements in the cosmic web. Padding, the jovial character, represented the warm and comforting side of the Force. His role was to provide support and cushioning to all digital citizens in the vast galaxy. Be it text, images, or other content, Padding enveloped them in a snug embrace, making sure everything felt cozy and visually appealing. He believed that a touch of extra cushioning added a sense of comfort to the cosmic web, ensuring that every element could thrive. Together, Margin and Padding formed a dynamic duo, creating the perfect framework for intergalactic harmony, a balance between personal space and comfort. In the great epic of web design in the Star Wars universe, they were not just CSS properties but the cosmic architects of a harmonious digital galaxy, proving that even in the vastness of space, balance and aesthetics were vital for a truly epic web design.
2. The four parts of an HTML element's box model are content, padding, border, and margin.
   *  The **Content** is the actual information, text, images, or other media contained within the element.
   *  The **Padding** is a buffer or space between the content and the element's border.
   *  The **Border** outlines the element's content and padding areas, creating a visible boundary for the element.
   *  The **Margin** is crucial for maintaining separation and preventing elements from overlapping.


[Learn JS](https://developer.mozilla.org/en-US/docs/Learn/JavaScript)
[Arrays](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/First_steps/Arrays) [Operators and Expressions](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Expressions_and_Operators) [Conditionals](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Building_blocks/conditionals) [Loops](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Building_blocks/Looping_code)

1. What data types can you store inside of an Array?
2. Is the people array a valid JavaScript array? If so, how can I access the values stored? If not, why?
## Example

       const people = [['pete', 32, 'librarian', null], ['Smith', 40, 'accountant', 'fishing:hiking:rock_climbing'], ['bill', null, 'artist', null]];
3. List five shorthand operators for assignment in javascript and describe what they do.
4. Read the code below and evaluate the last expression and explain what the result would be and why.

        let a = 10;
        let b = 'dog';
        let c = false;
             
         // evaluate this
        (a + c) + b;

## JS Answers
1. Numbers, strings, booleans, objects
2. Yes it is and you can access values in this array using array indexing.
3. += Addition Assignment: Adds the value of variable A to the value of veriable B and assigns the result back to B, -= Subtraction Assignment Subtracts the value of A from the current value of B and assigns the result back to B, *= Multiplication Assignment



      
Describe a real world example of when a conditional statement should be used in a JavaScript program.
Give an example of when a Loop is useful in JavaScript.