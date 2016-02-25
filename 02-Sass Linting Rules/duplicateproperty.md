### DuplicateProperty

Usually, if you set the same property twice inside the same selector is a mistake so you're not allowed to do so:

**Bad**

```scss
.sui-Card {
    float: left;
    text-transform: uppercase;
    float: right; // Second declaration
}
```