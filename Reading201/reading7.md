# Reading 7

## Domain Object Modeling

Explain why we need domain modeling.

1. Better understanding of the problem domain: Domain modeling helps to gain a deeper understanding of the problem domain and its complexities. By breaking down the domain into smaller, more manageable components, it is easier to identify the key concepts, relationships, and constraints that need to be modeled.

2. Clear communication: A domain model provides a common language and understanding of the problem domain that all stakeholders can use to communicate more clearly and effectively. This reduces misunderstandings and ensures that everyone is on the same page.

3. Improved requirements gathering: By modeling the domain, it is easier to identify and capture all of the requirements, including both functional and non-functional requirements. This ensures that the system being built meets the needs of all stakeholders.

4. Facilitates system design: Domain modeling helps to define the overall structure of the system being built. It provides a high-level view of the system and its components, which is essential for making design decisions.

5. Enables testing: Domain modeling provides a basis for creating test cases and validating the system against requirements. By modeling the domain, it is easier to identify the various scenarios that the system needs to support and to test against these scenarios.

6. Overall, domain modeling is an essential activity in software development, as it helps to ensure that the system being built meets the needs of all stakeholders and that it is designed in a way that is both effective and efficient.

## HTML Table Basics

Why should tables not be used for page layouts?
List and describe 3 different semantic HTML elements used in an HTML `<table>`.

1. Accessibility: Tables can create accessibility issues for users with visual impairments who use screen readers or other assistive technologies to navigate the web. When tables are used for layout, it can be difficult for these users to understand the structure of the content and navigate through it.
2. Maintenance: Using tables for layout can make it more difficult to maintain and update the content of a website. Changing the layout of a page may require changing the HTML structure of the table, which can be time-consuming and error-prone.

3. Compatibility: Tables used for layout may not display correctly on all devices or in all browsers. This can lead to inconsistencies in the appearance of the page and may cause issues for users trying to view the content.

#### Here are three different semantic HTML elements used in an HTML `<table>`:

1. `<thead>`: This element is used to group the header content in a table. It is typically used to contain the row or rows that define the column headers for the table.
2. `<tbody>`: This element is used to group the main content in a table. It is typically used to contain the rows of data in the table.
3. `<tfoot>`: This element is used to group the footer content in a table. It is typically used to contain summary information or totals for the data in the table.

### Introducing Constructors

What is a constructor and what are some advantages to using it?

1. Initialization: The constructor ensures that an object is initialized properly before it is used. This can help prevent errors or unexpected behavior that might occur if an object's properties are not set correctly.
2. Encapsulation: Constructors can be used to ensure that an object's properties are set in a controlled way. By using constructors, you can define how an object is created and restrict access to certain properties or methods.
3. Inheritance: Constructors are inherited by subclasses, which can simplify the process of creating and initializing objects. When a subclass is instantiated, its constructor calls the constructor of the superclass to ensure that the object is properly initialized.
4. Flexibility: Constructors can take arguments, which can be used to provide initial values for an object's properties. This can make it easier to create and configure objects in a flexible and customizable way.
5. Clarity: Using constructors can make your code more readable and easier to understand. By encapsulating the initialization logic in a constructor, you can make it clear to other developers how an object should be created and used. This can help improve the maintainability of your code over time.

Overall, constructors are an important feature of object-oriented programming, as they provide a way to initialize objects in a controlled and consistent way. By using constructors, you can ensure that your objects are properly initialized and that their properties are set in a way that is safe and secure.

How does the term this differ when used in an object literal versus when used in a constructor?
- Object Prototypes Using A Constructor

In JavaScript, the this keyword refers to the current execution context. However, the way this is used can differ when used in an object literal versus when used in a constructor.

When used in an object literal, this refers to the object that the method or property belongs to. For example:

    const myObject = {
      name: 'John',
      greet: function() {
        console.log(`Hello, my name is ${this.name}`);
      }
    };

    myObject.greet(); // Output: Hello, my name is John

In this example, this refers to the myObject object, and the greet method is able to access the name property of the object.

When used in a constructor, this refers to the object that is being created. Constructors are functions that are used to create new objects with a specific set of properties and methods. Here is an example of creating object prototypes using a constructor:

    function Person(name, age) {
      this.name = name;
      this.age = age;
      this.greet = function() {
        console.log(`Hello, my name is ${this.name} and I'm ${this.age} years old`);
      };
    }

    const john = new Person('John', 30);
    john.greet(); // Output: Hello, my name is John and I'm 30 years old

In this example, the Person function is used as a constructor to create a new object with the name and age properties, as well as the greet method. When the new keyword is used to create a new instance of the Person object, this refers to the new object being created. The greet method is then added to the new object as a property, which can be called using john.greet().

Overall, this is a powerful keyword in JavaScript that allows you to reference the current execution context, whether it is an object literal or a constructor. Understanding how this works is essential to writing effective and efficient JavaScript code.

- Explain prototypes and inheritance via an analogy from your previous work experience.

Let's say that you are a chef at a restaurant and you have a recipe for a pizza. The recipe consists of a list of ingredients and instructions for how to make the pizza. This recipe can be thought of as a prototype for creating pizzas.

Now, let's say that you want to create a new type of pizza that is similar to the original pizza but with some variations. You could create a new recipe that is based on the original recipe, but with some modifications to the ingredients or instructions. This new recipe would inherit some of the characteristics of the original recipe but would also have its own unique properties.

In this analogy, the original pizza recipe is like a prototype object in JavaScript. The recipe contains a set of properties and methods that define the characteristics of the pizza. When you create a new pizza recipe based on the original recipe, you are using inheritance to create a new object that shares some of the properties of the original object but also has its own unique properties.

In JavaScript, you can use inheritance to create new objects that inherit properties and methods from an existing object. This can be useful when you want to create multiple objects that share some common characteristics but also have their own unique properties. By using inheritance, you can create new objects that are based on existing objects, which can help you write more efficient and modular code.