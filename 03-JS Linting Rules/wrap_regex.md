### Wrap-regex
**Allowed** > Require Regex Literals to be Wrapped.

When a regular expression is used in certain situations, it can end up looking like a division operator. 

This is used to disambiguate the slash operator and facilitates more readable code.

The following patterns are considered problems:

```javascript
function a() {
    return /foo/.test("bar"); 
    /*error Wrap the regexp literal in parens to disambiguate the slash.*/
}
```

The following patterns are **not** considered problems:

```javascript
function a() {
    return (/foo/).test("bar");
}
```
