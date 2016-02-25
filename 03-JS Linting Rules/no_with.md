### No With
**Error** > The `with` statement is potentially problematic because it adds members of an object to the current scope, making it impossible to tell what a variable inside the block actually refers to. Additionally, the `with` statement cannot be used in `strict mode`.

This rule is aimed at eliminating `with` statements.
The following patterns is considered a problem:

```javascript
with (foo) { /*error Unexpected use of 'with' statement.*/
    // ...
}
```