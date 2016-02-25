### No Fallthrough
**Error** > The `switch` statement in JavaScript is one of the more error-prone constructs of the language thanks in part to the ability to "fall through" from one case to the next. For example:

This rule is aimed at eliminating **unintentional fallthrough** of one case to the other. As such, it flags and fallthrough scenarios that are not marked by a comment.

The following pattern is considered a problem:

```javascript
switch(foo) {
    case 1:            /*error Expected a "break" statement before "case".*/
        doSomething();

    case 2:
        doSomething();
}
```
The following pattern is **not** considered a problem:

```javascript
switch(foo) {
    case 1:
        doSomething();
        break;

    case 2:
        doSomething();
}
```