### No Implied Eval
**Error** > It's considered a good practice to avoid using `eval()` in JavaScript. There are security and performance implications involved with doing so, which is why many linters (including ESLint) recommend disallowing `eval()`. However, there are some other ways to pass a string and have it interpreted as JavaScript code that have similar concerns.

The first is using `setTimeout()`, `setInterval()` or `execScript()` (Internet Explorer only), both of which can accept a string of JavaScript code as their first argument. For example:

```javascript
setTimeout("alert('Hi!');", 100);
```

This is considered an implied `eval()` because a string of JavaScript code is passed in to be interpreted. The same can be done with `setInterval()` and `execScript()`. Both interpret the JavaScript code in the global scope. For both `setTimeout()` and `setInterval()`, the first argument can also be a function, and that is considered safer and is more performant:

```javascript
setTimeout(function() {
    alert("Hi!");
}, 100);
```
The best practice is to always use a function for the first argument of `setTimeout()` and `setInterval()` (and avoid `execScript()`).

