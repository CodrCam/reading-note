# Reading 6

## JavaScript Object Basics

- How would you describe an object to a non-technical friend you grew up with?

  - Maybe like a "car" object with properties like "make," "model," and "year," and "condition"

- What are some advantages to creating object literals?
How do objects differ from arrays?

  - allow you to define key-value pairs to represent an object's properties
  - grouping related properties and functions together.
  - easily passed as arguments to functions or returned as values from functions
- The array has an ordered list of data, but an object is an unordered collection of key-value items that link to the object loosely.
  - In an array, the keys are always integers (i.e., indices), whereas in an object, the keys can be any string or symbol.
  - Arrays have a length property that tells you how many values are in the array, while objects do not have a length property.
  - Arrays have built-in methods like push, pop, and sort that allow you to add, remove, and rearrange elements in the array, whereas objects do not have these methods
  - Arrays are typically used to store and manipulate collections of similar values (e.g., a list of numbers), while objects are typically used to represent more complex data structures with different types of properties (e.g., a user object with properties like name, age, and email).

- Give an example for when you would need to use bracket notation to access an object’s property instead of dot notation.
Evaluate the code below. What does the term this refer to and what is the advantage to using this?

      const dog = {
       name: 'Spot',
       age: 2,
       color: 'white with black spots',
      humanAge: function (){
         console.log(`${this.name} is ${this.age*7} in human years`);
       }
     }

  - THIS method allows you to extract that you would like, in this case the name and age, which allows a multiplication of 7 to age. Making the code more concise and easier to understand.

### Introduction To The DOM

- What is the DOM?

  - The Document Object Model (DOM) is a programming interface for HTML. Allowing you as the designer to  dynamically access and manipulate the content of the page.

  - The DOM is a tree structure that organizes elements on a web page, with each element represented by a node in the tree. The nodes can manipulate or modify content on the page when you change other ones. 

- Briefly describe the relationship between the DOM and JavaScript.

  - JavaScript and the Document Object Model (DOM) work hand in hand to create a reactive website.

  - JavaScript can interact with the DOM by using its APIs to access and modify the properties and behavior of elements on the page.

  - Using JavaScript to manipulate the DOM, developers can create highly dynamic and responsive web pages that provide a more engaging and personalized user experience.
