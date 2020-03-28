# Responsive Web Design

Responsive web design is the practice of building a website suitable to work on every device and every screen size

## Responsive vs. Adaptive vs. Mobile

Responsive and adaptive web design are closely related, and often transposed as one in the same. Responsive generally means to react quickly and positively to any change, while adaptive means to be easily modified for a new purpose or situation, such as change. With responsive design websites continually and fluidly change based on different factors, such as viewport width, while adaptive websites are built to a group of preset factors. A combination of the two is ideal, providing the perfect formula for functional websites.Mobile, on the other hand, generally means to build a separate website commonly on a new domain solely for mobile users. While this does occasionally have its place, it normally isn’t a great idea. Mobile websites can be extremely light but they do come with the dependencies of a new code base and browser sniffing, all of which can become an obstacle for both developers and users.

## Responsive design components

**Flexible layouts**
**Flexible media**
**media queries**

### Flexible layouts

flexible layouts, is the practice of building the layout of a website with a flexible grid, capable of dynamically resizing to any width. Flexible grids are built using relative length units, most commonly percentages or em units or  vw, vh, vmin, and vmax units in CSS3. These relative lengths are then used to declare common grid property values such as width, margin, or padding.

***Note:*** to build flexibl layout the later formula is used taget/context

**Taking the flexible layout concept, and formula, and reapplying it to all parts of a grid will create a completely dynamic website, scaling to every viewport size. For even more control within a flexible layout, you can also leverage the min-width, max-width, min-height, and max-height properties.**

The flexible layout approach alone isn’t enough. At times the width of a browser viewport may be so small that even scaling the the layout proportionally will create columns that are too small to effectively display content. Specifically, when the layout gets too small, or too large, text may become illegible and the layout may begin to break. In this event, media queries can be used to help build a better experience


### Media Queries

Media queries were built as an extension to media types commonly found when targeting and including styles. Media queries provide the ability to specify different styles for individual browser and device circumstances, the width of the viewport or device orientation for example. Being able to apply uniquely targeted styles opens up a world of opportunity and leverage to responsive web design.

**Initializing Media Queries**

There are a couple different ways to use media queries, using the @media rule inside of an existing style sheet, importing a new style sheet using the @import rule, or by linking to a separate style sheet from within the HTML document. Generally speaking it is recommend to use the @media rule inside of an existing style sheet to avoid any additional HTTP requests.

Each media query may include a media type followed by one or more expressions. Common media types include all, screen, print, tv, and braille. The HTML5 specification includes new media types, even including 3d-glasses. Should a media type not be specified the media query will default the media type to screen.

**Logical operators in media queries**

Logical operators in media queries help build powerful expressions. There are three different logical operators available for use within media queries, including and, not, and only.

Omitting a Media Type when using the not and only logical operators the media type may be left off. In this case the media type is defaulted to all.

***Media Features in Media Queries***

Height & Width Media Features
Using Minimum & Maximum Prefixes
Orientation Media Feature
Aspect Ratio Media Features
Pixel Ratio Media Features
Resolution Media Feature
Other Media Features:
Other media features include identifying available output colors with use of the color, color-index, and monochrome features, identifying bitmap devices with the grid feature, and identifying the scanning process of a television with the scan feature. These features are less common but equally as helpful when needed.

**Media Query Browser Support**
Unfortunately media queries do not work within Internet Explorer 8 and below, as well as other legacy browsers. There are, however, a couple suitable polyfills written in Javascript.

**Respond.js** is a lightweight polyfill that only looks for min/max-width media types, which is perfect should those be the only media query types used. 
**CSS3-MediaQueries.js** is a more developed, and heavier, polyfill offering support for a larger array of more complex media queries. Additionally, keep in mind any polyfill can have performance concerns, and potentially slow down websites. Make sure that any given polyfill is worth the performance trade off.