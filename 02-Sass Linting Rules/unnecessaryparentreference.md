
### UnnecessaryParentReference

Do not use parent selector references (`&`) when they would otherwise be
unnecessary.

**Bad**

```scss
.sui-Card {
  & > .sui-Card-content {
    ...
  }
}
```

**Good**

```scss
.sui-Card {
  > .sui-Card-content {
  }
}
```