# Webpack Packaging

Webpack is fast becoming the preferred build and packaging workflow tool for web apps. It is replacing or complementing popular build tools like Gulp and Grunt.

## Configure Loaders

Loaders help process different types of web app files including CSS, SASS, JSX, among others.

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
