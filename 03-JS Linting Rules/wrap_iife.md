### Wrap-iife
**Error** > Require IIFEs to be Wrapped.

Require immediate function invocation to be wrapped in parentheses.

```javascript
var (x = function () { 
    return { 
        y: 1 
    };
})();
```

Since function statements cannot be immediately invoked, and function expressions can be, a common technique to create an immediately-invoked function expression is to simply wrap a function statement in parentheses. The opening parentheses causes the contained function to be parsed as an expression, rather than a declaration.

