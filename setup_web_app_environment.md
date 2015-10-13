# Setup Web App Environment

Our target platform is NodeJS. We are assuming you are running a developer box on Cloud9. Read more about [Cloud9 code editor](https://manavsehgal.gitbooks.io/rapid-app-workflow/content/cloud9_code_editor.html).

## Custom container

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

As we found more current versions, we will start by updating NVM to latest. Follow [official nvm instructions](https://github.com/creationix/nvm#install-script) for updating using the install script. Note that the version ```v0.29.0``` mentioned here will change to latest release.

```
curl -o- https://raw.githubusercontent.com/creationix/nvm/v0.29.0/install.sh | bash
```

Next we follow [Cloud9 docs](https://docs.c9.io/docs/updating-nodejs) to update node using nvm.

```nvm install 4.1.2```

We complete the node environment setup by updating npm. [npm GitHub issue](https://github.com/npm/npm/issues/1840) on the subject and [stackoverflow top answer](http://stackoverflow.com/questions/23393707/how-to-update-npm) suggest a solution for updating npm.

```npm install npm -g```




