### No Eval
**Error** > JavaScript's `eval()` function is potentially dangerous and is often misused. Using `eval()` on untrusted code can open a program up to several different injection attacks. The use of `eval()` in most contexts can be substituted for a better, alternative approach to a problem.

```javascript
var obj = { x: "foo" },
    key = "x",
    value = eval("obj." + key);
```