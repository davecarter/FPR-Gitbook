### Comma Dangle
**Error** > Trailing commas in object literals are valid according to the ECMAScript 5 (and ECMAScript 3!) spec. On the other hand, trailing commas simplify adding and removing items to objects and arrays, since only the lines you are modifying must be touched.

This rule enforces consistent use of trailing commas in object and array literals.
The following patterns are considered problems:

```javascript
var foo = {
    bar: "baz",
    qux: "quux",   /*error Unexpected trailing comma.*/
};

var arr = [1,2,];  /*error Unexpected trailing comma.*/
```
