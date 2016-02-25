### No Catch Shadow
**Error** > Disallow Shadowing of Variables Inside of catch. In IE 8 and earlier, the catch clause parameter can overwrite the value of a variable in the outer scope, if that variable has the same name as the catch clause parameter.

```javascript
var err = 'x';

try {
    throw "problem";
} catch (err) {  /*error Value of 'err' may be overwritten in IE 8 and earlier.*/
    
    [...]
}
```