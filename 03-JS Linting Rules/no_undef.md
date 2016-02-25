### No Undef
**Error** > Any reference to an undeclared variable causes a warning, unless the variable is explicitly mentioned in a `/*global ...*/` comment. This rule can help you locate potential ReferenceErrors resulting from misspellings of variable and parameter names, or accidental implicit globals (for example, from forgetting the `var` keyword in a `for` loop initializer).

```javascript
var a = someFunction();  /*error "someFunction" is not defined.*/
b = 10;                  /*error "b" is not defined.*/
```

Explicitly checking an undefined identifier with typeof causes no warning:

```javascript
if (typeof UndefinedIdentifier === "undefined") {
    // do something ...
}
```