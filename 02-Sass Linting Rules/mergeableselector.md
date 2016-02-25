
### MergeableSelector

Reports when you define the same selector twice in a single sheet.

**Bad**

```scss
h1 {
  margin: 10px;
}

.baz {
  color: red;
}

// Second copy of h1 rule
h1 {
  text-transform: uppercase;
}
```