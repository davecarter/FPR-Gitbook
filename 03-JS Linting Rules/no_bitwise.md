### No Bitwise
**Allowed** > This rule is aimed at catching typos that end up as bitwise operators, but are meant to be the much more common `&&`, `||`, `<`, `>` operators. As Allowed rule, you must be carefull using them:

```javascript
// Wrong bitwise operator format:
var x = y | z;
var x = y & z;
var x = y ^ z;
var x = y ~ z;

// You should use this format instead:
var x = y || z;
var x = y && z;
var x = y > z;
var x = y < z;
x += y;
```