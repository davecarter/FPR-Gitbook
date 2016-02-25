
### SelectorDepth

Max depth of selectors applicability is set to 3.

**Bad: selectors with depths of 4**

```scss
.one .two .three > .four {
  ...
}

.one .two {
  .three > .four {
    ...
  }
}
```

**Good: Max depth of 3**

```scss
.one .two .three {
  ...
}

.one .two {
  .three {
    ...
  }
}
```