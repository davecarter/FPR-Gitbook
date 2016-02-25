### No Unused Vars
**Warning** > Variables that are declared and not used anywhere in the code are most likely an error due to incomplete refactoring. Such variables take up space in the code and can lead to confusion by readers.

This rule is aimed at eliminating unused variables, functions and variables in parameters of functions, as such, warns when one is found.

A variable is considered to be used when it:

- Represents a function that is called `(doSomething())`
- Is read `(var y = x)`
- Is passed into a function as an argument `(doSomething(x))`
- A variable is not considered read if it is only ever assigned to `(var x = 5)` or declared.

The following pattern are considered problems:

```javascript
var y = 10;   /*error "y" is defined but never used*/
y = 5;
```
