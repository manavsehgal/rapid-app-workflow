# Setup Web App Environment

Setting up the developer environment is one of the most crucial steps in your web app workflow. 

In this chapter we will achieve the following goals.

- Select an appropriate pre-installed container at Cloud9.
- Update node environment to latest releases.

## Environment assumptions

Our target platform is NodeJS. We are assuming you are running a developer box on Cloud9. Read more about [Cloud9 code editor](https://manavsehgal.gitbooks.io/rapid-app-workflow/content/cloud9_code_editor.html).

## Choose custom container

Start with a pre-configured container. Cloud9 offers choices of NodeJS, custom Ubuntu, HTML5, and Meteor stacks for NodeJS development.

We choose custom Ubuntu stack. This starts us with a blank file structure and basic target platform pre-installed.

## Check versions for Node environment

Check versions of NVM (Node Version Manager), NodeJS, and npm (Node Package Manager).

```nvm --version && node --version && npm --version```

This returns installed versions on our Cloud9 container as of this writing (2015 Oct).

```
0.24.1
v0.10.35
1.4.28
```

Check latest versions by visiting GitHub releases page for [NVM](https://github.com/creationix/nvm/releases), [NodeJS](https://github.com/nodejs/node/releases), and [NPM](https://github.com/npm/npm/releases).

## Upgrade node environment

As we found more current versions, we will start by updating NVM to latest. Follow [official nvm instructions](https://github.com/creationix/nvm#install-script) for updating using the install script. Note that the version ```v0.29.0``` mentioned here will change to latest release.

```
curl -o- https://raw.githubusercontent.com/creationix/nvm/v0.29.0/install.sh | bash
```

Next we follow [Cloud9 docs](https://docs.c9.io/docs/updating-nodejs) to update node using nvm.

```nvm install 4.1.2```

Your developer environment may have multiple versions of node installed. To ensure we always use the latest we run the following command.

```nvm alias default 4.1.2```

And the result.

![Result of running nvm alias](Screen Shot 2015-10-13 at 9.53.32 AM.png)

We complete the node environment setup by updating npm. [npm GitHub issue](https://github.com/npm/npm/issues/1840) on the subject and [stackoverflow top answer](http://stackoverflow.com/questions/23393707/how-to-update-npm) suggest a solution for updating npm.

```npm install npm -g```

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

- ES6 features that node compiles by default, no runtime flags required.
- Basic node server.
 


TODO: This section is in progress
