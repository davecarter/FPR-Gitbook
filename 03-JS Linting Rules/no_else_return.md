### No Else Return
**Error** > If an if block contains a return statement, the else block becomes unnecessary. Its contents can be placed outside of the block.

```javascript
function foo() {
    if (x) {
        return y;
    } else {
        return z;
    }
}
```