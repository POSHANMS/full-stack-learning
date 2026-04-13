Forms

The form element in HTML is used to gather user information, such as names and email addresses. Here is an example of a form element:

<form action="url-goes-here">
    input elements go here
</form>

The action attribute specifies where the form data will be sent upon submission.

To collect specific information, like names and email addresses, you would use the input element.

<form action="">    
    <input type="text"/>
</form>
The type attribute defines the data type expected from the user.

To add a label for the input, you would use a label element.

 <form action = "">
    <label>
        Full Name:
        <input type="text" />
    </label>
</form>
By nesting an input inside a label element, you create an implicit association between the label and the input field.

The term "implicit" refers to something that is understood or inferred without needing to be explicitly stated or defined with additional attributes or elements. To explicitly associate a label with an input, you can use the for attribute.

<form action = "">
    <label for="email"> Email Address: </label>
    <input type="email" id="email" />
</form>
When using an explicit association, the values for the for attribute and id need to be the same.

If you want to show additional hints to the users about the expected input, you can use the placeholder attribute.

<form action = "">
    <label for="email"> Email Address: </label>
    <input type="email" id="email" placeholder="example@gmail.com" />
</form>

Button

The button element is used to perform a particular action when it is activated. Here is an example of a button element with the button text of Start Game.
<button>Start Game</button>

The button element has a type attribute which controls the behavior of the button when it is activated. The first possible value for the type attribute would be the button type.
<button type="button">Show Alert</button>

Another possible value for the type attribute is the submit value. Here is an example of using a button element with the submit type.

<form action="">
    <label for="email">Email address:</label>
    <input type="email" id="email" name="email" />
    <button type="submit">Submit form</button>
</form>

When the user clicks on the submit button, their data will be sent to the server and will be processed. The third possible value for the type attribute is the reset value.

<form action="">
    <label for="email">Email address:</label>
    <input type="email" id="email" name="email" />
    <button type="reset">Reset form</button>
    <button type="submit">Submit form</button>
</form>

Validation in HTML Form

While client-side validation is important, you also need server-side validation for added security. Malicious users can bypass client-side checks, so robust server-side measures are essential. You'll learn more about this in a later module. For now, let's take a look at some examples of client-side form validation.

<form action="">
    <label for="email>Email Address (Required field): </label>
    <input required type="email" name="email" id="email" />
    <button type="submit">Submit Form</button>
</form>

Other forms of validation for email inputs are to use the minlength and maxlength attributes.

<form action="">
    <label for="email>Email Address (Required field): </label>
    <input 
    required 
    type="email" 
    name="email" 
    id="email"
    minlength="4"
    maxlenght="64"
     />
    <button type="submit">Submit Form</button>
</form>
The minlength and maxlength attributes are used to set the minimum and maximum length in characters for the email input. If you don't include the minimum length or exceed the max length of characters, the browser will show an alert message.

In HTML, form controls, like inputs, can be in different stages or conditions like a focused state, readonly state, or disabled state.

When the user clicks on a form control or selects it with the keyboard's tab key, then that means it is in the focused state. When an input is in the focused state, most browsers will show a blue highlighted border around the input. But you can choose to add additional styles in CSS.

Another form state is the disabled state. This state shows users that an input cannot be focused or activated.
<input disabled type="email" name="email" id="email" />

Another type of form state is the readonly state. This is when a form control, like an input, is not editable by the user. Here is an example of setting an email input to read-only. The value attribute is used to set the value shown inside the input field.

<input
  readonly
  type="email"
  name="email"
  id="email"
  value="example@email.com"
/>

Table
HTML tables aren't used as much these days as they used to be. But, as a front-end developer, you should still be familiar with them. Tables are one of the earliest ways devs had for displaying data in a browser way back in the 1990s.

There's a main table element with an id set to quickfacts

Inside it, the table has a table head element, thead, table body element, tbody, and a table foot element, tfoot.

The table head, body, and foot elements can each contain some number of table rows, tr. And each table row can contain a table header th which labels the data in that row. It can also contain some number of individual data cells, called table data, td.

<table>
  <thead>
    <tr>
      <th>The title of this table</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>First Row</th>
      <td>
        First Data Cell
      </td>
    </tr>
    <tr>
      <th>Second Row</th>
      <td>
        Second Data Cell
      </td>
    </tr>
  </tbody>
  <tfoot>
    <tr>
      <th>The footer of this table, which might contain date of publication, author credits, or other meta information.</th>
    </tr>
  </tfoot>
</table>

Nowadays, developers use CSS flexbox and grid to layout their designs.
