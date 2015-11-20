### Demo app #1

In order to quickly get up to speed with [React](../react), [Redux](../redux) and [React Router](../react-router), we have created a demo app for you to dissect; **Superhero battler 2000**!

![Superhero battler 2000](https://dl.dropboxusercontent.com/u/2287145/lnu/superherobattler.png)

You can run the game [here](http://blog.krawaller.se/riastart2015/), check out the code [here](https://github.com/krawaller/riastart2015) and read a more in-depth blog post [here](http://blog.krawaller.se/posts/a-react-redux-example-app/).

We recommend that you download the code to your own machine so you can learn by changing stuff around and see what happens. Simply...

1.    go to [the git repo](https://github.com/krawaller/riastart2015)
2.    download the zip
3.    unpack it locally
4.    navigate to the folder in the terminal and run `npm install` to download all needed packages
5.    run `npm run build` to create the `bundle.js` file which is actually run by the web app
6.    open `index.html` in a browser! You don't even need a server!

If you yourself change anything in the source code you have to do `npm run build` again to rebuild `bundle.js` before you reload the page, otherwise the same code will be run again.

Of note is that [Andreas](http://blog.krawaller.se/riaguild2015/#/member/afrxx09) made a [simpler version of the app](http://afrxx09.blogspot.se/2015/11/simple-react-redux-example.html), and [Maria](http://blog.krawaller.se/riaguild2015/#/member/mn22nw) wrote up a [good walkthrough of the code](http://mianygren.nu/RIA/Blog/posts-2015/46/#demo-app-a-more-thorough-look).


### Demo app #2

In the second demo app we continue on the above infrastructure but add **Firebase** and **Authentication**. The app also demonstrates how we can keep *all* UI state in Redux, and not have a single piece of state in any component.

![Quotes collector](https://dl.dropboxusercontent.com/u/2287145/lnu/quotesapp.png)

You can try the app [here](http://blog.krawaller.se/reduxfirebasedemo), and the code is [here](https://github.com/krawaller/reduxfirebasedemo).