# Reading 1

## Component-Based Architecture

1. What is a “component”?

In React, a component is a modular and reusable piece of code that defines a part of the user interface. For example, a button component could be created that can be reused across different parts of an application. The button component can be defined using a function that returns a JSX code that describes the button's structure and behavior, such as its text, color, and onClick function. The component can also have properties, such as size and style, that can be customized and passed down from its parent component. This allows developers to create complex user interfaces by composing multiple components together, each with their own properties and behavior.

2. What are the characteristics of a component?

- Modularity: Components are self-contained units that can be easily reused in different parts of an application, making it easier to maintain and scale complex systems.
- Encapsulation: Components encapsulate their implementation details, which means that the internal workings of a component are hidden from other components.
- Reusability: Components can be reused across different parts of an application, which makes it easier to develop and test new features.
- Composability: Components can be combined with other components to create more complex systems, making it easier to build large and complex applications.
- Customizability: Components can be customized by passing down properties (props) that control their behavior and appearance.
- Extensibility: Components can be extended or modified to add new functionality or behavior without affecting the rest of the application.
- Testability: Components can be easily tested in isolation, which makes it easier to identify and fix bugs.

3. What are the advantages of using component-based architecture?

- Reusability: Components are self-contained units that can be easily reused in different parts of an application, which can reduce development time and increase productivity.
- Scalability: Components can be combined and reused to create more complex systems, which makes it easier to scale applications as they grow.
- Modularity: Components encapsulate their implementation details, which means that changes made to one component will not affect other components, making it easier to maintain and update the codebase.
- Separation of concerns: Components allow developers to separate different concerns, such as UI logic and business logic, making it easier to maintain and update the codebase.
- Consistency: Components provide a consistent and standardized way of building user interfaces, which can improve the user experience and make it easier for developers to collaborate on projects.
- Testability: Components can be easily tested in isolation, which makes it easier to identify and fix bugs.
- Faster development: By using pre-built components, developers can focus on implementing the unique features of an application, which can speed up the development process.

## Props (properties)

1. What is Props short for and how to Use it in React.

- Props (short for properties) is a way of passing data from one component to another. Props are passed down from a parent component to its child component as an object, and can be accessed within the child component using the `this.props` syntax. Props can be any type of data, such as strings, numbers, objects, or even functions.

Example:

    // Parent component
        class ParentComponent extends React.Component {
          render() {
            const greeting = "Hello";
            return (
              <ChildComponent greeting={greeting} />
            );
          }
        }

    // Child component
    class ChildComponent extends React.Component {
      render() {
        return (
          <div>{this.props.greeting} World!</div>
        );
      }
    }

2. What is the flow of props?

- The parent component passes down props to its child component(s) by including them in the child component's JSX element as attributes. For example: `<ChildComponent prop1={value1} prop2={value2} />`
- The child component(s) receive the props as an object through their props property.
- The child component(s) can then use the props to render content, or pass them down to their own child components.
- Props are read-only and cannot be modified by the child component(s). If a child component needs to modify the data passed down through props, it should instead lift the state up to its parent component(s) by using callbacks.
- Any changes made to the props in the parent component will be automatically passed down to the child component(s) and trigger a re-render.