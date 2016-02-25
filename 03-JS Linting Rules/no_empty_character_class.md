### No Empty Character Class
**Error** > Empty character classes in regular expressions do not match anything and can result in code that may not work as intended.

This rule is aimed at highlighting possible typos and unexpected behavior in regular expressions which may arise from the use of empty character classes.

The following pattern is considered a problem:

```javascript
var foo = /^abc[]/;
/^abc[]/.test(foo);
```