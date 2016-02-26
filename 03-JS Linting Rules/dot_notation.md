### Dot Notation
**Error** > In JavaScript, one can access properties using the `dot` notation `foo.bar` or square-bracket notation `foo["bar"]`. However, the `dot` notation is often preferred because it is easier to read, less verbose, and works better with aggressive JavaScript minimizers.

This rule is aimed at maintaining code consistency and improving code readability by encouraging use of the dot notation style whenever possible. As such, it will throw an error when it encounters an unnecessary use of square-bracket notation.

The following patterns are considered problems:

```javascript
var x = foo["bar"]; /*error ["bar"] should be written in dot notation.*/
```
