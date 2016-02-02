# Developer environment Installation
This document is a step by step guide to add a development environment to work using JS, SASS and React linting in **Sublime Text 3**. Feel free to use the code editor of your choice. Just make sure you can add *Eslint*, *SASS-Lint* and *Editorconfig* features.

### Installing Node
![NodeJS](img/nodejs.png)

Download the LTE version of NodeJS from Node website and follow installer instructions. Besides, you might want to install Node Version Manager (NVM) too.

### NodeJS via NVM

We strongly recommend using Node Version Manager to avoid versioning hassle.
To install NVM open your terminal and type:

````
curl -o- https://raw.githubusercontent.com/creationix/nvm/v0.30.2/install.sh | bash

````

#### Working with NVM

Currently the most stable NodeJS version is 4.2. To add it to NVM type:

````
nvm install v4.2
````

List all your installed versions of NodeJS:

````
nvm list
````

Using an specific version:

````
nvm use v4.2
````

Setting an alias:

````
nvm alias default 4
$ default -> 4 (-> v4.2)
```


If you need further information visit [NVM GitHub Page](https://github.com/creationix/nvm).

---

### Updating NPM

<img src='img/Npm-logo.png' width='150' />

NPM stands for Node Package Manager. Is a good practice updating NPM after installing Node the first time:


```
$ sudo npm install npm -g
```

Test your NPM version:

```
$ npm --version
```

By the time of this publication current version is 3.3.12










