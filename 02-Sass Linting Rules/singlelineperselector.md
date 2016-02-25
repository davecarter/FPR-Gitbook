### SingleLinePerSelector

Split selectors onto separate lines after each comma, and have each individual
selector occupy a single line.

**Bad: comma-separated selectors not on their own lines**

```scss
.error p, p.explanation {
  ...
}
```

**Bad: descendent selector spread over multiple lines**

```scss
.error
  p,
  p.explanation {
  ...
}
```

**Good: each selector sequence is on its own individual line**

```scss
.error p,
p.explanation {
  ...
}
```