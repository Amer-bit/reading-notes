# React Concept: Composition
In programming, composition allows you to build more complex functionality by combining small and focused functions.

In React, composition allows you to have some pretty cool advantages.

You create small and lean components and use them to compose more functionality on top of them. Depending on how generalized these components are, they can be used in building many other components.

## Specialized Components
A specialized component is a generic component that accepts props that are used to render a specialized version.

## Container Components
In many cases, a specialized component will suffice, however, a drawback to using this pattern with some components is that it assumes that all components will be displayed in the same format

All React components have a special children prop so that consumers can pass components directly by nesting them inside the jsx.

## Component Composition - Logical
In this setup, you are sending your child components the raw data and allowing them to render the output as they decide.

## Component Composition - Using Logic-less Children
This is typically used when your children are already in JSX form (pre-rendered) and you need to display them as a whole. A good example might be a gallery of images


### props.children
 It is used to display whatever you include between the opening and closing tags when invoking a component.