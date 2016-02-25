### HexLength

Set always hexadecimal color values in long format

**Bad: no long format hex value**

```scss

$c-bg-light: #fe0:

.sui-Component {
    background-color: $c-bg-light;
}

```

**Good: Long format hex value applied to a SASS var**

```scss

$c-bg-light: #bada55:

.sui-Component {
    background-color: $c-bg-light;
}

```
