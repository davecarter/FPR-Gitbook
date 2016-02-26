### Key-spacing
**Error** > This rule enforces spacing around the colon in object literal properties. It can verify each property individually, or it can ensure vertical alignment of groups of properties in an object literal.

This rule has the properties `beforeColon` and `afterColon` set to `false` and `true`, respectively.

```javascript
var obj = { "foo": (42) };

foo = { thisLineWouldBeTooLong:
    soUseAnotherLine };
```

### Max-depth
**Allowed** > The `max-depth` rule allows you to specify the maximum depth blocks can be nested.

```javascript
function foo() {
  for (;;) { // Nested 1 deep.
    if (true) { // Nested 2 deep.
      if (true) { // Nested 3 deep.

      }
    }
  }
}
```

This rule aims to reduce the complexity of your code by allowing you to configure the maximum depth blocks can be nested in a function. As such, it will warn when blocks are nested too deeply.

