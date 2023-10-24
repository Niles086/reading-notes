# Class 01 Notes

## Opening Statement

Understanding how to add JavaScript to an HTML document is a fundamental skill with significant implications for various aspects of web development and design. This topic matters because it lays the foundation for creating dynamic and interactive web experiences.

**Reading**
[Skim How the Web Works.](https://developer.mozilla.org/en-US/docs/Learn/Getting_started_with_the_web/How_the_Web_works)
[Skim Website Design and Process.](https://developer.mozilla.org/en-US/docs/Learn/Getting_started_with_the_web/What_will_your_website_look_like)

## Getting Started Questions

1. Compose a short poem describing how HTTP sends data between computers.
1. Describe how HTML, CSS, and JS files are “parsed” in the browser.
1. How can you find images to add to a Website?
1. How do you create a String vs a Number in JavaScript?
1. What is a Variable and why are they important in JavaScript?

## Getting Started Answers

1. HTTP, just let it be, the silent stream we ride, Amazon's heart, its digital soul, in this vast online tide. In commerce's dance, it's a prime melody to see, Relies on HTTP, connecting you and me. As we browse and shop, with clicks and keys we steer, Through digital aisles, the treasures we hold dear. The browser sends its plea to the server's abode, A message in the ether, across the online road. A request, a whisper, sent with a simple plea, Send me the website, let me see what's to be. Through the vast web, like a river swift and free, Thanks to HTTP, the bridge between you and me.
1. The browser parses the HTML file first, and that leads to the browser to discovering any _Link_ elements pointing to any external CSS _stylesheets_, and any _script_ **element** pointing to scripts. As the browser parses the HTML it send request back to the server for any CSS files it has found from link elements or JavaScript files from script elements, and  from that it parses the CSS and JavaScript.
1. To avoid violating copyright laws, you can use Google's license filter. Click on the Tools button, then on the resulting Usage rights option that appears below. You should choose the option Creative Commons licenses.
1. To create a string enclose the value n single or double quote marks. Example let num = "10"; Numbers are different in that they dont have quote marks. Example let num = 10;
1. Variables are containers that store values. The are important because those stored values can be used later for different functions. It also makes your code cleaner and allows you to execute more dynamic functions.

## Introduction to HTML Questions

1. What is an HTML attribute?
1. Describe the Anatomy of an HTMl element.
1. What is the Difference between article and section element tags?
1. What Elements does a “typical” website include?
1. How does metadata influence Search Engine Optimization?
1. How is the meta HTML tag used when specifying metadata?

## Introduction to HTML Answers

1. An HTML attribute is like a little tag or label that we put on an HTML element. These tags are used to modify or even provide more detail about the element.
1. An HTML elements structure can be broken down into four basic parts. The **Opening** **Tag** this is the first part of an HTML element, **Attributes** attributes provide extra details about the element and are placed inside the opening tag, **Content** the content of the element goes between the opening and closing tags. It's the actual information you want to display on your web page, and the **Closing** **Tag** this is the last part of an HTML element. It's similar to the opening tag but includes a forward slash before the element name.
1. The **Article** element is used to mark up a self-contained, piece of content that can be distributed and understood independently, and the **Section** element is used to group related content within a document.
1. A typical wedsite encludes some of the following elements: Headings like h1 and h2, paragraphs or p tags, links, images, and list are just a few.
1. By using relevant keywords in metadata and accurate descriptions, you can improve your website's visibility in search engine rankings.
1. The **Meta** HTML tag provides information about the document or controls aspects of how the document should be displayed or processed. It's usually placed within the head section of the HTML document. The **meta** tag uses attributes to define different types of metadata.

## Miscellaneous Questions

1. What is the first step to designing a Website?
1. What is the most important question to answer when designing a Website?

## Miscellaneous Answers

1. The 1st step in designing a website is to organize your thoughts on paper. Before you deal with anything technical you need to deside the what and how. What you want your site to be about and how you want to present it. From there you can begin with a wire frame.
1. The most important question to answer when designing a Website, is What do you want to acomplish?

## Semantics Questions

1. Why should you use an h1 element over a span element to display a top level heading?
1. What are the benefits of using semantic tags in our HTML?

## Semantics Answers

1. By using you provide clear and meaningful structure to your content, making it easier for both humans and search engines to understand the Structure and importance of your headings.
1. The use of semantic HTML tags is essential for creating accessible, search engine-friendly, and maintainable web content.

## What is JavaScript? Questions

1. Describe 2 things that require JavaScript in the Browser?
1. How can you add JavaScript to an HTML document?

## What is JavaScript? Answers

1. JavaScript can be used to perform client-side form validation, and is used to create dynamic and interactive features on web pages like dropdown menus.
1. You can include JavaScript directly within the HTML document using the **script** element. You can also include the code from an external JavaScript file by creating a **script** element that points to the file.

## Things I want to know more about
