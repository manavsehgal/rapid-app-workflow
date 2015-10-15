# Webpack Packaging

Webpack is fast becoming the preferred build and packaging workflow tool for web apps. It is replacing or complementing popular build tools like Gulp and Grunt.

# Configure Loaders

Configure CSS loader.

```
npm install css-loader style-loader
```

Update ```webpack.config.js``` with css loader.

```
{ test: /\.css$/, loader: "style!css" }
```

Include a css file in the ```entry.js```.

```
require("./style.css");
```


*[TODO] This chapter is in progress*
