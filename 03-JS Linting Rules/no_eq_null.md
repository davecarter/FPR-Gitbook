### No Eq Null
**Error** > Comparing to `null` without a type-checking operator (`==` or `!=`), can have unintended results as the comparison will evaluate to `true` when comparing to not just a `null`, but also an `undefined` value.

The `no-eq-null` rule aims reduce potential bug and unwanted behavior by ensuring that comparisons to `null` only match `null`, and not also `undefined`. As such it will flag comparisons to `null` when using `==` and `!=`.

The following patterns are considered problems:

```javascript
if (foo == null) {     /*error Use ‘===’ to compare with ‘null’.*/
  bar();
}

while (qux != null) {  /*error Use ‘===’ to compare with ‘null’.*/
  baz();
}
```