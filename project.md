Still WIP!


###Getting started

Half of the course is made up by a project, where you will create and iterate on a web app. This app serves as a playground and source of discussion aiming to better your understanding of how to organise a JS RIA.

Before you get down and dirty, make sure you have read up at least some on Git and Github, React, React-Router and Redux! The rest will follow as we go along, but it is good to have at least a vague idea of how things fit together.

To get started you are recommended to simply rip off the [demo app](../demo-app), kick the tyres there so you understand what's going on, then rip my stuff out and replace it with your own.

###Publishing

We will use [Github Pages](../git-and-github) as a publishing platform. This means your project **must** live in the `gh-pages` branch. We recommend you use that as your master branch, and to not use the actual `master` at all.

By employing this approach it is very easy to test each other's projects as we can link them from your guild profiles!


###What to build

So, what should you create? Well, whatever you want! Here are some pointers;
 
*     It must be an app that handles data somehow, it cannot be completely static. However you don't need to use an external database, or even save the data to local storage. But at least during the actual session the user must be able to change something.
*     The scope shouldn't be too ambitious, since we'll be spending times on other things and evaluating our work.
*     ...

###Tools

As stated elsewhere you are forced to use React, React-Router and Redux. If you want to add other libraries apart from those you are most welcome to do so! Also see "sidetracked" below.


###Build process

Because JavaScript doesn't have a native module system (yet), we need to have a build step where we use a tool. This allows us to have a sane code organisation by having modules in separate files, and then calling on those modules without having to put everything in the global scope and use `<script>` tags.

Commonly the build tool will also accomplish other things at the same time. In our case it will compile the React JSX syntax. Other use cases could be to process sass/less css-code, or maybe some other compile-to-JavaScript language such as CoffeeScript, TypeScript or Dart.

In the [demo app project](../demo-app) I'm using Browserify, and to get started it is recommended you simply steal my approach. But if you prefer another build tool such as Webpack you are welcome to use that, but you must still be able to build the project by doing `npm run build` so make sure to set up that correctly.


###Collaboration

You are much encourage to also spend some time in other peoples' code! Doing that is an excellent way to gain perspective into your own choices, and since we're all (because of David's opressive tyrrany) using the same basic tools, the threshold to understand what's going on should be at least somewhat climbable.

Probably the easiest way to explore someone's project is to create a fork of it, and then download that fork locally. Remember to do `npm install` in order to install dependencies (since `node_modules` isn't part of the git repo because it is mentioned in `.gitignore`), and then to run `npm run build` whenever you make any changes.

When you're mucking about in their code, try to find an opportunity to add or improve something and make a pull request! If you do, remember to add it to the guild afterwards to get credit for it (whether it was accepted by the project owner or not)! Here's an example of what the pull requests look like in your `.json` file:

```
{
	"name": "Mattias Wikström",
	// ... other stuff redacted
	"pullrequests": [
		{
			"when": "2015-11-02 14:00",
		    "url": "https://github.com/krawaller/riaguild2015/pull/13",
		    "description": "Added ninja delight! <3"
		},
		{
			"when": "2015-11-03 14:00",
		    "url": "https://github.com/krawaller/riaguild2015/pull/18",
		    "description": "Added DEMONS!"
		}
	]
}
```

As you can see you should add the `url` to the actual pull request made.

Don't forget that the Guild is a very valid target for collaboration, so if you want to make an extra visible contribution, check it out! Although note that the guild is a completely static app and so it doesn't use Redux.


### Getting sidetracked

Unlike in other courses where the final product is what matters, here in the RIA course the journey is the point. This means you have an unpresedented blessing to be sidetracked into other things - as long as it is related to RIA creation with JavaScript, everything goes and it doesn't matter that this siphons time from the actual project. Here are some possible temptations:

*     Unit tests. Trying [test-driven development](http://tddjs.com) will greatly enhance your organisation skills, whether you actually like tests or not!
*     Set up a [Travis build check](http://blog.krawaller.se/posts/travis-ci-and-github-pages/) for your project and play around with the settings!
*     Add a tyrannical JSHint-setting (or JSLint or ESLint or...) for your project, forcing all collaborators to write in your style!
*     Use an online database such as [Firebase](https://www.firebase.com/) (which works supremely well with Redux)
*     Refactoring. Try to change your API, move stuff around, change your data structure, rewrite your app. As long as you document your thoughts, the fact that you're not taking the project forward with regards to features doesn't matter one bit!

