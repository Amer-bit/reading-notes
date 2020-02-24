# Tables (126-145)

In this chapter you will learn how to:
* Use the four key elements for creating tables
* Represent complex data using tables
* Add captions to tables

### Table Declration
The \<table> element is used to create a table. The contents of the table are written out row by row. 

You indicate the **start of each row** using the opening <tr> tag.(The tr stands for table row.)
I**it is followed by one or more <td> elements **(one for each cell in that row). **At the end** of the row you use a closing </tr> tag.

### Table Heading

The <th> element is used just like the /<td> element but its purpose is to represent the heading for either a column or a row. (The th stands for table heading.)

You can use the scope attribute on the /<th> element to indicate whether it is a heading for a
column or a row. It can take the values: row to indicate a heading for a row or col to indicate a heading for a column.
 
 we can **Span Coloumn and Rows**  using colspan nad rowspan attributes and they are used on th or td tags

 There are three elements that help distinguish between the main content of the table and the first and last rows (which can contain different content). These elements help people who use screen readers and also allow you to style these sections in a different manner than the rest of the table whcich are:
 * /<thead>: The headings of the table should sit inside the /<thead> element.
 * /<tbosy>: The body should sit inside the /<tbody> element.
 * /<tfoot>: The footer belongs inside the /<tfoot> element.

 **Wecan also change the width, spacing, border and background of the table

 # Js Function and methods
 