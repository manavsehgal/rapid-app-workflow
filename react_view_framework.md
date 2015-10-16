# React View Framework

Facebook and Instagram teams have released their view framework called [React](http://facebook.github.io/react/). React encourages component oriented UI development. This in turn improves re-usability, maintainability, and performance of your code.

## Hello world components

We will use ES6 features [2] to define React components as JavaScript classes.

Create ```\front\hello.js``` file. This is your first React component.

```
import React from 'react';
 
class Hello extends React.Component {
  render() {
    return <h1>Hello</h1>
  }
}

React.render(<Hello/>, document.getElementById('hello'));
```


## References

1. Twilio's 2015-Aug post on [Setting up React for ES6 with Webpack and Babel](https://www.twilio.com/blog/2015/08/setting-up-react-for-es6-with-webpack-and-babel-2.html). Concise introduction to the workflow setup. Also introduces ES6 based React programming, which is cleaner approach.

2. The official [React blog post on release v0.13.0](https://facebook.github.io/react/blog/2015/01/27/react-v0.13.0-beta-1.html) introducing ES6 and ES7 features supported by react. These include classes and properties.

3. The [latest React release v0.14.0](https://facebook.github.io/react/blog/2015/10/07/react-v0.14.html) has major enhancements which the blog post discusses. These include deprecation of react-tools in favor of Babel for JSX transform to JavaScript.

4. Video on [React Hot Loader](https://vimeo.com/100010922) and [getting started](http://gaearon.github.io/react-hot-loader/getstarted/) with React Hot Loader. [React Hot Bolilerplate](https://github.com/gaearon/react-hot-boilerplate) on GitHub.

5. [Thoughtbot tutorial](https://robots.thoughtbot.com/setting-up-webpack-for-react-and-hot-module-replacement) on React Hot Loader.

6. [JMFurlott tutorial](http://jmfurlott.com/tutorial-setting-up-a-single-page-react-web-app-with-react-router-and-webpack/) on React Router.

7. Tutorial on setting up [SASS](http://www.jonathan-petitcolas.com/2015/05/15/howto-setup-webpack-on-es6-react-application-with-sass.html).

8. [React and ES6](http://babeljs.io/blog/2015/06/07/react-on-es6-plus/).

9. [Refactoring from ES5 to ES6 for React](http://www.newmediacampaigns.com/blog/refactoring-react-components-to-es6-classes).