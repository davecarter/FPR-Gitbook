### No Div Regex
**Error** > Disallow Regexs That Look Like Division. This is used to disambiguate the division operator to not confuse users.

The following patterns are considered problems:

```javascript
function bar() { return /=foo/; } /*error A regular expression literal can be confused with '/='.*/
```