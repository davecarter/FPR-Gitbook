### Eqeqeq
**Error** > It is considered good practice to use the type-safe equality operators `===` and `!==` instead of their regular counterparts `==` and `!=`.

The reason for this is that `==` and `!=` do type coercion which follows the rather obscure Abstract Equality Comparison Algorithm. For instance, the following statements are all considered true:

- [] == false
- [] == ![]
- 3 == "03"

If one of those occurs in an innocent-looking statement such as `a == b` the actual problem is very difficult to spot.

```javascript
if (x == 42) { }            /*error Expected '===' and instead saw '=='.*/

if ("" == text) { }         /*error Expected '===' and instead saw '=='.*/

if (obj.getStuff() != undefined) {
}                           /*error Expected '!==' and instead saw '!='.*/
```
