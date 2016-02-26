# JSX Linting Rules in ReactJS

![](../img/react-logo.png)

JSX is a JavaScript syntax extension that looks like XML. You can use a simple JSX syntactic transform with **ReactJS**.

JSX is **not** HTML inside JS. Is *syntactic sugar* to make more readable your returned code inside React components.

React JSX transforms from an XML-like syntax into native JavaScript. XML elements, attributes and children are transformed into arguments that are passed to `React.createElement`.

```javascript
var Nav;
// Input (JSX):
var app = <Nav color="blue" />;
// Output (JS):
var app = React.createElement(Nav, {color:"blue"});
```


React linting is provided by [Eslint-Plugin-React](https://github.com/yannickcr/eslint-plugin-react). We use JSX with React. These set of rules also has a different level of acceptance as JS:

- **Allowed** > You can use whatever is specified in this rule.
- **Warning** > If you don't follow this rule you'll get a warning alert in console.
- **Error** > You are not allowed to omit this rule.

