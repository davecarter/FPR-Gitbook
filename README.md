# Frontend precommit rules for Javascript, SASS and ReactJS

### The main goal of this set of rules is to establish healthy boundaries where cleaner code will be easier to share, more scalable, more readable and easier to maintain for everyone.

![](img/SUI-engineers.png)

----

These linting rules comes preconfigured as a [precommit hook](http://githooks.com/). This means it will not allow you nor anyone in your project to commit to the repository if any of these rules are invalid. Although it might look restrictive in the beginning it offers lots of advantages later on as commented above.

To do so we decided to rely on [Eslint](http://eslint.org/), a great JavaScript linter by [Nicholas C. Zakas](https://twitter.com/slicknet) and [SASS-Lint](https://github.com/sasstools/sass-lint) for... yes! SASS linting.

#### TL;DR
If you are wondering if this set of rules if for you here's a brief description. Keep reading to get a detailed description.

####**Your SASS code must:**
- Merge rules of same selector.
- Set properties to `0` instead of `none`.
- Match the selector format set in the [Naming Convention](#naming-convention)
- ...

####**Your JavaScript code must**
- Be free of alert(), console.log() and Debugger.
- Avoid references to Prototype.
- Use dot notation, camel case and single quotes.
- ...

####**Your ReactJS code must**
- Include just one component per file.
- Always declare expected proptype.
- Use JSX.
- ...


In addition, ES6 syntax is fully supported thanks to BabelJS.

----

## How to install Frontend Pre-Commit Rules in your project:

In your **NodeJS** based project add a dev-dependency as follows:

```javascript
npm i @schibstedspain/frontend-pre-commit-rules --save-dev
```

#### Set a Precommit Hook

Edit your `package.json` file and add the following:

```javascript
  "pre-commit": [
    "lint"
  ],
````

Now NPM will trigger a `lint script` every time you do `git commit -m "my commit rocks"`.

To set up this `lint script` add the following to your `package.json` config file:

```javascript
"scripts": {
    "lint": "npm run lint:eslint && npm run lint:sass",
    "lint:eslint": "eslint --ext=.jsx --ext=js ./src/ ./test/ ./docs/",
    "lint:sass": "scss-lint src/"
}
```

Here we define a `lint` task that will trigger two sub tasks: `npm:eslint` for JavaScript and JSX linting and `lint:sass` for Sass linting.

If you need more information to set up `eslint` or `scss-lint` go to the [Installation](installation.md) chapter:

----

### Contribute to this Open Source project

This Open Source project is maintain by [@SUIEngineers](https://twitter.com/suiengineers).
If you like this project and want to improve it don't hesitate to contribute by opening issues or pull request. In addition **you can show your love just by starring it** Great feedback is always welcome.

<table>
    <tr>
        <td width='10%'><img src='img/GitHub-Mark.png' width='90' /></td>
        <td width='90%'> <a href='https://github.com/SUI-Components/frontend-pre-commit-rules'>Github Repository</a> </td>
    </tr>
    <tr>
        <td width='10%'><img src='img/Npm-logo.png' width='90' /></td>
        <td width='90%'> <a href='https://www.npmjs.com/package/@schibstedspain/frontend-pre-commit-rules'>NPM</a> </td>
    </tr>
</table>