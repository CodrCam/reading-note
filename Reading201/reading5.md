# Readings: Lab 5

## Images, Color, Text

### HTML Media

**Using Images In HTML. Read Common Image Types and Choosing Image Formats.**

- What is a real world use case for the alt attribute being used in a website?

  The alt attribute is used for accessibility on images for screen readers, when the internet is slow, and SEO for search engines.

- How can you improve accessibility of images in an HTML document?

  Proper responsiveness to the users browser so they can be seen, along with the above mentioned alt attribute with a solid description.

- Provide an example of when the figure element would be useful in an HTML document.

  Figure is used as a container for an image and description similar to `<article>` but focused on image or visual information.

`<figure>`

  `<img src="example-chart.png" alt="A bar chart` 
  `showing the growth of sales over the last year">`
  `<figcaption>Sales growth over the last year</figcaption>`
`</figure>`

- Describe the difference between a gif image and an svg image, pretend you are explaining to an elder in your community.

The main difference is scalability, SVG can be scaled, and GIFs are a set size. SVG is vector based which means it’s great for scaling to massive sizing like billboards. Making it ideal for brand exposure. Whereas a GIF might be better for a clear set of images for the set size of the publishing method.

-What image type would you use to display a screenshot on your website and why?

  A JPEG or PNG would be ideal. Each has advantages, the JPGs fixed size typically being smaller in size. But a PNG is a lossless image and plays better on larger screens.

**Color in CSS. Styling HTML Text Elements**

- Describe the difference between foreground and background colors of an HTML element, pretend you are talking to someone with no technical knowledge.

  It’s like a coloring book, the foreground the color inside the lines, the background is coloring around the lines. The foreground is like text and other HTML elements. Background is just that it sits behind those elements.

-Your friend asks you to give his colorless blog website a touch up. How would you use color to give his blog some character?

  Start simple with some light color changes like “dark mode” style change.

- What should you consider when choosing fonts for an HTML document?

 How easy is the font size and type to read. Browser safe fonts so I don’t end up with Wing dings. Does the font fit the tone? Performance, if the font needs to be loaded and takes more time than your site and traffic could be affected.

- What do font-size, font-weight, and font-style do to HTML text elements?

  `font-size`, `font-weight`, and `font-style` are CSS properties that control the appearance of text for the HTML doc style

  `font-size` - Changes the physical size of the text

  `font-weight` - affects the thickness of the text by making it light, bold, or bolder.

- Describe two ways you could add spacing around the characters displayed in an h1 element.

  Use the `letter-spacing` the affect the space between the letters within the words. Another way is `word-spacing`in which you can change the space in between the words.
