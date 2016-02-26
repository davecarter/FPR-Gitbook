### React/react-in-jsx-scope
**Warning** > Prevent missing React when using JSX.

When using JSX, `<a />` expands to `React.createElement("a")`. Therefore the React variable must be in scope.

The following patterns are considered warnings:

```
const Stateless = (props) => <div>Hello {this.props.name}</div>;
```

The following patterns **are not** considered warnings:

```
import React from 'react';

const Stateless = (props) => <div>Hello {this.props.name}</div>;
```

