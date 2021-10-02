# node-mongo CLI

![npm version](https://badge.fury.io/js/%40code-collabo%2Fnode-mongo-cli.svg) ![NPM Downloads](https://img.shields.io/npm/dy/@code-collabo/node-mongo-cli?color=blue) ![contributions welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat) ![License: ISC](https://img.shields.io/badge/License-ISC-blue.svg) ![GitHub issues](https://img.shields.io/github/issues/code-collabo/node-mongo-cli?color=red) ![GitHub pull requests](https://img.shields.io/github/issues-pr/code-collabo/node-mongo-cli?color=goldenrod)

**Supported node versions:** node v12.x to v16.x

The **node-mongo** project has 3 main projects:

* The node-mongo CLI to bootstrap boilerplate templates.
* 3 boilerplate templates for nodejs and/or mongoDB development.
* Demo CRUD app to test connection and show example usage of the templates.

## CLI Features

![node-mongo](https://github.com/Ifycode/Ifycode/blob/main/code-collabo/node-mongo-cli.gif?raw=true)

* CLI bootstraps the esm, cjs or ts templates for nodejs and/or mongoDB development.
* Install dependencies and intialize git for the template bootstrapped or choose to skip them.
* Folders are automatically created based on user entry in prompt or command-line.
* Default folder name is provided and incremented if name already exists.

## **CLI Installation**

Install **node-mongo-cli** globally with this command:

```text
npm install -g @code-collabo/node-mongo-cli
```

## Command

After installing globally, use the node-mongo command.

```text
node-mongo
```

### Usage

```text
node-mongo <folder_name> <template>
```

### Usage example

The example below will bootstrap the cjs template i.e. the common js template into a folder named test-folder.

```text
node-mongo test-folder cjs
```

### Flags

```text
-h, --help          Show help
-i, --install       Install dependencies
-g, --git           Initialize git repo
-s, --skip-install  Skip installing dependencies
-x, --skip-git      Skip initializing git
-y, --yes           See note on --yes flag below
```

### Prompts

If you do not specify one or both arguments above, you will be prompted to add your folder name and/or choose template option from list. For folder name, you can choose to use the default folder name provided in the prompt or type in your preferred folder name.

### Skip prompts

No prompt when --yes flag is used. It skips both install and git init, and uses esm template as default if no template is specified or if template entered is not in the template collection. In the case of folder name, default folder name is used if no folder name is specified or when folder name already exists.
