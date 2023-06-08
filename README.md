# Accessibility-Quiz-Page
This project is a practice quiz for HTML and CSS concepts.<br />
It features a responsive layout, semantic HTML, and accessibility enhancements. <br />
The quiz includes sections for student information, HTML questions, and CSS questions. <br />

The project includes an HTML form with multiple sections, each focusing on a different topic. The sections include:
* <b>Student Info:</b> This section allows students to input their name, email, and date of birth.
* <b>HTML Questions:</b> Here, you will find a couple of true/false questions related to HTML.
* <b>CSS Questions:</b> This section includes a dropdown menu and a textarea <br/>
for students to provide information about their experience as a frontend developer<br />
and ask any CSS-related questions they might have.<br />

The project utilizes semantic HTML elements and incorporates accessibility features <br />
to ensure a better user experience for everyone. <br />
It also includes a responsive design using CSS Flexbox for the header and other layout elements. <br /><br />




## Concepts Learned

- The Lang attribute:
  - Assist screen readers in identifying the language of the page.<br />

- Meta element:
  - Specify information about the page (title, description, keywords, author, viewport definition, description definition, character encoding).
  - utilizing this element improves visual accessibility on mobile and SEO.<br />

- Title element (screen-reader):
  - Useful for screen readers to understand the content of a page.
  - Important for SEO.<br />

- Semantic HTML Element:
  - Core part of accessibility.
  - screen readers rely on the provision of an acute structure of the page
  - Use semantic HTML elements (header, main, footer) to provide page structure.
  - Header element for page introduction and navigation menu.<br />

- Nav Semantic Element:
  - Container for text links to different parts of the page. <br />

- Section Semantic element:
  - this semantically separates parts of a webpage
  - it was used in this project to separate content within a form semantically. <br />

- Footer/address Semantic Element:
  - Footer: Container for related content on the page.
  - Address: Container for contact information of the author. <br />

- SVG images:
  - SVG images contain a path attribute, allowing scaling without affecting resolution.<br />

- Aspect-ratio property:
  - Describes proportional relationship between width and height.
  - Preferred aspect ratio and default height.
  - aspect-ratio: auto|initial|inherit|revert|revert-layer|unset|<ratio>
  - e.g aspect-ration: 35 /4; <br />

- Max/min function:
  - Choose between values based on maximum/minimum. <br />

- Max-width/min-width property :
  - Max-width: sets the maximum width that an element can have.
  - Min-width: when browser window is smaller than the min-width there would be an overflow. <br />

- **Role attribute**:
  - Indicate the purpose of an element to assistive technologies.
  - Use preset values (e.g., region value on section element). <br />

- **Aria-labelledby attribute**:
  - Labels a region.
  - Required for every region role.
  - it was used in this project to label each section of the form to assistive technologies.<br />

- "Label element" to "input element" (for attribute):
  - Link each input to the corresponding label element for visual reference. <br />

- Position property:
  - Specify positioning method for an element (absolute, relative, fixed, sticky, static ).
  - Top, bottom, left, and right properties defines the elements coordinates. <br />
  they work differently depending on the positioning method used <br />
  
- Positioning things on image:
  - Position text on an image using container and absolute positioning.
  - Reduce image opacity.

- Overflow property:
  - Control content that is too big to fit in an area.
  - Specify whether to clip or add scrollbars.
  - overflow: visible|hidden|scroll|auto
  - overflow-x: specifies what to do with the left/right edges of the content.
  - overflow-y: specifies what to do with the top/bottom edges of the content. <br />

- Clip property:
  - Clip an absolutely positioned element using a rectangle.
  - the rectangele acts as a window, such that only through this rectangle, can you see the element.
  - the four coordinates of the rectangle is specified from the top-left corner.
  - for this property to be effective **overflow should not be visible** & **position should be absolute**

- White-space property:
  - Specify how white-space inside an element is handled.
  - Affects text behavior and wrapping.
  - white-space: normal|nowrap|pre|pre-line|pre-wrap|initial|inherit;

- Text only the Screen Reader can read:
  - Use CSS techniques to hide text visually but would still be accessible to screen readers.
  - make element absolutely positioned, a 1px by 1px size, <br />
  hidden overflow, nowrap white space, a clip retangle of size 0 (rect(0,0,0,0) - no window)<br />

- ::before, ::after pseudo-elements:
  - Insert generated content before/after an element. <br />

- Content property:
  - Used with ::before, ::after pseudo-elements to insert generated content.<br />

- Contrast (visual accessibility):
  - Measure contrast ratio between text/graphics and background color/image.
  - a white text on a white background has a contrast ration of 1. this is impossible to perceive
  - a black text on a white background has a contrast ratio of 21.
  - Aim for minimum contrast ratio of 4.5.
  
  - Any interactive component has different states.
  - for example hover, focus, active, unvisited, visited and deactivated.
  - remember to ensure that the states also have good contrast.
  - there are online tools to check the constrast ratio of 2 colors<br />

- Cursor property:
  - Specify mouse cursor appearance when hovering over an element. <br />

- Display: inline VS display: inline-block:
  - Inline-block allows setting width and height on the element.
  - Inline-block respects top/bottom margins/paddings.

- Display: block VS display: inline-block:
  - inline-block does not add a line-break after the element,
  - so the element can sit next to other elements.
  
- **scroll-behaviour property**:<br/>
    Clicking on the navigation links should jump <br />
    the viewport to the relevant section. <br />
    However, this jumping can be disorienting for some users.

    The scroll-behavior property specifies <br />
    whether to smoothly animate the scroll position, <br />
    instead of a straight jump, <br />
    when the user clicks on a link within a scrollable box.<br />
    By setting scroll-behavior: smooth <br /><br />
  
- **Media-rule (prefers-reduced-motion)**:<br />
    Setting the scroll-behavior to smooth is preferred by most users. <br />
    However, some users find this to be too slow, <br />
    they prefer to have the scrolling happen instantaneously.

    There exists a media rule to set CSS based on the user's browser settings called 
    **prefers-reduced-motion**

    This accepts one of two values "reduce" & "no-preference" <br />
    We can specify within a prefers-reduced-motion media rule whose user's browser setting is "no-preference"
    that the scroll-behaviour should be smooth. via **@media (prefers-reduced-motion: no-preference)**
