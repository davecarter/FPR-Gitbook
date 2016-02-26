### React/no-multi-comp
**Error** > Prevent multiple component definition per file.

Declaring only one component per file improves readability and reusability of components.

The following patterns are considered errors:

```
// File components.js

class MyFirstComponent extends React.Component {
    render(){
        return(
            <div>Hello {this.props.name} </div>
        )
    }
}

class MySecondComponent extends React.Component {
    render(){
        return(
            <div>Hello {this.props.name} </div>
        )
    }
}

export default {MyFirstComponent, MySecondComponent};
```

The following patterns **are not** considered errors:

```
// File myFirstComponent.js

class MyFirstComponent extends React.Component {
    render(){
        return(
            <div>Hello {this.props.name} </div>
        )
    }
}

export default {MyFirstComponent};
```
