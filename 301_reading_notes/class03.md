# Javascript Templating Language and Engine— Mustache.js with Node and Express

Javascript templating is a fast and efficient technique to render client-side view templates with Javascript by using a JSON data source. The template is HTML markup, with added templating tags that will either insert variables or run programming logic.

**Mustache**

Mustache is a logic-less template syntax. It can be used for HTML, config files, source code — anything. It works by expanding tags in a template using values provided in a hash or object.
It is often referred to as “logic-less” because there are no if statements, else clauses, or for loops. Instead, there are only tags. Some tags are replaced with a value, some nothing, and others a series of values.
mustache.js is an implementation of the mustache template system in JavaScript. It is often considered the base for JavaScript templating. ***And, since mustache supports various languages, we don’t need a separate templating system on the server side.Mustache is NOT a templating engine. Mustache is a specification for a templating language.***

**Mustache-Express**

If you intend you use mustache with Node and Express, you can use mustache-express. Mustache Express lets you use Mustache and Express together easily.


# Flexbox

The Flexbox Layout aims at providing a more efficient way to lay out, align and distribute space among items in a container, even when their size is unknown and/or dynamic. The main idea behind the flex layout is to give the container the ability to alter its items’ width/height (and order) to best fill the available space (mostly to accommodate to all kind of display devices and screen sizes). A flex container expands items to fill available free space or shrinks them to prevent overflow. Most importantly, the flexbox layout is **direction-agnostic as opposed to the regular layouts and the Grid layout is intended for larger scale layouts.**


**Properties for the Parent:**


1. display: This defines a flex container; inline or block depending on the given value. It enables a flex context for all its direct children.
2. flex-direction: This establishes the main-axis, thus defining the direction flex items are placed in the flex container.
3. flex-wrap
4. flex-flow (Applies to: parent flex container element): This is a shorthand for the flex-direction and flex-wrap properties
5. justify-content : This defines the alignment along the main axis.Note that that browser support for these values is nuanced. For example, space-between never got support from some versions of Edge, and start/end/left/right aren’t in Chrome yet. MDN has detailed charts. **The safest values are flex-start, flex-end, and center.There are also two additional keywords you can pair with these values: safe and unsafe.**
6. align-items: This defines the default behavior for how flex items are laid out along the cross axis on the current line. **Think of it as the justify-content version for the cross axis (perpendicular to the main-axis).** 
7. align-content: This aligns a flex container’s lines within when there is extra space in the cross-axis, similar to how justify-content aligns individual items within the main-axis. Note: this property has no effect when there is only one line of flex items.


**Properties for the Children**

1. Order
2. flex-grow: This defines the ability for a flex item to grow if necessary. Negative numbers are invalid.
3. flex-shrink:This defines the ability for a flex item to shrink if necessary.Negative numbers are invalid.
4. flex-basis: This defines the default size of an element before the remaining space is distributed.
5. flex: This is the shorthand for flex-grow, flex-shrink and flex-basis combined.**It is recommended that you use this shorthand propert**
6. align-self: This allows the default alignment (or the one specified by align-items) to be overridden for individual flex items.
**NOTE: float, clear and vertical-align have no effect on a flex item**
