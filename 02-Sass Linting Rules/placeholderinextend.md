### PlaceholderInExtend

Always use placeholder selectors in `@extend` to avoid generating more code than necessary.

**Bad: extending a class**

```scss
.fatal {
  @extend .error;
}
```

**Good: extending a placeholder**

```scss
.fatal {
  @extend %error;
}
```