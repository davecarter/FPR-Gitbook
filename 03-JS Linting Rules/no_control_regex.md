### No Control Regex
**Error** > Control characters are special, invisible characters in the ASCII range 0-31. These characters are rarely used in JavaScript strings so a regular expression containing these characters is most likely a mistake.

```javascript
var pattern1 = /\\x1f/;
var pattern2 = new RegExp("\x1f");
```