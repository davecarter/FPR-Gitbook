### ImportantRule

In order to avoid specificity problems using `!important` in SASS properties is not allowed.

**Bad:**

```scss

.sui-Component {
    background-color: $c-bg-light !important;
}

```

**Good: Apply Class selector instead**

```scss

.sui-Component {
    background-color: $c-bg-light;
}

```