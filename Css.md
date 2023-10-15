#About CSS

#### <ins> What is CSS?
CSS, or Cascading Style Sheets, is a technique used for adding style to a web page. CSS is used to arrange the layout of a webpage, giving you control over aspects such as text color, font, spacing, text size, background pictures or colors, and much more. It styles HTML components rather than creating new ones. CSS may be embedded into HTML texts in three ways: inline, internal, and external, with external being the most commonly used method. With an external style sheet, you may change the whole appearance of the website by modifying only one file. CSS is used by front-end developers to design the layout of web pages, including changing the font, color, and size.
<ul>
<li> <b> Explain what the "box model" CSS is and the layout components that make it up?</b>
The box model is a fundamental concept in CSS that governs the layout and sizing of elements on a webpage. It describes how every HTML element is represented as a rectangular box, comprising content, padding, border, and margin. The content refers to the actual information or visuals within the element, while padding provides space between the content and the border. The border outlines the content and padding, and the margin creates space between the element and its neighboring elements. The dimensions of the box, such as width and height, are determined by the sum of content, padding, and border. Understanding the box model is crucial for precise element positioning and layout control in CSS, ensuring consistent and predictable designs across different browsers and devices.
<ul>
<li>Content - The content of the field, which reflects all images and text</li>
<li>Padding - the transparent area that surrounds the content (the amount of space between the border and the content)
</li>
<li>Border - border surrounding the padding (if any) and content
</li>
<li>Margin - is the transparent area around the border (the amount of space between the border and any neighboring elements)</li>

</ul>
</li>
<li><b>Head Tag: </b> the head contains machine-readable metadata about the page and typical sub elements include the title, meta tags, script tags, and stylesheets of (or links to stylesheets). They are not to be confused with header tags of various levels of headings (h1, h2 etc) which define the structure of the page as you would in an outline.</li>
<li><b>EM vs REM</b>: EM are relative to the immediate parents while REM is only relative to the html (root) font-size.</li>
<li><b>Z-Index: </b>Z-index is used to specify the stack order of elements that overlap each other. Its default value is zero and can take both negative and positive values. A higher z-index value is stacked above the lower index element. It takes the following values- auto, number, initial, and inherit. </li>
<li><b>Block Elements </b>are <code>div</code> and <code>p</code>. They usually start on a new line and can take space for an entire row or width.</li>
<li><b>Inline elements </b> <code>a</code>, <code>span</code>, <code>strong</code>, and <code>img</code> tags. They don't start on a new line. However, they appear on the same line as the content and tags beside them.</li>
<li><b>Inline block elements </b> have padding and margins and set height and width values. Though, they are similar to inline elements</li>

<li><b> tag vs attribute: </b>tags define page elements and the text enclosed by them (if any), usually with a start and end tag while attributes are name value pairs that pertain to tags and are defined within a start tag. Common attributes include id (which must be unique to identify an element on a page), class and style. In the example below, “p” is a tag while “style” is an attribute.

```JS
<p style=“color:blue” >This is a paragraph</p>
```
</li>
<li><b>Difference between Span & Div </b> <code>div</code> is a block element and <code>span</code> is an inline element. Placing a block element inside an inline element is illegal. Although a div can have a p tag, and a p tag can have a span, a span can't have a div or p tag inside. </li>
<li><b>What are the different types of CSS selectors?</b>CSS selectors are used to select elements in an HTML document. There are several types of CSS selectors, including class selectors, ID selectors, and attribute selectors.</li>
<li><b>What is a pseudo-class?</b>A pseudo-class is a selector that styles an element based on its state. For example, the <code> :hover </code>pseudo-class styles an element when the user hovers over it with their mouse but does nothing when they don't.</li>
<li><b>What is a CSS reset?</b>A CSS reset is a set of rules applied to all browsers to normalize the default styling of HTML elements. It’s particularly useful when stripping the formatting of HTML elements.</li>
<li><b>What is a CSS grid system?</b>A CSS grid system is a set of rules that can be used to create a responsive layout. There are many different grid systems available, but the most popular one is Bootstrap. Bootstrap makes it easier to create layouts that react predictably without having to reinvent the wheel.
</li>
<li><b>What is a CSS preprocessor?</b>A CSS preprocessor is a tool that allows you to write CSS in a more concise and structured manner. The most popular CSS preprocessors are Less and Sass. They aren't very useful for small projects but become exponentially more powerful as a project grows. There are several benefits of using a CSS preprocessor, such as writing code in a more structured and concise manner, reducing the amount of code that needs to be written, and making it easier to maintain and update code. More importantly, it makes it easier to manage a project among large numbers of devs.</li>
 <li><b>What is a task runner?</b>Task runners are tools that help automate common tasks in the development process, such as minification, compilation, linting, etc. Some of the most popular task runners are Gulp and Grunt.</li>
  <li><b>What do media queries in CSS accomplish?</b> In CSS, media queries allow you to apply alternative styles or rules to a webpage based on certain parameters such as the device’s screen size, orientation, resolution, or other features. They make it possible to develop responsive designs that adjust to multiple devices and deliver an ideal user experience across a range of screen sizes. A media query is made up of a media type (for example, screen or print) and one or more expressions that describe the circumstances under which the styles should be applied. </li>
 <li><b>How do you use media queries to optimize for different screen sizes?</b>Media queries are a CSS3 feature that allows you to apply different styles based on the screen’s width. To use media queries, you would first need to include a viewport meta tag in your HTML. Then, you would need to write your CSS using media queries -- but integrating it into the HTML is important, too.</li>
 <li><b>What are the differences between inline, embedded, and external stylesheets?</b>Inline styles are written as a part of the code (<div style=”background-color: blue”>), embedded styles are style sheets embedded in the header of the page, and external style sheets are linked within the header of the page.</li>
 <li><b>Can you explain the concept of a CSS float and provide an example of its usage?</b>A CSS float tells the browser to put a particular element to the right side or the left side of the container. I use floats when I’m developing a page that dynamically resizes based on the user resolution.</li>
 <li><b>CSS selectors </b>There are five main types of CSS selectors:
 <ul>
