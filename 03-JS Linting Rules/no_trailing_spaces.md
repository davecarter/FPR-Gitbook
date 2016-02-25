### No Trailing Spaces
**Error** > Sometimes in the course of editing files, you can end up with extra whitespace at the end of lines. These whitespace differences can be picked up by source control systems and flagged as `diffs`, causing frustration for developers. While this extra whitespace causes no functional issues, many code conventions require that trailing spaces be removed before checkin.

The following patterns are considered problems:

```javascript
var foo = 0;//•••••  /*error Trailing spaces not allowed.*/
var baz = 5;//••     /*error Trailing spaces not allowed.*/
```

In this set of linting rules, the option `skipBlankLines` is set to true. It will not flag any lines that are made up purely of whitespace. In short, if a line is zero-length after being trimmed of whitespace, then the rule will not flag that line when skipBlankLines is enabled.

The following patterns are not considered problems:

```javascript
var foo = 0;
//••••
var baz = 5;
```
