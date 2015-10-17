# Webpack Packaging

[Webpack](http://webpack.github.io/docs/) is fast becoming the preferred build and packaging workflow tool for web apps. It is replacing popular build automation tools like [Gulp](http://gulpjs.com/). It competes with JS module bundling tools including [Browserify](http://browserify.org/).

We include Webpack in Rapid App Workflow because of following reasons.

- **Fast.** Webpack optimizes build time using in-memory compiles, production switch, development server, hot-loading, among other features.
- **Saves time.** Combines multiple tools under one roof. Asset pipeline automation, module bundling, ES6 transpile, JSX transform, all rolled into one tool.
- **Less coding.** You write far less lines of code when compared to Gulp or Grunt to do similar tasks.

This of webpack as the glue for our Rapid App Workflow for Web Apps. It is that important.

## Get started with webpack

> **Reference: ** Webpack provides a [basic tutorial](http://webpack.github.io/docs/tutorials/getting-started/) for installing and packaging JS and CSS.

Install webpack.

```
npm install webpack --global
```

Install webpack dev server.

```
npm install webpack-dev-server --global
```

Run webpack showing progress, color coding output, and watching changes.

```
webpack --progress --colors --watch
```

Run webpack dev server.

```
webpack-dev-server --progress --colors
```

> **Note from webpack docs:** The dev server uses webpack’s watch mode. It also prevents webpack from emitting the resulting files to disk. Instead it keeps and serves the resulting files from memory.


## Configure Loaders

Loaders help process different types of web app files including CSS, SASS, JSX, among others. Webpack [lists all the loaders](http://webpack.github.io/docs/list-of-loaders.html) which you can configure as part of your workflow.

### CSS Loaders

Configure CSS loader.

```
npm install css-loader style-loader --save-dev
```

Update ```webpack.config.js``` with css loader.

```
{ test: /\.css$/, loader: "style!css" }
```

Including a css file.

```
require("./style.css");
```

### ES6 Loaders

Babel transpiles ES6 to ES5 for client side code. Babel also transforms React JSX code to JS.

Install Babel loader.

```
npm install babel-loader --save-dev
npm install babel-core --save-dev
```

Update ```webpack.config.js``` with babel loader.

```
{ test: /.jsx?$/, loader: 'babel-loader', exclude: /node_modules/ }
```


## References

1. The [SurviveJS](http://survivejs.com/) Book.

2. [Creating a workflow with webpack](http://christianalfoni.github.io/javascript/2014/12/13/did-you-know-webpack-and-react-is-awesome.html).



*[TODO] This chapter is in progress*
