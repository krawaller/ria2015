
###What Redux is

[ReduxJS](http://redux.js.org/) is a (very) small data flow control library. The purpose is to provide a central data storage, and ways to update/query that storage. It does so with a "uni-directional flow", which makes the app very easy to test and reason about.

Redux isn't tied to React, you can use it with pretty much any framework. However, because of the way data flow down the component tree in React, they are a very good match for each other. 

While reading about React you might have come across the term "Flux" - Redux is an alternative to that. If you use Redux in your React app (which we will do in this course), there's no need for a parallel Flux solution.

###Redux in the course

Along with React and React Router, Redux is a mandatory inclusion in your main course project. This means you must store your app state in a Redux store, and use Redux action creators to change that data. 

You do not however have to hook up React Router to Redux, although [there are libraries to do that](https://github.com/rackt/redux-router) if you want to explore it.

Using [Redux-thunk](https://github.com/gaearon/redux-thunk) to be able to do async updates more easily is not mandatory, but recommended. It is used in the demo app.

When you read up on Redux you are likely to come across demonstrations on hot reloading and time travel - we won't force you into that since it requires us to use webpack instead of browserify which is somewhat more convoluted. But if you are interested feel free to go there as it is really neat stuff!

###Learning resources

First off don't miss the [Demo app](../demo-app/) listed under resources here on the course page. It is specially tailored to allow you to grok how Redux works from a real-life example.

Redux has [truly excellent official docs](http://redux.js.org/)!  You can also get [offline version](https://github.com/paulkogel/redux-offline-docs) to print or read on your tablet.

An excellent first step is to watch the speech at React Europe where Redux's creator, Dan Abramov, introduces the library:

<iframe width="560" height="315" src="https://www.youtube.com/embed/xsSnOQynTHs" frameborder="0" allowfullscreen></iframe>

Also check out this brilliant [explanation of Redux in comic format](https://code-cartoons.com/a-cartoon-intro-to-redux-3afb775501a6). No code, just focusing on the high-level stuff.