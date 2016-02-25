### No Dupe Keys
**Error** > Creating objects with duplicate keys in objects can cause unexpected behavior in your application. The `no-dupe-keys` rule flags the use of duplicate keys in object literals.

The following patterns are considered problems:

```javascript
var foo = {
    bar: "baz",
    bar: "qux"
};
```