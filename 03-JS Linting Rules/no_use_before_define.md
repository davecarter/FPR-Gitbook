### No Use Before Define
**Error** > In JavaScript, prior to ES6, variable and function declarations are hoisted to the top of a scope, so it's possible to use identifiers before their formal declarations in code. This can be confusing and some believe it is best to always declare variables and functions before using them.

In ES6, block-level bindings (let and const) introduce a "temporal dead zone" where a `ReferenceError` will be thrown with any attempt to access the variable before its declaration.

The following pattern is considered a problem:

```javascript
var a;
a = 10;
alert(a);
```
Due to the parameter `no-func` of this rule set to `true`, the following pattern is **not** considered a problem:

```javascript
f();            /*is NOT an error even if it was used before being defined*/
function f(){
    // code
}
```
