### Space-infix-ops
**Error** > Require Spaces Around Infix Operators.

This rule is aimed at ensuring there are spaces around infix operators.

While formatting preferences are very personal, a number of style guides require spaces around operators, such as:

```javascript
var sum = 1 + 2;
```

The proponents of these extra spaces believe it make the code easier to read and can more easily highlight potential errors, such as:

```javascript
var sum = 1+++2;
```

While this is valid JavaScript syntax, it is hard to determine what the author intended.

