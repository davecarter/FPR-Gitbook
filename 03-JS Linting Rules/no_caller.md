### No Caller
**Error** > This rule is aimed at discouraging the use of deprecated and sub-optimal code, but disallowing the use of `arguments.caller` and `arguments.callee`.

You are not allow to do:

```javascript
function whoCalled() {
   if (arguments.caller == null)
      console.log('I was called from the global scope.');
   else
      console.log(arguments.caller + ' called me!');
}
```