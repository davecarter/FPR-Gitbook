### React/wrap-multilines
**Error** > Prevent missing parentheses around multiline JSX.

Wrapping multiline JSX in parentheses can improve readability and/or convenience. It optionally takes a second parameter in the form of an object, containing places to apply the rule. By default, "declaration", "assignment", and "return" syntax is checked, but these can be explicitly disabled. Any syntax type missing in the object will follow the default behavior.

The following patterns are considered errors:

```
class MyFirstComponent extends React.Component {
    render(){
        return
            <div>
                <h1>Hello {this.props.name}</h1>
            </div>
    }
}
```

The following patterns **are not** considered errors:

```
const singleLineJSX = <p>Hello</p>

class MyFirstComponent extends React.Component {
    render(){
        return(
            <div>
                <h1>Hello {this.props.name}</h1>
            </div>
        )
    }
}
```