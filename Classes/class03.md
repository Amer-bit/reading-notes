# Lists
HTML include three different list types:
* Ordered lists using ol tag followed by li tag
* Unordered lists using ul tag followed by li tag
* Definition lists using dl tag followd by dt to contain the title definition followed by dd wich contain the definition

**Note:** In lists there can be Nested list

# Boxes
boxes is one of the most important feature to learn in CSS it gives us the ability to control the dimension of inline and block level elements.

## height,width 
So by default the box is big enough just to hold the content inside it but we can control the dimension of a box by using 
* height
* width

## max/min height and width
limiting the width and the height of a box is done by using max-height or width, min-height or width and its better practice to use percentage values to determine their values because  the user could be using small or bigger screen and the percentage value ensure that the box fit everywhere

## overflow
overflow property tells the browser what to do if the content contained within a box is larger than the box itself. It can have one of two values:
* hidden This property simply hides any extra content that does not fit in the box.
* scroll This property adds a scrollbar to the box so that users can scroll to see the missing content.

## Border, Margin, Padding
Every box has three available properties that can be adjusted to control its appearance a border ,margin, padding

**Note:** If you specify a width for a box, then the borders, margin, and padding are added to its width and height.

**Border**

The border separates the edge of one box from another.we can style border using border-style and the width can be controlled usig border-width and to control the color we use border color and these some we can group into one order which is border:width style color;

**Padding**

The padding property allows you to specify how much space should appear between the content of an element and its border.The value of this property is most often specified in pixels we can we can specify values to the top, right, bottom, left of the padding 

**Margin**

The margin property controls the gap between boxes. Its value is commonly given in pixels If one box sits on top of another,
margins are collapsed, which means the larger of the two margins will be used and the smaller will be disregarded.
If the width of a box is specified then the margin is added to the width of the box. we specify values to the top, right, bottom, left of the margin

**Centering Content**
If you want to center a box on the page (or center it inside the element that it sits in), you can set the ***left-margin and right-margin to auto***.In order to center a box on the page, **you need to set a width for the box** (otherwise it will take up the full width of the page). Specifing the width of the box and then setting the left and right margins to auto will make the browser put an equal gap on each side of the box

**Changing display type:** The four types of diplaying can be changed which are block, inline, inline-block, none like we can change inline level element into a block level element and vise verca.

**Note**If you do not want a blank space to appear, then you should use the display property with a value of none.


Also the **visiblity** of the box can be controlled using visibility: hidden or visible

other properties can be controlled using CSS like image-border, box-shadow, border-raduis

border-raduis can create simple rounded corner or more complex shape by specifing the horizantal and vertical distance


# JS
## Switch statement
switch syyntax:
switch(condition) {
    
    case ():
    //Block of code;
    break;
    
    case ():
    //Block of code;
    break;
    
    default:
    //Block of code
    break;
}
Each case indicates a possible value for this variable and the code that should run if the variable matches that value if none of the cases is exeuted the default value will be executed.

**JS type correction and weak typing**
js is **weak typing language** which means that data type for a value can change other languages are strong typing language requires specifing what data type each variable will be. So JS convert data types behind the scenes to complete an operation. Type correction can lead to **unexpected error** so it's better to use strict equal or not equal in comparison operation

# Loops
the most faomus loops are while, do while, for loops. Any loop contain **intializing element, condition and a update or in other words a counter**


**key loop concepts**
* keywords used for loops are **continue and break**
* loops are very useful with arrays it can be used to check every elemnt of the array
* Js will affect the performance of the webpage when a browser comes across JavaScript, it will stop doing anything else until it has   processed that script ***Be CAREFUL of INFINTE LOOPS***

