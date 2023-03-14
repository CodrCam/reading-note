# Reading 2

## React lifecycle

1. Based off the diagram, what happens first, the ‘render’ or the ‘componentDidMount’?

-`render` is called before `componentDidMount`. 

2. What is the very first thing to happen in the lifecycle of React?

At the beginning of the React component's lifecycle, the component object is constructed and its state and props are initialized. This marks the creation of the component and sets the stage for the later steps in the lifecycle.

3. Put the following things in the order that they happen: componentDidMount, render, constructor, componentWillUnmount, React Updates

- `constructor` -> `render` -> `componentDidMount` -> `re-render updates` -> `componentWillUnmount`

4. What does componentDidMount do?

The `componentDidMount` method is a key part of the React component lifecycle, and it is an excellent place to perform a variety of setup tasks that require access to the DOM or external data sources. For example, if you need to manipulate the DOM directly, such as adding or removing elements, you can use `componentDidMount` to do so. This is also a good place to make network requests or fetch data from an external API, and update the component's state with the result. Additionally, `componentDidMount` can be used to set up subscriptions or event listeners to update the component's state when changes occur.

## React State Vs Props

1. What types of things can you pass in the props?

- Strings, Numbers, Booleans, Objects, Functions, Arrays, and React elements.

2. What is the big difference between props and state?

Props are used to pass data and behavior from a parent component down to its child components. They are a way to customize and configure components, and are read-only, meaning they cannot be modified by the child component.

State is used to manage data within a component itself. State can be modified by the component itself using the `setState` method, triggering a re-render of the component to reflect the updated state.

The key difference between props and state is that props are passed down from parent to child components, while state is managed within a component itself. Additionally, props are read-only and cannot be modified, while state can be updated using the `setState` method.

3. When do we re-render our application?

In React, a component will re-render when its state or props change. React uses a "shallow comparison" to determine if the props or state have changed. If a property has changed, React will re-render the component, but if only a nested property has changed, React may not recognize the change and may not re-render the component. Additionally, some methods in the component lifecycle, such as `shouldComponentUpdate`, can optimize performance by preventing unnecessary re-renders.

4. What are some examples of things that we could store in state?

State in React is used to manage data specific to a component that may change over time, such as user input, API data, loading status, UI state, error messages, and toggle switches, enabling dynamic UI updates in response to user interactions and external data changes.
