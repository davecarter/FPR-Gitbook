### DeclarationOrder

Place `@extend` and `@include` before properties so you can overwrite them later if needed.

**Bad**

```scss
.sui-Card-mediaContent {
p {
...
}

color: #bg-light;
@extend %sui-Card-boxContent;
@include message-box();
}
```

**Good**

```scss
.sui-Card-mediaContent {
    @extend %sui-Card-boxContent;
    @include message-box();
    color: #bg-light;

    p {
        ...
    }
}
```