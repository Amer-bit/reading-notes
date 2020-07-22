# 10 Best JavaScript Frameworks

1- AngularJS
2- React
3- Ember.js
4- Vue.js
5- Backbone.js
6- Mithril.js
7- Polymer.js
8- Node.js
9- Meteor.js
10- Aurelia

## CRA vs Next.js vs Gatsby

### Create React App
Create React App is plain simple and it generates HTML code needed to render on the client side. So when you look at the source code before rendering, you can see it’s basically few js files and an empty div. These js files inject content into that div in the browser (Client-side rendering). All heavy lifting is done in the browser.
### Next.js
Next.js a somewhat similar to Create React App, but supports server-side rendering. What it essentially means is that necessary HTML code is generated from the server itself, based on the URL. So your browser is receiving pre-rendered HTML code, not an empty ‘div’.
### Gatsby
While CRA offers client-side rendering and Next.js offers server-side rending, Gatsby is something called “Static Site Generator”. If you’re new to static site generators, those are generators which build “HTML” code during the “build”, by fetching data from some APIs, markdown files or anything. Note that everything is done in the “build” process. Similar to Next.js browser receives pre-rendered HTML code.