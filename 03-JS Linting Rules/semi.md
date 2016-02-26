### Semi
**Error** > Enforce Semicolons.

JavaScript is unique amongst the C-like languages in that it doesn't require semicolons at the end of each statement. In many cases, the JavaScript engine can determine that a semicolon should be in a certain spot and will automatically add it. This feature is known as automatic semicolon insertion (ASI) and is considered one of the more controversial features of JavaScript. For example, the following lines are both valid:

```javascript
var name = "ESLint"
var website = "eslint.org";
```

However, the ASI mechanism can sometimes be tricky to people who are using semicolons. For example, consider this code:

```javascript
return
{
    name: 'ESLint'
};
```

This may look like a `return` statement that returns an object literal, however, the JavaScript engine will interpret this code as:

```jasvascript
return;
{
    name: 'ESLint';
}
```

Effectively, a semicolon is inserted after the `return` statement, causing the code below it (a labeled literal inside a block) to be unreachable. This rule and the `no-unreachable` rule will protect your code from such cases.

On the other side of the argument are those who says that since semicolons are inserted automatically, they are optional and do not need to be inserted manually. However, the ASI mechanism can also be tricky to people who don't use semicolons. For example, consider this code:

```javascript
var globalCounter = { }

(function () {
    var n = 0
    globalCounter.increment = function () {
        return ++n
    }
})()
```

In this example, a semicolon will not be inserted after the first line, causing a run-time error (because an empty object is called as if it's a function). The `no-unexpected-multiline` rule can protect your code from such cases.

Although ASI allows for more freedom over your coding style, it can also make your code behave in an unexpected way, whether you use semicolons or not. Therefore, it is best to know when ASI takes place and when it does not, and have ESLint protect your code from these potentially unexpected cases. In short, as once described by Isaac Schlueter, a `\n` character always ends a statement (just like a semicolon) unless one of the following is true:

The statement has an unclosed paren, array literal, or object literal or ends in some other way that is not a valid way to end a statement. (For instance, ending with `.` or `,`.)
The line is `--` or `++` (in which case it will decrement/increment the next token.)
It is a `for()`, `while()`, `do`, `if()`, or `else`, and there is no `{`
The next line starts with `[`, `(`, `+`, `*`, `/`, `-`, `,`, `.`, or some other binary operator that can only be found between two tokens in a single expression.
