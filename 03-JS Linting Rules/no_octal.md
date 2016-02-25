### No Octal
**Error** > Octal literals are numerals that begin with a leading zero, such as:

```javascript
var num = 071;      // 57
```
The leading zero to identify an octal literal has been a source of confusion and error in JavaScript. ECMAScript 5 deprecates the use of octal numeric literals in JavaScript and octal literals cause syntax errors in strict mode.

It's therefore recommended to avoid using octal literals in JavaScript code.
