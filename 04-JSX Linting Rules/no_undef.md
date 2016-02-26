### React/jsx-no-undef
**Warning** > Disallow undeclared variables in JSX.

This rules can help you locate potential ReferenceErrors resulting from misspellings or missing components.

The following patterns are considered warnings:

```html
<MyComponent data={data} />
```

The following patterns **are not** considered warnings:

```html
import MyComponent from './src';

<MyComponent data={data} />
```

