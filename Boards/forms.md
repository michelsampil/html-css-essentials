# HTML FORM ELEMENTS

HTML5 introduces several new elements and attributes to improve form usability and functionality. Here's an extensive summary of HTML5 form elements and their attributes:

## 1. Form Element (<form>)

The <form> element defines a form for user input.

- action: Specifies the URL where the form data will be sent.
- method: Specifies the HTTP method (GET or POST) to use when sending form data.
- autocomplete: Indicates whether the browser should enable autocomplete for the form. Values are on (default) and off.
- novalidate: When present, the form will not be validated when submitted.

<form action="/submit" method="POST" autocomplete="on" novalidate>
  <!-- form elements go here -->
</form>

## 2. Input Element (<input>)

The <input> element is the most common form element, supporting various types of data.

- type: Specifies the type of input (text, password, email, number, date, etc.).
- name: Defines the name of the input, used when form data is submitted.
- value: Specifies the initial value of the input.
- placeholder: Provides a hint to the user about what to enter in the input.
- required: When present, indicates that the input must be filled out before submitting the form.
- readonly: Makes the input read-only.
- disabled: Disables the input, preventing user interaction.
- min and max: Define the minimum and maximum values for inputs of type number, date, etc.
- pattern: Specifies a regular expression that the input's value must match.
- step: Defines the interval between legal numbers for inputs of type number.

<input type="text" name="username" placeholder="Enter your username" required>
<input type="password" name="password" placeholder="Enter your password" required>
<input type="email" name="email" placeholder="Enter your email" required>
<input type="number" name="age" min="0" max="100" step="1">
<input type="date" name="dob">

## 3. Textarea Element (<textarea>)

The <textarea> element is used for multi-line text input.

- name: Defines the name of the textarea, used when form data is submitted.
- rows and cols: Specify the visible number of rows and columns in the textarea.
- placeholder: Provides a hint to the user about what to enter in the textarea.
- required: When present, indicates that the textarea must be filled out before submitting the form.
- readonly: Makes the textarea read-only.
- disabled: Disables the textarea, preventing user interaction.

<textarea name="message" rows="5" cols="40" placeholder="Enter your message" required></textarea>

## 4. Select Element (<select>)

The <select> element creates a drop-down list.

- name: Defines the name of the select element, used when form data is submitted.
- multiple: Allows multiple selections if present.
- required: When present, indicates that an option must be selected before submitting the form.
- disabled: Disables the select element, preventing user interaction.

<select name="country" required>
  <option value="usa">USA</option>
  <option value="canada">Canada</option>
  <option value="mexico">Mexico</option>
</select>

## 5. Option Element (<option>)

The <option> element defines an option in a select list.

- value: Specifies the value to be submitted if the option is selected.
- selected: Specifies that the option should be pre-selected when the page loads.
- disabled: Disables the option, preventing it from being selected.

<select name="language">
  <option value="en" selected>English</option>
  <option value="es">Spanish</option>
  <option value="fr">French</option>
</select>

## 6. Button Element (<button>)

The <button> element represents a clickable button.

- type: Specifies the type of button (button, submit, or reset).
- name: Defines the name of the button, used when form data is submitted.
- value: Specifies the initial value of the button.
- disabled: Disables the button, preventing user interaction.

<button type="submit">Submit</button>
<button type="reset">Reset</button>
<button type="button" onclick="alert('Hello!')">Click me</button>

## 7. Fieldset and Legend Elements (<fieldset>, <legend>)

The <fieldset> element is used to group related elements in a form, and the <legend> element provides a caption for the <fieldset>.

disabled: Disables all the form controls within the fieldset if present.

<fieldset>
  <legend>Personal Information</legend>
  <input type="text" name="firstname" placeholder="First Name" required>
  <input type="text" name="lastname" placeholder="Last Name" required>
</fieldset>

## 8. Datalist Element (<datalist>)

The <datalist> element contains a set of <option> elements that represent the permissible or suggested options available to users in other controls.

<input list="browsers" name="browser" placeholder="Choose a browser...">
<datalist id="browsers">
  <option value="Chrome">
  <option value="Firefox">
  <option value="Safari">
  <option value="Edge">
  <option value="Opera">
</datalist>

## 9. Output Element (<output>)

The <output> element represents the result of a calculation.

<form oninput="result.value=parseInt(a.value)+parseInt(b.value)">
  <input type="number" id="a" name="a" value="0"> +
  <input type="number" id="b" name="b" value="0"> =
  <output name="result" for="a b">0</output>
</form>

## 10. New Input Types in HTML5

- color: For color input.
- date: For date input.
- datetime-local: For date and time input.
- email: For email address input.
- month: For month and year input.
- number: For numeric input.
- range: For input control with a range of values.
- search: For search input.
- tel: For telephone number input.
- time: For time input.
- url: For URL input.
- week: For week and year input.

<input type="color" name="favcolor">
<input type="date" name="bday">
<input type="datetime-local" name="appointment">
<input type="email" name="email">
<input type="month" name="bdaymonth">
<input type="number" name="quantity">
<input type="range" name="points" min="0" max="10">
<input type="search" name="search">
<input type="tel" name="phone">
<input type="time" name="appt">
<input type="url" name="homepage">
<input type="week" name="week">
