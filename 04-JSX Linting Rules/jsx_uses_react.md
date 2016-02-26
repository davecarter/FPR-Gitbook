### React/jsx-uses-react
**Warning** > Prevent React to be incorrectly marked as unused.

JSX expands to a call to `React.createElement`, a file which includes React but only uses JSX should consider the React variable as used.

This rule has no effect if the `no-unused-vars` rule is not enabled.

The following patterns are considered warnings:

```javascript
import React from 'react';

// nothing to do with React
```

The following patterns **are not** considered warnings:

```
import React from 'react';

const Stateless = (props) => <div>Hello {this.props.name}</div>;
```
