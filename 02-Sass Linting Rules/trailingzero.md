### TrailingZero

Don't write trailing zeros for numeric values with a decimal point in order to save additional bytes in generated CSS files.

**Bad: unnecessary trailing zero**

```scss
margin: .500em;
padding: 0.5em
```

**Good: no trailing zero**

```scss
margin: .5em;
padding: .5em
```