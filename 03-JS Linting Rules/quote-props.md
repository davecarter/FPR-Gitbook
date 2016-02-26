### Quote-props
**Allowed** > Quoting Style for Property Names.

Object literal property names can be defined in two ways: using literals or using strings. For example, these two objects are equivalent:

```javascript
var object1 = {
    property: true
};

var object2 = {
    "property": true
};
```

In many cases, it doesn't matter if you choose to use an identifier instead of a string or vice-versa. Even so, you might decide to enforce a consistent style in your code.

