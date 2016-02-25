### HexNotation

Reports uppercase hex color notation:

**Bad: Uppercase notation is not allowed**

```scss

$c-bg-light: #BADA55:

.sui-Component {
    background-color: $c-bg-light;
}

```

**Good: Lowercase hex notation value applied to a SASS var**

```scss

$c-bg-light: #bada55:

.sui-Component {
    background-color: $c-bg-light;
}

```
