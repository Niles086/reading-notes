# Design web pages with CSS

What is the purpose of CSS? Using CSS, you can control exactly how HTML elements look in the browser, presenting your markup using whatever design you like. CSS is a language for specifying how documents are presented to users — how they are styled, laid out, etc. CSS can be used for very basic document text styling — for example, for changing the color and size of headings and links. It can be used to create a layout — for example, turning a single column of text into a layout with a main content area and a sidebar for related information. It can even be used for effects such as animation.

What are the three ways to insert CSS into your project?

External CSS With an external style sheet, you can change the look of an entire website by changing just one file!
Each HTML page must include a reference to the external style sheet file inside the <link> element, inside the head section. An external style sheet can be written in any text editor, and must be saved with a .css extension.
The external .css file should not contain any HTML tags.
<!DOCTYPE html>
<html>
<head>
<link rel="stylesheet" href="mystyle.css">
</head>
<body>

<h1>This is a heading</h1>
<p>This is a paragraph.</p>

</body>
</html>

Internal CSS An internal style sheet may be used if one single HTML page has a unique style.
The internal style is defined inside the <style> element, inside the head section.
<!DOCTYPE html>
<html>
<head>
<style>
body {
  background-color: linen;
}

h1 {
  color: maroon;
  margin-left: 40px;
}
</style>
</head>
<body>

<h1>This is a heading</h1>
<p>This is a paragraph.</p>

</body>
</html>

Inline CSS An inline style may be used to apply a unique style for a single element.
To use inline styles, add the style attribute to the relevant element. The style attribute can contain any CSS property.
<!DOCTYPE html>
<html>
<body>

<h1 style="color:blue;text-align:center;">This is a heading</h1>
<p style="color:red;">This is a paragraph.</p>

</body>
</html>

Write an example of a CSS rule that would give all <p> elements red text.
<p> {
  color: red;
  }



Comment command is controle /

* is global element

# for  ID 

. for classes


If some properties have been defined for the same selector (element) in different style sheets, the value from the last read style sheet will be used. 

Example of CSS rule to make heading red
h1 {
  color: red;
  font-size: 5em;
}

In the above example, the CSS rule opens with a selector. This selects the HTML element that we are going to style. In this case, we are styling level one headings (h1).
We then have a set of curly braces { }.
Inside the braces will be one or more declarations, which take the form of property and value pairs. We specify the property (color in the above example) before the colon, and we specify the value of the property after the colon (red in this example).
This example contains two declarations, one for color and the other for font-size. Each pair specifies a property of the element(s) we are selecting (h1 in this case), then a value that we'd like to give the property.

