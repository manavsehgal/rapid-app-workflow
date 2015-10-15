# Webpack Packaging

Webpack is fast becoming the preferred build and packaging workflow tool for web apps. It is replacing or complementing popular build tools like Gulp and Grunt and JS module bundling tools like browserify.

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




*[TODO] This chapter is in progress*
