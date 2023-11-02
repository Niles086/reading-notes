# Forms and JS Events


## [HTML Forms](https://developer.mozilla.org/en-US/docs/Learn/Forms)
## [Your first Web Form.](https://developer.mozilla.org/en-US/docs/Learn/Forms/Your_first_form) 
## [How To Structure A Web Form.](https://developer.mozilla.org/en-US/docs/Learn/Forms/How_to_structure_a_web_form)

1. Why are forms so important in web development?
   * Forms allow users to interact with a website by inputting various types of data, such as text, numbers, checkboxes, radio buttons, and more. This user input is crucial for various web applications, like search engines, login pages, registration forms, and e-commerce sites.
   * Forms enable users to engage with a website by submitting data, making choices, and providing feedback. This interaction enhances user engagement and makes the website more dynamic and interactive.
   
2. When designing a form, what are some key things to keep in mind when it comes to user experience?
   * When designing forms for a website, prioritize user experience by keeping them simple, clear, and consistent in layout and style. Provide helpful cues, validation, and guidance to assist users, and ensure accessibility for all. Test and iterate your design based on real user feedback to continually improve the form's usability and performance.

3. List 5 form elements and explain their importance.
   * Text input fields are crucial for collecting user information like names, email addresses, and messages.
   * Checkboxes are used for selecting multiple items from a list of options. They play a vital role in scenarios where users can make multiple choices, like selecting products for purchase.
   * Dropdown menus are valuable for presenting a list of options in a compact format. 
   * Radio buttons offer users a way to select a single option from a predefined list.
   * Textareas serve as input fields for longer text entries, including comments, messages, and detailed descriptions. 


## [Learn JS](https://developer.mozilla.org/en-US/docs/Learn/JavaScript)
## [Introduction To Events.](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Building_blocks/Events)

1. How would you describe events to a non-technical friend?
   * Imagine events in JavaScript like actions or occurrences that happen on a web page when you interact with it. These interactions could be things like clicking a button, moving your mouse over an image, or pressing a key on your keyboard. Events are like triggers that make something happen on a website. 
  
2. When using the addEventListener() method, what 2 arguments will you need to provide?
   * The event type this is a string that specifies the type of event you want to listen for. It could be something like "click," "mouseover," "keydown," or any other event type you want to handle.
   * The event handler function: This is a JavaScript function that will be executed when the specified event occurs. It's the code that you want to run in response to the event. This function will be automatically called when the event is triggered.
  
3. Describe the event object. Why is the target within the event object useful?
   * The event object in JavaScript is automatically created and passed to an event handler function when an event occurs, such as a mouse click, keyboard press, or other user interactions. The event.target property represents the DOM element that triggered the event. It is particularly useful because it allows you to identify the specific element on which the event occurred. This is useful when you have multiple elements of the same type, or when elements are created dynamically and not present in the DOM when the page loads, event.target helps identify the newly added elements that triggered the event. 
  
4. What is the difference between event bubbling and event capturing?
   * Event bubbling and event capturing are two different phases in the event propagation process in the Document Object Model (DOM) of web browsers. They describe the order in which events are handled when an event occurs on an element and propagates through the DOM tree. The key difference between them lies in the direction of propagation:
   * Event Bubbling:
   * Event bubbling is the default behavior in most browsers.
   * When an event occurs on an element, it first triggers the event on the target element. Then, the event bubbles up through the DOM hierarchy, from the target element to its parent elements, and so on, up to the root of the document (the html element).
   * Event listeners registered on parent elements can catch the event during the bubbling phase, potentially leading to multiple elements responding to the same event.
   * Event Capturing:
   * Event capturing is less commonly used and is an optional phase in event propagation.
   * In event capturing, the event is first triggered at the root of the document (the html element) and then propagates down through the DOM hierarchy to the target element.
   * Event listeners registered on parent elements can catch the event during the capturing 

## Bookmark and Review

## [HTML5 Input Types](https://developer.mozilla.org/en-US/docs/Learn/Forms/HTML5_input_types)

## [Event Reference and listings(https://developer.mozilla.org/en-US/docs/Web/Events)]