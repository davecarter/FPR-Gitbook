
### Indentation

Default basic indentation is set to the followind value:

- Indentation 2 spaces.

##### Use Editorconfig instead

In the other hand, automatic **indentation** can be performed by Editorconfig to ensure a consistent coding style no matter what editor or IDE you use. Consists of a hidden file named `.editorconfig` and a plugin that needs to be installed in your code editor.

Also helps Github diffing tool to avoid incorrect file changes. The presets included in Editorconfig are:

- `[*]` - Applies the following rules to **all characters in files**.
- `indent_style = space` - Use *soft tabs* for indentation.
- `indent_size = 2` - 2 columns are used for each indentation.
- `end_of_line = lf` - Line ending are set to *line feed*
- `charset = utf-8` - Character encoding is set to utf-8.
- `trim_trailing_whitespace = true` - Whitespace preceding new lines is removed.
- `insert_final_newline = true` - An empty new line at the end of every file must to be added.

Markdown files has the following rule redefined:

- `indent_size = 4` - 4 columns are used for each indentation.

Make sure you install the right plugin for your code editor. Check out the [EditorConfig](http://editorconfig.org/#download) website to get the right one.

If you are using **Sublime Text**:

- open Package Control.
- Type `EditorConfig` .
- Press `enter` to Install it.