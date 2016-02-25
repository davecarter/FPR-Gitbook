### Curly
**Error** > JavaScript allows the omission of curly braces when a block contains only one statement. However, it is considered by many to be best practice to never omit curly braces around blocks, even when they are optional, because it can lead to bugs and reduces code clarity. So the following:

This rule is aimed at preventing bugs and increasing code clarity by ensuring that block statements are wrapped in curly braces. It will throw an error when it encounters blocks that omit curly braces.

The following pattern is considered a problem:

```javascript
if (foo) foo++;
```
Can be rewritten as:

```javascript
if (foo) {
    foo++;
}
```
