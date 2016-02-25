### No Console
**Error** > In JavaScript that is designed to be executed in the browser, it's considered a best practice to avoid using methods on console. Such messages are considered to be for debugging purposes and therefore not suitable to ship to the client.

```javascript
console.log("Hello world!");
console.error("Something bad happened.");
```
