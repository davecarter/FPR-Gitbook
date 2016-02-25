### VendorPrefix

Avoid vendor prefixes. Use `autoprefixer` tools. Don't write them yourself.

**Bad: vendor prefixes**

```scss
@-webkit-keyframes anim {
  0% { opacity: 0; }
}

```

**Good**

```scss
// Autoprefix later in pre/post SASS processing...
@keyframes anim {
  0% { opacity: 0; }
}
```