<li><b>Universal Selector: </b>The Universal Selector selects all elements on a webpage.</li>
<li><b>Element Selector: </b>The Element Selector matches HTML elements with the same name.</li>
<li><b>ID Selector:</b>The ID Selector matches elements with ID attributes that have the same value.</li>
<li><b>Class Selector: </b>The Class Selector matches elements with class attributes that have the same name.</li>
</ul>
 </li>
<li><b>Margin: </b> The space outside of an element’s border is referred to as its margin. It is used to create a distance between an element and the elements around it. Margins can be used to space out a list of items or to create a gap between two columns of text, for example. the margin: auto attribute can be used to center the element itself </li>
<li><b>Padding: </b> Padding is the space between the border of an element and its content. It is used to provide space between an element’s content and its border. Padding can be used to provide a border around an image or to add space around words in a paragraph.</li>
<li><b>display: flex</b>attribute may also be used to center an element both horizontally and vertically. This turns the element into a flex container, which implies that its children are automatically centered.</li>
<li><b>justify-content property</b> determines how the flex container’s children are aligned horizontally,</li>
<li><b> align-items property</b>determines how the flex container’s children are positioned vertically. </li>
 <li><b>position: absolute property</b>used to center an element both horizontally and vertically. This will position the element relative to its parent element, and then you can use the top and left properties to specify the exact position of the element. </li>
 <li><b>benefits of using responsive web design</b>
 <ul>
<li><b>Improved User Experience:</b>In frontend development a responsive design allows your website to be easily accessible on all devices. This means that users can easily navigate your website and find the information they are looking for, regardless of the device they are using.</li>
<li><b>Increased Accessibility:</b>Responsive web design makes your website more accessible to people with disabilities. This is because the layout of your website will automatically adjust to the size of the screen, so people with limited mobility can still use it.</li>
<li><b>Better SEO: </b>Google and other search engines favor websites that are responsive. This means that your website will be more likely to appear high in search results if it is responsive.</li>
</ul>
 </li>
</ul>
<ul>
<li><b>Mixin</b> - Mixin is one of the blocks of code with which we can group CSS declarations. We can reuse these declarations on the site.</li>
<li><b> adaptive design and responsive design: </b>
<ul>
<b>Adaptive:</b>
<li>Main focus is to develop a website in multiple fixed layout sizes.</li>
<li>Offers good control over the design to develop variation in screens.</li>
<li>It is very time-consuming and takes a lot of effort to build the best possible adaptive design as examining it will need to go for many options with respect to the realities of the end user.</li>
<li>There are six standard screen sizes for the appropriate layouts; they are 320px, 480px, 760px, 960px, 1200px, 1600px to design.</li>
<b>Responsive: </b>

<li>Main focus is to show content with respect to browser space.</li>
 <li>Offers less control over the design.</li>
 <li>It takes less time to build the design and there is no screen size issue irrespective of content.</li>
 <li>It uses CSS media queries to design the screen layouts with respect to specific devices and property changes in the screen.</li>
</ul>
</li>
<li><b>Cascading: </b>Cascading is defined as the process of style declaration and its weight that will help the browser in selecting the styling rules with respect to time. NOTE: Preprocessor (SASS, LESS, etc.) variables don’t cascade.</li>
<li><b>!important: </b>The style “!important” in the CSS has the highest precedence. Also, the cascaded property will be overridden with it.</li>
<li><b>When does DOM reflow occur?</b> DOM reflow occurs when you insert, move, update, remove, and animate the elements in the DOM as well as when you modify content on the page and change style.</li>
<li><b>Accessibility (a11y): </b>Accessibility is to make the system accessible in such a manner that the website should have the text-to-speech capability, for people with physical disabilities, designed with the help of software or hardware combinations.</li>
<li><b></b></li>
<li><b></b></li>
<li><b></b></li>
<li><b></b></li>
<li><b></b></li>
</ul>
