### About SublimeLinter

SublimeLinter is a plugin for Sublime Text 3 that provides a framework for **linting code**.

Whatever language you code in, **SublimeLinter** can help you write cleaner, better, more bug-free code. SublimeLinter has been designed to provide maximum flexibility and usability for users and maximum simplicity for linter authors.

**SublimeLinter does not do the linting itself**; it acts as a host for linting plugins. The linting plugins themselves usually do not perform linting either; they just act as a bridge between the code you type in Sublime Text and the actual linter.

Note that SublimeLinter is not limited to a single linter plugin per syntax — you are free to install multiple linter plugins for a syntax, and all of them will run when you edit a file in that syntax.

In addition, SublimeLinter supports multiple syntaxes in a single file, which is common when editing HTML. For example, a single HTML file may contain embedded CSS, JavaScript, and PHP. SublimeLinter will lint all of the embedded code using the appropriate linter plugin.

### Step 2 - Install Sublime Linter

To install SublimeLinter via Package Control, follow these steps:

- Open the Command Palette `cmd+shift+p` on Mac OS X, `ctrl+shift+p` (on Linux/Windows).
- Type install and select Package Control: Install Package from the Command Palette. There will be a pause of a few seconds while Package Control finds the available packages.
- When the list of available packages appears, type linter and select SublimeLinter. Note: The github repository name is “SublimeLinter3”, but the plugin name remains “SublimeLinter”.
- After a few seconds SublimeLinter will be installed and loaded. Depending on your setup, you may see some prompts from SublimeLinter. For more information on SublimeLinter’s startup actions, see Startup actions.
- You will see an install message. After reading the message, restart Sublime Text 3.


