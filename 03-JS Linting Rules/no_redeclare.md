### No Redeclare
**Error* > In JavaScript, it's possible to redeclare the same variable name using `var`. This can lead to confusion as to where the variable is actually declared and initialized.

This rule is aimed at eliminating variables that have multiple declarations in the same scope.

The following pattern in considered a problem:

```javascript
var a = 3;
var a = 10; /*error "a" is already defined*/
```

