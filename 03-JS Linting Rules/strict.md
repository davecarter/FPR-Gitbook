### Strict
**Allowed** > Strict Mode

A Use Strict Directive at the beginning of a script or function body enables strict mode semantics:

```javascript
'use-strict';
```

When used globally, as in the preceding example, the entire script, including all contained functions, are strict mode code. It is also possible to specify function-level strict mode, such that strict mode applies only to the function in which the directive occurs:

```javascript
function foo() {
    "use strict";
    return;
}

var bar = function() {
    "use strict";
    return;
};
```

This rule is aimed at using strict directives effectively, and as such, will flag any unexpected uses or omissions of strict directives.

