### TrailingSemicolon

All property values including; `@extend`, `@include`, and `@import` directives; and variable declarations should always end with a semicolon.
Although in CSS you can omit the semicolon if the statement is the last one it might lead to inconsistencies.

**Bad: no semicolon**

```scss
p {
  color: #fff
}
```

**Bad: space between value and semicolon**

```scss
p {
  color: #fff ;
}
```

**Good**

```scss
p {
  color: #fff;
}
```