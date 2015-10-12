# Setup Web App Environment

Our target platform is NodeJS. We are assuming you are running a developer box on Cloud9. Read more about [Cloud9 code editor](https://manavsehgal.gitbooks.io/rapid-app-workflow/content/cloud9_code_editor.html).

## Custom container

Start with a pre-configured container. Cloud9 offers choices of NodeJS, custom, HTML5, and Meteor stacks for NodeJS development.

![Pre-configured containers in Cloud9](Screen Shot 2015-10-12 at 8.26.21 PM.png)

We choose custom Ubuntu stack. This starts us with a blank file structure and basic target platform pre-installed.

Check versions of NodeJS, npm.

```nvm --version && node --version && npm --version```

This returns installed versions on our Cloud9 container as of this writing (2015 Oct).

```
0.24.1
v0.10.35
1.4.28
```



