#### 🔹 CSS

## CSS - which stands for Cascading Style Sheets

It's a markup language used to apply styles for HTML. In simpler terms, if HTML is the structure of a web page, CSS is what makes it look good.

In the world of web development, CSS plays a vital role in creating visually appealing, responsive, and user-friendly websites.

It allows developers to transform simple HTML documents into engaging web experiences that capture users' attention and enhance their interaction with web content.

## Basic Anatomy of a CSS Rule

All of these styles are made up of various CSS rules.

A CSS rule is made up of two main parts: a selector and a declaration block.

'''
selector {
property: value;
}
'''
A selector is a pattern used in CSS to identify and target specific HTML elements for styling.

Examples of selectors include type selectors, class selectors, and ID selectors.

The curly braces provided in the basic syntax are known as a declaration block. A declaration block applies a set of styles for a given selector, or selectors.

Inside the declaration block, you will have a series of declarations. Each declaration consists of a property and a value.

The property is the CSS identifier that specifies which feature is being styled. An example of a property would be the background-color property.

The value would be the specific setting applied to that property. For example, if the property is background-color, a value could be purple, which sets the background color to purple.

After each property name, you need to place a colon, and after each value, you should have a semicolon.

## Meta Viewport Element Used For?

The meta viewport element is a crucial component in responsive web design.

It's a special HTML meta element that gives the browser instructions on how to control the page's dimensions and scaling on different devices, particularly on mobile phones and tablets.

'''

<meta name="viewport" content="width=device-width, initial-scale=1.0">
'''

The width=device-width part tells the browser to set the width of the page to match the screen width of the device. This is essential for creating responsive layouts that adapt to different screen sizes.

The initial-scale=1.0 sets the initial zoom level when the page is first loaded. A value of 1.0 means that the page is displayed at 100% zoom, without any scaling.

By using the meta viewport element, you're ensuring that your web pages are displayed properly on mobile devices.

## Inline, Internal, and External CSS

# Inline CSS

Inline CSS is written directly within an HTML element using the style attribute. It applies styles to a specific element.

Inline CSS is generally used for quick, one-off styles or to override other styles for a specific element.

# Internal CSS

Internal CSS is written within the style tags inside the head section of an HTML document. It applies styles to the entire page and is useful when you need to style a single document.

Internal CSS is best used when you need to apply styles to a specific page rather than across multiple pages. It’s useful for single-page websites or when the styles don’t need to be reused elsewhere.

# External CSS

External CSS is written in a separate .css file and linked to the HTML document using the link element in the head section.

## How Do Width and Height Work?

width and height properties are used to control the dimensions of elements on a webpage.

These properties can be defined in different units such as pixels (px), percentages (%), viewport units (vw, vh), and more.

The width property specifies the width of an element. If you do not specify a width, then the default is set to auto. This lets the browser determine the element's width based on its content, parent, and display type. For a div element, width: auto makes it expand to fill the full width of its parent container.

The height property specifies the height of an element. Similarly, the height is auto by default, which means it will adjust to the content inside.

Pixels are a fixed-size unit of measurement in CSS, providing precise control over dimensions.

The min-width property specifies the minimum width an element can be. Even if the content inside is smaller, the element won’t shrink below this value.

The min-height specifies the minimum height an element can be. It ensures that the element does not become shorter than the set value.

Even though the box has its width and height set to 50px, it will actually be 100px by 100px. This is because the min-width and min-height are set to 100px, which are larger than the specified width and height.

min-width or min-height are larger than the width or height, they will override the smaller values. This ensures that elements don't become too small, which is important for maintaining a consistent and usable design.

The max-width specifies the maximum width an element can grow to, even if there is enough space for it to be wider.

The max-height specifies the maximum height an element can grow to, regardless of the content size.

when max-width or max-height are smaller than width or height, they take precedence. This is important for controlling the maximum size of elements in your layouts.

CSS prioritizes min-width and min-height over width and height. max-width and max-height restrict dimensions if values exceed their limits.
