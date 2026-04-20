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

## Default Browser Styles Applied to HTML

When you start working with HTML and CSS, you'll notice that some styles are applied to your web pages even before you write any CSS. These styles are called "default browser styles" or "user-agent styles".

These default browser styles provide basic formatting to ensure that HTML elements are displayed in a readable way across all browsers.

Headings are one of the most commonly used HTML elements and are styled by default to have varying sizes and weights.

Blockquotes are used to indicate a section of text that is a quotation from another source. Browsers typically add indentation and sometimes italicize the text.

The indentation helps set blockquotes apart from the rest of the text, making it clear that this content is quoted from another source.

Another element with default styles is the anchor element (<a>), which is styled with a default blue color and underlining to make it recognizable as a link.

## Inline, Internal, and External CSS

Inline CSS is written directly within an HTML element using the style attribute. It applies styles to a specific element.

# Inline CSS

Inline CSS is generally used for quick, one-off styles or to override other styles for a specific element.
It can clutter the HTML and make the code harder to maintain.

# Internal CSS

Internal CSS is written within the style tags inside the head section of an HTML document. It applies styles to the entire page and is useful when you need to style a single document.

Internal CSS is best used when you need to apply styles to a specific page rather than across multiple pages. It’s useful for single-page websites or when the styles don’t need to be reused elsewhere.

# External CSS

External CSS is written in a separate .css file and linked to the HTML document using the link element in the head section.

It allows you to style multiple pages consistently and is the preferred method in professional web development.

## How Do Width and Height Work?

The width and height properties are used to control the dimensions of elements on a webpage.
