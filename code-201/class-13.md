# Readings



## [Local Storage and How To Use It On Websites](https://www.smashingmagazine.com/2010/10/local-storage-and-how-to-use-it/)

1. Why would a developer use local storage for a web application?
   * Developers use local storage in web applications to store data on the client-side, ensuring persistent data storage even after the browser is closed. It improves application performance by reducing server requests, supports offline functionality, and reduces bandwidth usage. 
2. What information should not be stored in local storage?
   * Sensitive information like passwords, authentication tokens, or personally identifiable information.
3. Local storage can store what type of data? How would you convert it to that type before storing?
   * Local storage primarily stores data in the form of strings. To store other data types like objects, arrays, or numbers, you need to convert them to strings before saving to local storage. You can use the JSON.stringify() method to convert objects and arrays to JSON strings. For numbers or other data types, you can use the String() function or manually convert them to strings before saving to local storage. 


## Bookmark/Skim

## [“The Past, Present, and Future of Local Storage for Web Applications”](http://diveinto.html5doctor.com/storage.html)


## Things I want to know more about

## JSON.stringify()  and JSON.parse() methods

JSON.stringify():

1. JSON.stringify() is used to convert a JavaScript object or value into a JSON string.
1. It takes one or two parameters: the first parameter is the value to be converted to a JSON string, and the second parameter is a replacer function or an array that specifies how values are transformed.

## Example


            const person = {
            name: "John",
            age: 30,
            city: "New York"
            };
            const jsonString = JSON.stringify(person);
            console.log(jsonString);


   The jsonString variable will contain the JSON representation of the "person" object.


1. JSON.parse() is used to parse a JSON string and convert it into a JavaScript object or value.
1. It takes a single parameter: the JSON string to be parsed.
   
## Example:

                const jsonString = '{"name":"John","age":30,"city":"New York"}';
                const person = JSON.parse(jsonString);
                console.log(person.name); // Outputs "John"

    The "person" variable now holds a JavaScript object created from the JSON string.
JSON.stringify() and JSON.parse() are essential for working with data in web applications, particularly when you need to send data to a server or store it locally. They help maintain the data's structure and ensure interoperability between different systems.            


