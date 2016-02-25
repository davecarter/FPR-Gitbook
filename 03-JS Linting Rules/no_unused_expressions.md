### No Unused Expressions
**Error** > Unused expressions are those expressions that evaluate to a value but are never used. For example:

```javascript
"Hello world";
```
By default the following patterns are considered problems:

```javascript
0         /*error Expected an assignment or function call and instead saw an expression.*/

if(0) 0   /*error Expected an assignment or function call and instead saw an expression.*/
```

The following patterns are **not** considered problems by default:

```javascript
a = 0
new C
delete a.b
```
