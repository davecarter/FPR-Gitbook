### No Empty
**Error** > Empty statements usually occur due to refactoring that wasn't completed, such as:

```javascript
if (foo) {
}
```

The following pattern is **not** considered a problem:

```javascript
if (foo) {
  // left empty on purpose
}
```