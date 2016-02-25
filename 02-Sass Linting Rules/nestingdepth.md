### NestingDepth

The max nesting selectors in SASS files is: **4 levels**.

**Bad: descendent name anidation add overspecificity**

```scss

.sui-Component {
        …
    &-header {
    …
    }
    &-avatar {
    …
    }
    &-bodyText {
    …
    }
}
```

**Good: each descendent name is not anided with the parent**

```scss
.sui-Component {
… 
}
.sui-Component-header {
…
}
.sui-Component-avatar {
…
}
.sui-Component-bodyText {
…
}
```