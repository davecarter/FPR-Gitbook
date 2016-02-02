### Linter installation

Before using this plugin, you must ensure that `sass-lint` is installed on your system. To install `sass-lint`, do the following:

````
$ npm install -g sass-lint
````

**Note**: This plugin requires sass-lint 1.2.0 or later. Check your version with:
````
$ sass-lint --version.
````


### Step 4 - Install SASS Linting plugin

- Open Package control in Sublime Text by typing: `cmd + shift + p` and then search for `install package`

![](../img/package-control.png)

- Select `SublimeLinter-contrib-sass-lint` to install it.
- Reopen Sublime Text if necessary.
- SASS linting rules must be defined in a `.sass-lint.yml` file in the root directory.
