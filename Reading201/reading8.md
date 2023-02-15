# Reading

## Learn CSS - Flexbox

- Flexbox is designed for one-dimensional content. Explain what this means.

Flexbox is a layout mode in CSS that is designed to provide a flexible way of arranging and aligning elements within a container. The term "one-dimensional content" refers to content that is arranged in a single dimension, either horizontally or vertically.

In the case of flexbox, the single dimension is determined by the flex-direction property, which can be set to either row or column. When the flex-direction property is set to row, the content is arranged horizontally along the main axis, while when it is set to column, the content is arranged vertically along the cross axis.

The key feature of flexbox is its ability to dynamically adjust the size and position of elements within the container. This is achieved using a set of flexible sizing and alignment properties, such as flex-grow, flex-shrink, and flex-basis, which allow the elements to expand or shrink based on the available space in the container.

Overall, flexbox is designed to provide a flexible and responsive way of laying out one-dimensional content, making it easier to create complex and dynamic layouts that adapt to different screen sizes and devices.

- Explain the difference between the main axis and cross axis.

In Flexbox, the terms "main axis" and "cross axis" are used to refer to the two perpendicular directions in which flex items are arranged within a flex container.

The main axis is determined by the `flex-direction` property, and it defines the primary axis along which the flex items are laid out. For example, if `flex-direction` is set to `row`, the main axis runs horizontally from left to right, while if it's set to `column`, the main axis runs vertically from top to bottom.

The cross axis is perpendicular to the main axis, and its direction is determined by the opposite direction to the `flex-direction` property. So, if `flex-direction` is set to `row`, the cross axis runs vertically from top to bottom, and if it's set to column, the cross axis runs horizontally from left to right.

The main and cross axes are important concepts in Flexbox because they determine how the `justify-content` and `align-items` properties work. The `justify-content` property aligns the flex items along the main axis, while the `align-items` property aligns them along the cross axis.

Overall, understanding the main and cross axes is essential for creating effective and responsive layouts using Flexbox, as it allows you to control the positioning and alignment of flex items within a flex container.

How can using certain properties of flexbox negatively impact accessibility?

1. Overriding natural document flow: One of the key features of Flexbox is that it allows you to change the order in which content appears on the page. However, this can be problematic for users who rely on screen readers, as it can make it difficult for them to navigate the content in a logical order. To avoid this, it's important to use the order property sparingly and only when it's necessary for the design.
2. Using fixed widths and heights: Flexbox provides a number of properties for controlling the size of elements, such as `flex-basis`, `flex-grow`, and `flex-shrink`. However, using fixed widths and heights can make it difficult for users with low vision to read the content, as it may not be resizable. It's generally best to use relative units, such as percentages, ems, or rems, to allow for flexibility and scalability.
3. Overusing `justify-content` and `align-items`: The `justify-content` and `align-items` properties can be useful for aligning and spacing elements, but overusing them can make it difficult for users with cognitive or visual disabilities to understand the layout. In particular, using justify-content: space-between or `justify-content`: `space-around` can create uneven spacing that can be confusing for some users.
4. Not providing adequate color contrast: Flexbox makes it easy to position and align elements on the page, but it doesn't provide any built-in tools for ensuring adequate color contrast. This can be problematic for users with visual impairments who rely on high contrast to read the content. It's important to follow WCAG guidelines for color contrast and use tools like the WebAIM contrast checker to test your design.

Overall, while Flexbox can be a powerful tool for creating layouts, it's important to use it in a way that is accessible to all users. This means understanding the impact of each property on accessibility and making design choices that prioritize inclusivity and usability.

## CSS Layout - Flexbox

What is “Flex-Flow Shorthand”?

`flex-flow` is a shorthand property in CSS that combines the `flex-direction` and `flex-wrap` properties into a single declaration. It allows you to specify both the direction in which the flex items should flow and whether they should wrap to a new line when the container is full.

The `flex-direction` property determines the direction in which the flex items are laid out within the container, and can be set to one of four values:

- `row`: Flex items are laid out in a horizontal row from left to right (the default value).
- `row-reverse`: Flex items are laid out in a horizontal row from right to left.
- `column`: Flex items are laid out in a vertical column from top to bottom.
- `column-reverse`: Flex items are laid out in a vertical column from bottom to top.

The `flex-wrap` property determines whether the flex items should wrap to a new line if they don't fit in a single row or column, and can be set to one of three values:

- `nowrap`: Flex items are not allowed to wrap to a new line and will overflow the container if necessary (the default value).
- `wrap`: Flex items will wrap to a new line if they don't fit in a single row or column.
- `wrap-reverse`: Flex items will wrap to a new line in the opposite direction if they don't fit in a single `row` or `column`.

The `flex-flow` property combines these two properties into a single shorthand declaration, with the `flex-direction` value coming first, followed by the `flex-wrap` value, separated by a space. For example:

    .container {
      flex-flow: row wrap;
    }

This sets the `flex-direction` to row and the `flex-wrap` to wrap, allowing the flex items to flow in a horizontal row and wrap to a new line if necessary. Using the `flex-flow` shorthand can make your code more concise and easier to read, especially when you need to specify both flex-direction and `flex-wrap` together.

What are some advantages of using flexbox over float?

Flexbox and float are both CSS layout techniques, but there are some advantages to using Flexbox over float:

1. Flexbox provides more control over alignment: Flexbox makes it easier to control the alignment and spacing of elements within a container. You can use the `justify-content` and `align-items` properties to control the positioning of elements along the main and cross axes, and use the `flex` property to control the relative sizes of elements. Floats, on the other hand, were primarily designed for positioning images and text within a block of content, and can be more difficult to control for more complex layouts.
2. Flexbox is more intuitive: Flexbox provides a more intuitive and natural approach to layout than floats. It's easier to understand how the layout will work just by looking at the CSS code, without having to visualize how elements will be positioned and floated in relation to each other.
3. Flexbox is more flexible: Flexbox is designed for one-dimensional layouts, but it can also be used for two-dimensional layouts by combining multiple flex containers. This makes it more flexible than float, which can only be used for one-dimensional layouts.
4. Flexbox is responsive by default: Flexbox is designed to be responsive by default, which means it's easy to create layouts that adapt to different screen sizes and devices. By contrast, floats can be more difficult to use in a responsive design, as they require careful positioning and clearance management to avoid overlapping content.
5. Flexbox has better support: Flexbox is now widely supported across all modern browsers, while support for floats can be less consistent across different devices and browsers. This means that Flexbox is a more reliable and consistent way to create layouts that work across a range of devices and browsers.

Overall, while floats can still be useful in some situations, Flexbox offers more control, flexibility, and responsiveness, making it a better choice for many modern web layouts.

How does this topic connect with your long term goals?

I'm not entirely sure yet. I may stay on the backend as I seem to enjoy and be more profiecient at it.
