### No Multi Spaces
**Error** > Multiple spaces in a row that are not used for indentation are typically mistakes. For example:

```javascript
if(foo  === "bar") {}
```

It's hard to tell, but there are two spaces between `foo` and `===`. 
Multiple spaces such as this are generally frowned upon in favor of single spaces:

```javascript
if(foo === "bar") {}
```

