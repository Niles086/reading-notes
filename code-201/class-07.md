# Object-Oriented Programming, HTML Tables

**Learning Object-Oriented Programming and HTML tables is important because they are fundamental to software development and web design. OOP provides a structured and efficient way to build software systems, while HTML tables are vital for presenting data on web pages and maintaining legacy web content.**

## [Domain Modeling](https://github.com/codefellows/domain_modeling#domain-modeling)

1. Explain why we need domain modeling.
   * Domain modeling is a fundamental step in software development that promotes clarity, consistency, and alignment with business goals. It facilitates collaboration, reduces ambiguity, and supports both the initial development and long-term maintenance of software systems

## Define a constructor and initialize properties

![epicFailVideoTable](img/epicFailVideoTable.png)

Here's an implementation of the EpicFailVideo constructor function.

             var EpicFailVideo = function(epicRating, hasAnimals) {
               this.epicRating = epicRating;
               this.hasAnimals = hasAnimals;
             }
             
             var parkourFail = new EpicFailVideo(7, false);
             var corgiFail = new EpicFailVideo(4, true);
             
             console.log(parkourFail);
             console.log(corgiFail);

 
**This is object-oriented programming in JavaScript at its most fundamental level.**
1. The new keyword instantiates (i.e. creates) an object.
1. The constructor function initializes properties inside that object using the this variable.
1. The object is stored in a variable for later use.

## Generate random numbers

To model the random nature of user behavior, you'll need the help of a random number generator. Fortunately, the JavaScript standard library includes a Math.random() function for just this sort of occasion. 

_EXAMPLE_

            var EpicFailVideo = function(epicRating, hasAnimals) {
            this.epicRating = epicRating;
            this.hasAnimals = hasAnimals;
            }

            EpicFailVideo.prototype.generateRandom = function(min, max) {
            return Math.floor(Math.random() * (max - min + 1)) + min;
            }

            var parkourFail = new EpicFailVideo(7, false);
            var corgiFail = new EpicFailVideo(4, true);

            console.log(parkourFail.generateRandom(1, 5));
            console.log(corgiFail.generateRandom(1, 5));

## [HTML Table Basics](https://developer.mozilla.org/en-US/docs/Learn/HTML/Tables/Basics)

1. Why should tables not be used for page layouts?
   * HTML tables are designed for displaying tabular data, such as spreadsheets. When you use tables for layout, you are misusing the intended purpose of the HTML elements. This can make your web page less accessible and harder to understand for search engines and assistive technologies.
2. List and describe 3 different semantic HTML elements used in an HTML table.
   * The table element is the root element that defines the table structure. It contains all other table-related elements, such as rows, columns, headers, and data cells.
   * The thead element is used to group and define the header section of a table.
   * The th element represents a table header cell. It is used within the thead element to define column or row headers. 
  
## [Introducing Constructors](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Objects/Basics#introducing_constructors)

1. What is a constructor and what are some advantages to using it?
   * A constructor is responsible for initializing and setting up the initial state of an object when an instance of a class is created.
   * Constructors can encapsulate the initialization logic, hiding the details of how an object is initialized from the outside world.
   * Constructors promote consistent object creation by ensuring that all instances of a class start with the same initial values or configurations. 
2. How does the term this differ when used in an object literal versus when used in a constructor?
   *In an object literal, this refers to the object itself, which is the object that is currently being defined. It allows you to set properties and methods within the object, and those properties and methods can reference other properties or methods within the same object.
   *When used in a constructor function, this refers to the newly created instance of the object, not the object itself. It's a placeholder for the specific instance being created. Constructors are typically used to create multiple instances of objects with similar properties and methods.
   
## [Object Prototypes Using A Constructor](https://ui.dev/beginners-guide-to-javascript-prototype)

1. Explain prototypes and inheritance via an analogy from your previous work experience.
   * Prototypes:Think of prototypes as standardized configuration templates for different types of network devices in your organization. These templates outline the common configurations, settings, and security policies that all devices of a specific category should adhere to.
   In my role as a network admin, i had templates like "Router Template," "Switch Template," and "Firewall Template." These prototypes define the common settings and configurations that all routers, switches, and firewalls should have.
   * Inheritance in this analogy relates to how specific network devices inherit configurations and settings from their respective prototypes. When you deploy a new network device, you start with one of these templates as a base.
   For example, when setting up a new router, you begin with the "Router Template." This template includes essential configurations for routing protocols, access control lists, and interface settings. You customize this base configuration by adding specific details like IP addresses, subnet masks, and routing table entries.
## Bookmark and Review

## [HTML Table Advanced Features and Accessibility](https://developer.mozilla.org/en-US/docs/Learn/HTML/Tables/Advanced)

## Things I want to know more about

I want to leard more about server side databases so i can make more complex tables 