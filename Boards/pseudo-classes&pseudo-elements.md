# Pseudo-classes

Pseudo-classes are used to define the special state of an element. They can be used to style an element when a user interacts with it or when it is in a specific state. Here’s a comprehensive list of common pseudo-classes:

## Structural Pseudo-classes

- :first-child: Selects the first child of its parent.

- :last-child: Selects the last child of its parent.

- :nth-child(n): Selects the nth child of its parent.

- :nth-last-child(n): Selects the nth child of its parent, counting from the end.

- :nth-of-type(n): Selects the nth child of its type (tag name) of its parent.

- :nth-last-of-type(n): Selects the nth child of its type (tag name) of its parent, counting from the end.

- :first-of-type: Selects the first child of its type (tag name) of its parent.

- :last-of-type: Selects the last child of its type (tag name) of its parent.

- :only-child: Selects an element that is the only child of its parent.

- :only-of-type: Selects an element that is the only child of its type of its parent.

## UI Element States

- :hover: Selects an element when the user hovers over it.

- :focus: Selects an element when it has focus.

- :active: Selects an element when it is activated (e.g., pressed).

- :visited: Selects links that the user has already visited.

- :link: Selects links that the user has not visited yet.

## Form Pseudo-classes

- :enabled: Selects enabled form elements.

- :disabled: Selects disabled form elements.

- :checked: Selects checked radio buttons or checkboxes.

- :indeterminate: Selects indeterminate checkboxes.

- :valid: Selects form elements with valid values.

- :invalid: Selects form elements with invalid values.

- :in-range: Selects form elements with values in a specified range.

- :out-of-range: Selects form elements with values outside a specified range.

- :required: Selects required form elements.

- :optional: Selects optional form elements.

- :read-only: Selects read-only form elements.

- :read-write: Selects form elements that are editable
  (neither read-only nor disabled).
  Negation Pseudo-class

- :not(selector): Selects every element that does not match the specified selector.

## State-based Pseudo-classes

- :root: Selects the document's root element.

- :empty: Selects elements that have no children (including text nodes).
- :target: Selects the current active target element (the element pointed to by the fragment identifier in the URL).

# Pseudo-elements

Pseudo-elements are used to style specified parts of an element. They can be used to style elements that don’t have a corresponding HTML element in the document. Here’s a list of common pseudo-elements:

## Content-based Pseudo-elements

- ::before: Inserts content before the content of an element.

- ::after: Inserts content after the content of an element.

## First-line and First-letter

- ::first-line: Selects the first line of a block-level element.

- ::first-letter: Selects the first letter of a block-level element.

## Selection-based Pseudo-elements

- ::selection: Selects the portion of an element that is selected by a user.

## Element-fragment Pseudo-elements

- ::placeholder: Selects the placeholder text of an input or textarea element.
- ::marker: Selects the marker box of a list item element.
- ::backdrop: Selects the background of the element behind the dialog element when it is open.

## Examples

### Pseudo-classes

- Hover effect

a:hover {
color: red;
}

- First child

div:first-child {
background-color: yellow;
}

- Odd and even children

li:nth-child(odd) {
background-color: lightgrey;
}

li:nth-child(even) {
background-color: white;
}

### Pseudo-elements

- Adding content before and after

p::before {
content: "Note: ";
color: blue;
}

p::after {
content: " Read more.";
color: green;
}

- First letter and first line

p::first-letter {
font-size: 200%;
color: red;
}

p::first-line {
font-weight: bold;
}

- Placeholder styling

input::placeholder {
color: grey;
font-style: italic;
}
