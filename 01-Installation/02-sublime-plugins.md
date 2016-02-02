### Step 2 - Install Sublime Linting Plugins

SublimeLinter is a plugin for Sublime Text 3 that provides a framework for **linting code**.

Whatever language you code in, **SublimeLinter** can help you write cleaner, better, more bug-free code. SublimeLinter has been designed to provide maximum flexibility and usability for users and maximum simplicity for linter authors.

**SublimeLinter does not do the linting itself**; it acts as a host for linting plugins. The linting plugins themselves usually do not perform linting either; they just act as a bridge between the code you type in Sublime Text and the actual linter.

Note that SublimeLinter is not limited to a single linter plugin per syntax — you are free to install multiple linter plugins for a syntax, and all of them will run when you edit a file in that syntax.

In addition, SublimeLinter supports multiple syntaxes in a single file, which is common when editing HTML. For example, a single HTML file may contain embedded CSS, JavaScript, and PHP. SublimeLinter will lint all of the embedded code using the appropriate linter plugin.

- Open Package Control and install: `SublimeLinter` [Sublime Linter Plugin](http://www.sublimelinter.com/en/latest/).

