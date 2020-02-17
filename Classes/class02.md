# HTML
## Chapter 2
## Text
there is tow knids of tags in HTML a **semantic** one and a **structural** one the first one is essentially a tag that has meaning   i.e. in english while the structural doesn't represent whats inside it 

#### Example of semantic tags
- form
- article
- aside
- table
#### Example of semantic tags
- h 
- div
- span
- p
# CSS
## Chapter 10
## CSS introduction
CSS display elements on two basis an inline and block; in the inline the content fit inside the space it need while block elements takes the whole width of the screen
to associate a certain style with elements first u should select the element/s by using a selectors followed with declaring the style between curly braces 

## CSS Selectors
to select an element css provides a couple selectors we can use
Selectors|Definition|Expression
-----------|------------|------------
Universal selector|Applies to all elements in the document| * {}
Type Selector|Matches element names|h1, h2, h3 {}
Class Selector|Elements have the same attribute class| .atrributeName{}
Child Selector|element that is a direct child of another|ul>li {}

## Cascading Effects
#### CSS deals with cascading effects on the basis of last rule i.e. the latest style will be applied to the element, specificity that is If one selector is more specific than the others, the more specific rule will be applied lastly by using !important after any property to indicate that it should be considered more important than other rules that apply to the same element

**Note:** its always recommended to use external CSS styling


# JavaScript
## Basic Javascript instruction
first of all JS is a **Case SENSITIVE** language
second writing **comments** is good programming habit by using /* */

* var variableName = 3; **this how to declare a variable and assign value to it**

### Data Types
* numarical data 
* String data 
* Boolean Data

#### use a technique called escaping the quotation characters. This is done by using a backwards slash before any type of quote mark that appears within a string
#### boolean are used when the value is always true or false

## Rules for naming variables
1. must start with a letter, dollarSign and underscore but cant start with a number
2. it can contain the previous and the numbers but must not contain dash or period
3. cnat use reserved words like var
4. case sensitive langauge
5. good habit to give the variable name to indicate its value
6. use standart casing style like camel case

## Arrays
An array is a special type of variable which can store a list of data value, The values are assigned to the array inside a pair of square brackets, and each value is separated by a comma The
values in the array do not need to be the same data type, so you can store a string, a number and a Boolean all in the same array. This technique for creating an array is known as an array literal. It is usually the preferred method for creating an array. You can also write each value on a separate line.
## Expression
there are two type of expressions
Expressions that assign a value to a variable
Expressions that use two or more variable to return a single value

**Note** Expression rely on operators they allow to create a single variable from two or more variables
**Note** addition is the only operators used with string

# Decisions and loops
Programers relys on decision making tools like  and while loops, for loops to name a few.

To make a decision it contain two components a expression and a coniditional statement which Programers relys on to make these decisions like if statement,if-else statement.

## Comparison Operators

comparison operators will return boolean value

some of the comparison operators are
* == which means equal to and compares numbers,srings and boolean values
* != which means is not equal to and compares numbers,srings and boolean values
* === which means strict equal to and compares both data type and value
* !== which means strict not strict equal to and compares both data type and value
## logical operators 
1. And: has && symbol
2. or: with the | symbol
3. Not: which has a ! symbol