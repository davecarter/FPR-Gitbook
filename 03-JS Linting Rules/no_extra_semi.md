### No Extra Semi
**Warning** > JavaScript will more or less let you put semicolons after any statement without complaining. Typos and misunderstandings about where semicolons are required can lead to extra semicolons that are unnecessary.

The following pattern in considered a problem:

```javascript
var x = 5;;     /*error Unnecessary semicolon.*/

function foo() {
    // code
};              /*error Unnecessary semicolon.*/
```
