<img class="toprightimg" src="https://cdn.auth0.com/blog/react-js/react.png"/>

###What React is

The foundation for the main course project is Facebook's [React](http://facebook.github.io/react/) framework. It offers a way to modularise your application into **components**. Each component can be passed **properties** from the parent, and it can also hold some **state** that can be changed. You never have to update anything when properties or state change; a component just needs a **render** function for the initial rendering, and then React will do some behind-the-scenes magic to performantly use that for updates as well!

###Learning resources

There is an excellent [getting started section](https://facebook.github.io/react/docs/getting-started.html) on the main React homepage which we heartily recommend. Prior to going through that this video serves as a good first getting-to-know-React flirt:

<iframe width="560" height="315" src="https://www.youtube.com/embed/x7cQ3mrcKaY" frameborder="0" allowfullscreen></iframe>

To get started yourself we recommend the [course demo app](../demo-app). 

Note that there might also be some React stuff in the snippets list on the [JavaScript resource page](../javascript)

###Using React in the course

As already said your main course project will be built using React, along with [Redux](../redux) for data handling and [React Router](../react-router) for routing.

The reason behind choosing React is that it is a tiny API and thus has a rather low threshold when compared to other frameworks such as [Ember](http://emberjs.com/) or [Angular](https://angularjs.org/). Also, since this course focuses on code organisation and best practices, we don't want to use a framework which answers most such questions for you! And, finally - React is rather brilliant!

