### React/jsx-uses-vars
**Warning** > Prevent variables used in JSX to be incorrectly marked as unused.

Since 0.17.0 the ESLint `no-unused-vars` rule does not detect variables used in JSX (see details). This rules will find variables used in JSX and mark them as used.

This rule has no effect if the `no-unused-vars` rule is not enabled.

```javascript
import React from 'react';

// nothing to do with React
```

The following patterns **are not** considered warnings:

```
import React from 'react';

const Stateless = (props) => <div>Hello {this.props.name}</div>;
```
