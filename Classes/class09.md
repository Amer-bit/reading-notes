# Forms (144-175)

There are several types of form controls that you can use to collect information from visitors to your site.

1. **Adding Text**

* Text input for single line like name
* password input
* Text input area for multiple line entry

2. **Making Choice**

* Radio button to select one option
* Check box to select or unselect multiple option
* Drop downsWhen a user must pick one of a number of options from a list

3. **Submiting forms**

* Submit buttons To submit data from your form to another web page.
* Image buttons Similar to submit buttons but they allow you to use an image.

4. **Uploding files**

* Allows users to upload files (e.g. images) to a website

## How forms works
A user fills in a form and then presses a button to submit the information to the server. The server creates a new page to send back to the browser based on the information received.

## Form Structure

**form**

Form controls live inside a \<form> element. This element should always carry the action attribute and will usually have a method and id attribute too.

**action**

Every \<form> element requires an action attribute. Its value is the URL for the page on the
server that will receive the information in the form when it is submitted.

**method**

Forms can be sent using one of two methods: get or post. With the get method, the values from the form are added to the end of the URL specified in the action attribute. The get
method is ideal for:
* short forms (such as search boxes)
* when you are just retrieving data from the web server (not sending information that
should be added to or deleted from a database)
With the post method the values are sent in what are known as HTTP headers. As a rule of thumb you should use the post method if your form:
* allows users to upload a file
* is very long
* contains sensitive data (e.g. passwords)
* adds information to, or deletes information from, a database

If the method attribute is not used, the form data will be sent using the get method.

**ID**
This value is used to identify the form distinctly from other elements on the page (and
is often used by scripts — such as those that check you have entered information into fields
that require values).

Ways of entring data to a form:
* Text input
* Password input
* Text area
* Radio button
* Check box
* Dropdown list
* Multiple select box
* File input box
* Submit Button
* Image button
* Button and hidden control
* Labeling form controls
* Grouping form elements

**We can determine the type of data that the user should input and have some kind of ***VALIDATION***

# List, Table and Forms (330-357)

**List style type**
Unordered lists styling : none, Disk, Circle, Square
Ordered list stylng: decimal, decimal-leading-zero, lower-alpha, upper-alpha, lower-roman, upper-roman

**List-style-image**:You can specify an image to act as a bullet point using this property
This property can be used on rules that apply to the <\ul> and <\li> elements.

**List postioning(List-style-position)**: Lists are indented into the page by default and the list-styleposition property indicates whether the marker should appear on the inside or the outside of the box containing the main points.


**List shorthand(ListList-style)**: As with several of the other CSS properties, there is a property that acts as a shorthand for list styles. It is called list-style, and it allows you to express the markers' style, image and position properties in any order.

**Table properties p.337** 

**border on empty cell (empty-cells)**: If you have empty cells in your table, then you can use
the empty-cells property to specify whether or not their borders should be shown. it hold the one of these values hide, show and inherit

**gaps between cells (border-spacing,border-collapse)**


## Styling Forms

**styling text input**
**styling submit button**
**styling fieldset and legends**
**Aligning Form Controls: Problem and solutions**
**curson style**


## Events (243-292)