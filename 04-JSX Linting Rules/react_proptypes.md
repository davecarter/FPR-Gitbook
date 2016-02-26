### React/prop-types
**Error** > Prevent missing props validation in a React component definition.

PropTypes improve the reusability of your component by validating the received data.

It can warn other developers if they make a mistake while reusing the component with improper data type.

The following patterns are considered errors:

```
class MyFirstComponent extends React.Component {
    render(){
        return(
            <div>Hello {this.props.name} </div>
        )
    }
}
```

The following patterns **are not** considered errors:

```
class MyFirstComponent extends React.Component {
    render(){
        return(
            <div>Hello {this.props.name} </div>
        )
    }
}

MyFirstComponent.propTypes = {
  name: React.PropTypes.string
};
```


