### ColorVariable

To avoid colour entropy all arround the site is mandatory to set colour using SASS variables as shown in the example below. Colour parametrization ensures better maintainability and are more verbose than setting an hex value as `#bada55`

**Bad: literal color**

```scss
.sui-Card-title {
    color: green;
}
```

**Good: refer to color by variable name**

```scss
$body-color: #c0ffee;

...

.sui-Card-title {
    color: $body-color;
}
```