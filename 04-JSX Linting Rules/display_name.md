### React/display-name
**Allowed** > `displayName` allows you to name your component in a React component definition. This name is used by React in debugging messages.

Example:

```javascript
class MyNamedComponent extends React.Component {

    constructor(props) {
        super(props);
        this.displayName = 'My named component';
        ...
    }

    render(){
        return /* Your JSX here */
    }
}
```
