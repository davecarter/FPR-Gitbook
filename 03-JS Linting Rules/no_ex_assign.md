### No Ex Assign
**Error** > Disallow Assignment of the Exception Parameter. When an error is caught using a `catch` block, it's possible to accidentally (or purposely) overwrite the reference to the error.

This rule's purpose is to enforce convention. Assigning a value to the exception parameter wipes out all the valuable data contained therein and thus should be avoided. Since there is no `arguments` object to offer alternative access to this data, assignment of the parameter is absolutely destructive.

The following pattern is considered a problem:

```javascript
try {
    // code
} catch (e) {
    e = 10;   /*error Do not assign to the exception parameter.*/
}
```