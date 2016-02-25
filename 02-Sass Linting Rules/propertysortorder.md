### PropertySortOrder

Use alphabetical order in your declaration statements. If you are using Sublime Text select all the properties and press `F5` to automatic sorting. Note: No grouping or line spaces between property blocks are allowed.

**Bad: No alphabetically ordered properties**

```scss

.sui-Component {
    width: 100%;
    background-color: $c-bg-light;
    margin: 0 auto;
}

```

**Good: Alphabetically ordered properties**

```scss

.sui-Component {
    background-color: $c-bg-light;
    margin: 0 auto;
    width: 100%;
}

```