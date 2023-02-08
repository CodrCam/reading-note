# Reading 3

## Learn HTML

### Ordered and Unordered lists

- When should you use an unordered list in your HTML document?

    When you want to list out items with bullet points instead of numbers.

- How do you change the bullet style of unordered list items?

   With `list-style` you can remove or change the bullet points.

- When should you use an ordered list vs an unorder list in your HTML document?

    When you desire sequential order of the list as the browser will order it.

- Describe two ways you can change the numbers on list items provided by an ordered list?

    `<ol type=”A”>` - Will use letters
    `<ol type=”I”>` - Will use roman numerals

## Learn CSS

### The Box Model

- Describe the CSS properties of margin and padding as characters in a story. What is their role in a story titled: “The Box Model”?
List and describe the four parts of an HTML elements box as referred to by the box model.

    Margin is the space outside of the contents border. Where you can create space outside of the content. 

    Padding is where you create space inside the border for your content.

### Learn JS

#### Arrays. Operators and Expressions. Conditionals. Loops

- What data types can you store inside of an Array?

    All types from numbers, to strings, booleans, along with objects, and characters.

- Is the people array a valid JavaScript array?

    Yes

- If so, how can I access the values stored? If not, why?

    By using the indexed location of the item you wish to utilize. `<array>[<index>]=`

       const people = [['pete', 32, 'librarian', null], ['Smith', 40, 'accountant', 'fishing:hiking:rock_climbing'], ['bill', null, 'artist', null]]

- List five shorthand operators for assignment in javascript and describe what they do.

`=` x = y - The Value of X is Y
`+=` x = x + y - The value is X plus Y equals X
`*=` x = x * y - The value of X time Y equals X
`-=` x = x - y -  X minus Y equals X
`%=` x = x % y - When you divide X over Y you get remainder X

- Read the code below and evaluate the last expression and explain what the result would be and why.

       let a = 10;
       let b = 'dog';
       let c = false;

// evaluate this
(a + c) + b;

    `10dog` as false doesn’t change the values or content. So you concatenate the 10 and dog.

- Describe a real world example of when a conditional statement should be used in a JavaScript program.

    A conditional statement is used as a decision tree to guide the script through the desired course of actions. 

- Give an example of when a Loop is useful in JavaScript.

    A loop is useful for iterating through data with multiple goals in mind. Allowing for repetitive tasks to become automated and simplified for the user. 
