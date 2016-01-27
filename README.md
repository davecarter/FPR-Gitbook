# Frontend precommit rules for Javascript, SASS and ReactJS

### The main goal of this set of rules is to establish healthy boundaries where cleaner code will be easier to share, more scalable, more readable and easier to maintain for everyone.

![](img/SUI-engineers.png)

----

These linting rules comes preconfigured as a [precommit hook](http://githooks.com/). This means it will not allow you nor anyone in your project to commit to the repository if any of these rules are invalid. Although it might look restrictive at the beginning offers many advantages later on as commented above.

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


In addition, ES6 syntax is fully supported thanks to BabelJS. Feel free to use the right transpiling level for your project. Set the [right value](https://babeljs.io/docs/usage/babelrc/) in `.babelrc` config file.

----

This Open Source project is maintain by [@SUIEngineers](https://twitter.com/suiengineers).

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