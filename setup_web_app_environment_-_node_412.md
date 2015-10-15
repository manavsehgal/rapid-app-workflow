# Setup Web App Environment - Node 4.1.2

> We are facing issues using popular npm packages on Node.js 4.1.2 as on 2015-Oct. This chapter is in archive for future release and updates. 

## Upgrade node environment

As we found more current versions, we will start by updating NVM to latest. Follow [official nvm instructions](https://github.com/creationix/nvm#install-script) for updating using the install script. Note that the version ```v0.29.0``` mentioned here will change to latest release.

```
curl -o- https://raw.githubusercontent.com/creationix/nvm/v0.29.0/install.sh | bash
```

Next we follow [Cloud9 docs](https://docs.c9.io/docs/updating-nodejs) to update node using nvm.

```
nvm install 4.1.2
```

Your developer environment may have multiple versions of node installed. To ensure we always use the latest we run the following command.

```
nvm alias default 4.1.2
```

And the result.

![Result of running nvm alias](Screen Shot 2015-10-13 at 9.53.32 AM.png)

We complete the node environment setup by updating npm. [npm GitHub issue](https://github.com/npm/npm/issues/1840) on the subject and [stackoverflow top answer](http://stackoverflow.com/questions/23393707/how-to-update-npm) suggest a solution for updating npm.

```
npm install npm -g
```

We check latest versions again as on 2015-Oct.

```
0.29.0
v4.1.2
3.3.6
```

Done! Our node environment is setup with latest versions.

**Note:** You will notice that node and npm major versions have jumped. This is because node is now following Semantic Versioning. [Official release](https://nodejs.org/en/blog/release/v4.0.0/) explains the significance of this change.

## Test node environment

Let us develop a basic testing strategy for our new node environment.

- [ES6 features](https://nodejs.org/en/docs/es6/) which Node.js now compiles by default. No run-time flags required.

### Default ES6 features

Create ```es6-default.js``` and copy following code.

```javascript
var myMap = new Map();
myMap.set(0, "zero"); myMap.set(1, "one");

console.log("Collections: Map");

myMap.forEach(function(value, key) {
  console.log(key + " = " + value);
}, myMap)

```

Run this ES6 sample.

```
node es6-default
```

Success if following result displays in console.

```
0 = zero
1 = one
```
