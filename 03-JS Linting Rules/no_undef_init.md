### No Undef Init
**Error** > In JavaScript, a variable that is declared and not initialized to any value automatically gets the value of `undefined`. For example:

```javascript
var foo;
console.log(foo === undefined);     // true
```
It's therefore unnecessary to initialize a variable to undefined, such as:

```javascript
var foo = undefined;
```