
### ImportPath

An imported partials SASS file paths cannot have preceding underscores `_` but it must contain a `.scss` expension declared in path in order to be compatible with the `node-sass v.3.4.1`.

This update to `node-sass` is mandatory to execute this package under Node v.4.

**Bad**

```scss
@import "foo/_bar.scss";
@import "_bar.scss";
@import "_bar";
@import "bar.scss";
```

**Good**

```scss
@import "foo/bar";
@import "bar";
```
