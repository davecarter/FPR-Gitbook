### No Array Constructor
**Error** > Use of the Array constructor to construct a new array is generally discouraged in favour of array literal notation because of the single-argument pitfall and because the Array global may be redefined.

```javascript
new Array(0, 1, 2)
```