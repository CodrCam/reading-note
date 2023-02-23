# Reading

## CSS Transforms

- What does a CSS transform allow the developer to do to an element?

Here are some of the common transformations that can be applied using CSS transform:

1. Rotate - Rotate the element around a specified point, either in degrees or radians.
2. Scale - Increase or decrease the size of the element, either horizontally or vertically or both.
3. Skew - Skew the element by tilting it along the X or Y-axis.
4. Translate - Move the element along the X and Y-axis.
5. Perspective - Define a 3D perspective for the element.
6. RotateX, RotateY, and RotateZ - Rotate the element around a specific axis in 3D space.
7. Matrix - Define a 2D transformation matrix for the element.

- Provide an example of a transform and how you could see that being used on a website.

      `.box {
        width: 100px;
        height: 100px;
        background-color: red;
        transform: rotate(45deg);
      }`
  *This rotation effect can be used in a variety of ways on a website, such as creating a unique and eye-catching navigation menu or animating a button when it's hovered over by the user.*

## CSS Transitions & Animations

- What does a CSS transition allow the developer to do to an element?

A CSS transition allows a developer to apply an animation effect to an HTML element, specifying a gradual change of the element's style over a defined duration and with a defined timing function.

Here are some of the properties that can be used to define a CSS transition:

1. transition-property: The name of the CSS property to which the transition should be applied.
2. transition-duration: The length of time it takes for the transition to complete, usually in seconds or milliseconds.
3. transition-timing-function: The speed curve of the transition. For example, ease-in, ease-out, linear, etc.
4. transition-delay: The length of time before the transition starts.

Example:

    `.button {
      background-color: blue;
      color: white;
      padding: 10px 20px;
      border: none;
      transition: background-color 0.5s ease;
    }`

    `.button:hover {
      background-color: red;
    }`

- How does a CSS animation differ from a CSS transition?

A CSS transition animates a property from one state to another over a specified period of time. It is designed to create a smooth and gradual transition between two states of an element. A transition is triggered when the state of the element changes, such as when it's hovered over, clicked, or focused.

A CSS animation, on the other hand, allows developers to create complex and more advanced animations by defining a series of keyframes. Unlike a transition, an animation doesn't depend on a change of state and can be triggered at any time.

- What are some benefits to using CSS transitions on websites?

1. Improved user experience: CSS transitions can make a website feel more responsive and engaging to users. They create a smooth and gradual change between two states, which can be more visually appealing than an abrupt change.
2. Cross-browser compatibility: CSS transitions are supported in all modern web browsers, making them a reliable way to add animation effects to websites. They can also be used in conjunction with JavaScript animations for even more flexibility.
3. Accessibility: CSS transitions can be used to create more accessible interfaces. For example, adding a transition to a navigation menu can help users understand which option they are hovering over.
4. Flexibility: CSS transitions are highly customizable and can be used to create a wide range of animation effects. They can be used to create subtle effects, such as highlighting links or buttons, or more complex animations such as page transitions.
5. Improved performance: CSS transitions are hardware-accelerated, which means they use the computer's graphics card to perform animations, resulting in improved performance and smoother animation.
6. Ease of use: CSS transitions are relatively easy to implement and require no external libraries or tools. They can be added to an element by simply adding a few lines of CSS code.

How this topic fits in with your long-term goals?

I'm still unsure how deep I'll go on CSS but, I am inspired by the colorful and reactive elements on websites. 
