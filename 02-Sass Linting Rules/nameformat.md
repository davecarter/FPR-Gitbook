
### NameFormat

Functions, mixins, variables, and placeholders should be declared with all
lowercase letters and hyphens instead of underscores.

**Bad: uppercase characters**

```scss
$myVar: 10px;

@mixin myMixin() {
  ...
}
```

**Good: all lowercase with hyphens**

```scss
$my-var: 10px;

@mixin my-mixin() {
  ...
}
```