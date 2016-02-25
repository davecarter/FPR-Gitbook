### UnnecessaryMantissa

Numeric values should not contain unnecessary fractional portions. Otherwhise SASS will take that value as an unnecesary floating point unit reducing performance and increasing memory usage.

**Bad**

```scss
margin: 1.0em;
```

**Good**

```scss
margin: 1em;
```