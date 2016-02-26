### Guard-for-in
**Allowed** > Looping over objects with a `for in` loop will include properties that are inherited through the prototype chain. This behavior can lead to unexpected items in your for loop.

```javascript
for (key in foo) {
    doSomething(key);
}
```

This rule is aimed at preventing unexpected behavior that could arise from using a `for in` loop without filtering the results in the loop. As such, it will warn when `for in` loops do not filter their results with an `if` statement.

The following patterns are considered problems:
```javascript
for (key in foo) {    
    /*error The body of a for-in should be wrapped in an if statement to filter unwanted properties from the prototype.*/
    doSomething(key);
}
```

The following patterns are not considered problems:

```javascript
for (key in foo) {
    if ({}.hasOwnProperty.call(foo, key)) {
        doSomething(key);
    }
}
```

