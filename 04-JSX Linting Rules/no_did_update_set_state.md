### React/no-did-update-set-state
**Allowed** > Prevent usage of setState in componentDidUpdate.

Updating the state after a component update will trigger a second `render()`` call and can lead to property/layout thrashing.

The following patterns are considered warnings:

```
class MyComponent extends React.Component {
    componentDidUpdate(){
        this.setEstate({
            name: this.props.name.toUpperCase()
        });
    }

    render(){
        return(
            <div>Hello {this.state.name} </div>
        )
    }
}
```

The following patterns **are not** considered warnings:

```
class MyComponent extends React.Component {
    constructor(){
         this.setEstate({
            name: this.props.name.toUpperCase()
        });
    }

    componentDidUpdate(){
       this.props.onUpdate();
    }

    render(){
        return(
            <div>Hello {this.props.name} </div>
        )
    }
}
```
