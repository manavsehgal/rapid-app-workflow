# Webpack Packaging

Webpack is fast becoming the preferred build and packaging workflow tool for web apps. It is replacing or complementing popular build tools like Gulp and Grunt.

# Configure Loaders

Add CSS loader.

```
npm install css-loader style-loader
```

Update ```webpack.config.js``` with css loader.

```
{ test: /\.css$/, loader: "style!css" }
```


*[TODO] This chapter is in progress*
