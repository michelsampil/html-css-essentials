# CSS display Property

The display property determines how an element is displayed on the web page. It has multiple values, each affecting the element's behavior in terms of layout and rendering.

## display Property Values

### none:

Description: The element is not displayed at all. It does not take up any space in the layout.

Use Case: Hiding elements dynamically, such as in response to user interactions or for conditional rendering.

### block:

Description: The element is displayed as a block element, meaning it starts on a new line and takes up the full width available.

Use Case: Creating block-level containers like <div>, <p>, and <header>.

### inline:

Description: The element is displayed as an inline element, meaning it does not start on a new line and only takes up as much width as necessary.

Use Case: Styling text elements like <span> or <a>.

### inline-block:

Description: The element is displayed as an inline element but can have width and height set, behaving like a block element in that sense.

Use Case: Creating elements that need to be inline but also require block-level styling, such as buttons or navigation links.
flex:

Description: The element becomes a flex container, enabling a flexible layout system for its children using the Flexbox model.

Use Case: Creating responsive layouts with flexible and dynamic arrangement of elements.

### inline-flex:

Description: The element behaves like an inline element but also a flex container for its children.

Use Case: Creating inline elements that need the flexible layout capabilities of Flexbox.
grid:

Description: The element becomes a grid container, allowing its children to be placed within a grid layout system.

Use Case: Creating complex, responsive layouts using CSS Grid.

### inline-grid:

Description: The element behaves like an inline element but also a grid container.

Use Case: Using CSS Grid layout in an inline context.

### table:

Description: The element behaves like a <table> element, making it a block-level table.

Use Case: Creating table-like structures without using the actual <table> element.

### inline-table:

Description: The element behaves like an inline element but also as a table.

Use Case: Creating table-like structures in an inline context.

### list-item:

Description: The element behaves like a list item (<li>), including markers.

Use Case: Creating custom list items or styling without using the <ul> or <ol> elements.
run-in:

Description: The element behaves like a block or inline element depending on the context.

Use Case: Rarely used due to inconsistent browser support and limited practical applications.

### initial:

Description: Sets the property to its default value.

Use Case: Resetting the display property to its initial value.

### inherit:

Description: The element inherits the display property value from its parent.

Use Case: Ensuring consistent display behavior across nested elements.

### contents:

Description: The element itself is not rendered, but its children are rendered as normal.

Use Case: Removing wrapper elements without affecting their children’s display.
table-row, table-cell, table-column, table-row-group, table-column-group, table-footer-group, table-header-group, table-caption:

Description: These values mimic the behavior of corresponding table elements.

Use Case: Creating table structures without using the actual <table> element.

# CSS position Property

The position property specifies how an element is positioned in the document. It also determines whether it will use the normal document flow or be taken out of it.

## position Property Values

### static:

Description: The default value. The element is positioned according to the normal document flow.

Use Case: Standard document flow positioning without any additional positioning.

### relative:

Description: The element is positioned relative to its normal position. Offsets (top, right, bottom, left) will move it from that position.

Use Case: Slightly adjusting an element's position while maintaining its space in the layout.
absolute:

Description: The element is positioned relative to its nearest positioned ancestor (anything other than static), or to the initial containing block if no such ancestor exists. It is removed from the normal document flow.

Use Case: Precisely positioning an element anywhere within its containing block.

### fixed:

Description: The element is positioned relative to the viewport, meaning it stays in the same place even if the page is scrolled. It is removed from the normal document flow.

Use Case: Creating sticky headers, footers, or other elements that need to remain visible regardless of scroll position.

### sticky:

Description: The element is positioned based on the user's scroll position. It toggles between relative and fixed positioning, depending on the scroll position.

Use Case: Creating elements that stick to the viewport when scrolling past a certain point, like sticky headers or sidebars.

### initial:

Description: Sets the property to its default value.

Use Case: Resetting the position property to its initial value.

### inherit:

Description: The element inherits the position property value from its parent.

Use Case: Ensuring consistent positioning behavior across nested elements.

# Positioning Properties

When using relative, absolute, fixed, or sticky positioning, the following properties can be used to adjust the position of the

## element:

top: Moves the element down from the top of its containing block.
right: Moves the element to the left from the right of its containing block.
bottom: Moves the element up from the bottom of its containing block.
left: Moves the element to the right from the left of its containing block.

## Z-Index

z-index: Specifies the stack order of an element. Elements with a higher z-index will be in front of elements with a lower z-index.
Use Case: Controlling the stacking order of positioned elements to ensure they are layered correctly.

Combining display and position

The display and position properties can be combined to achieve complex layouts and precise positioning. For example, you can use display: flex to create a flexible layout and position: absolute to precisely position elements within that layout.

## Example Use Cases

### Responsive Navigation Bar:

Display: flex
Position: fixed for the navbar, ensuring it stays at the top of the viewport.

### Modal Dialog:

Display: block for the modal background and content.
Position: fixed for the modal, centered in the viewport with top, left, transform for centering.

### Tooltip:

Display: inline-block for the tooltip text.
Position: absolute to position the tooltip relative to its parent element.

### Sticky Sidebar:

Display: block for the sidebar.
Position: sticky to keep the sidebar visible as the user scrolls.
