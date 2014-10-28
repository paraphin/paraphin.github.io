# Paraphin Inc.

We build [responsive][1] [single page apps][2] with Javascript, Node.js, and SASS.

## Software Stack - BREW

* [Backbone.js][3] - a minimal framework that makes single page apps easier to develop
* [React.js][4] - a library that uses JSX to make UI components with very fast data binding
* [Express][5] - Node.js's webapp framework, which organizes the backend very well
* [Webpack][6] - packages assets into optimized bundles to reduce network load

## Workflow

Some of us use [Sublime Text][7], while others use [Atom][8] for text editing. Ben has been working on a cross-platform Sublime plugin to compile SASS files (see [github.com/blitzrk/libsass-build-sublime](https://github.com/blitzrk/libsass-build-sublime)). However, unless you have compilation errors that you're finding hard to debug, webpack handles compiling SASS, so by having a terminal running `webpack --watch --progress --colors` and another running `node server` allows you to have a fully functional local deployment. One catch is that you may need to change the `myHostname` for [everyauth][9].

We like to host on DigitalOcean with a Ubuntu 14.04 droplet. Don't worry about this, though, because we have hooks in place to automate deployment.

## Xoshoal

For the backend, we are using a mix of Redis, MongoDB, and Neo4j for data storage. For the frontend, we are using [Bourbon][10] and [Neat][11] as a SASS framework. For now, we are creating all of our UI elements from scratch.

## Recommended Reading

### Right Away

* [Why Single Page Apps?][2]
* [SPA with Backbone Tutorial](http://code.tutsplus.com/tutorials/single-page-todo-application-with-backbonejs--cms-21417) - you can just skim the view part, because...
* [Using React as Backbone View](http://www.thomasboyt.com/2013/12/17/using-reactjs-as-a-backbone-view.html)
* [Learning React](http://scotch.io/tutorials/javascript/learning-react-getting-started-and-concepts) - save parts 2 and 3 for later
* [Flexbox Cheat Sheet](http://www.sketchingwithcss.com/samplechapter/cheatsheet.html)
* [Solved by Flexbox](http://philipwalton.github.io/solved-by-flexbox/)

### When You're Ready

* [Learning React Part 2](http://scotch.io/tutorials/javascript/build-a-real-time-twitter-stream-with-node-and-react-js) - and [Part 3](http://scotch.io/tutorials/javascript/getting-to-know-flux-the-react-js-architecture)
* [Crazy CSS Stuff to Inspire You](http://tympanus.net/codrops/2013/07/05/using-custom-data-attributes-and-pseudo-elements/) - see also [Scotch.io](http://scotch.io/)'s Codepens of the Week

[1]: https://developers.google.com/web/fundamentals/layouts/rwd-fundamentals/
[2]: http://singlepageappbook.com/goal.html
[3]: http://backbonejs.org/
[4]: http://facebook.github.io/react/
[5]: http://expressjs.com/
[6]: http://webpack.github.io/docs/what-is-webpack.html
[7]: http://www.sublimetext.com/3
[8]: https://atom.io/
[9]: https://www.npmjs.org/package/everyauth
[10]: http://bourbon.io/
[11]: http://neat.bourbon.io/