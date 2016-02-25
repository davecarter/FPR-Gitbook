### IdSelector

To avoid highly specific selectors ID's are not allowed to apply SASS styling:

**Bad: ID selector**

```scss

#sui-Component {
    background-color: $c-bg-light;
}

```

**Good: Apply Class selector instead**

```scss

.sui-Component {
    background-color: $c-bg-light;
}

```