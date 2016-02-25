### No Script Url
**Error** > Using `javascript:` URLs is considered by some as a form of `eval`. Code passed in `javascript:` URLs has to be parsed and evaluated by the browser in the same way that eval is processed.

The following pattern in considered a problem:

```javascript
location.href = "javascript:void(0)"; /*error Script URL is a form of eval.*/
```
