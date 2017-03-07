---
layout: post
title:  "Javascript with npm"
date:   2016-11-20
desc: "A quick overview in setting up a Javascript with npm"
keywords: "javascript,npm,node,linux"
categories: [Linux,Windows]
tags: [Javascript,npm,shell]
icon: fa-terminal
---

The Node Package Manager makes it very easy to start working on projects in Javascript. This will give a quick overview:

1. Open a terminal and create a folder to work in. `mkdir JavascriptProject`
- Run `npm init` to create a `package.json` file and follow the prompts.
- Install some dependencies, eg. `node install chalk`
- Create a `js` file that `"main":` in `package.json` points to, eg. `index.js`
- Make sure to add any dependencies in the `index.js` file, eg. `var chalk       = require('chalk');`
- Add your code to `index.js`, eg.
```js
console.log(
	chalk.yellow('test')
);
```
Lastly run it as: `node index.js`
