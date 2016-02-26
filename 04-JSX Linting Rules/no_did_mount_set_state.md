### React/no-did-mount-set-state
**Allowed** > Prevent usage of setState in componentDidMount.

Updating the state after a component mount will trigger a second `render()`` call and can lead to property/layout thrashing.

The following patterns are considered warnings:

```javascript
class MyComponent extends React.Component {
    componentDidMount(){
        this.setEstate({
            data: data
        });
    }
}
```

The following patterns **are not** considered warnings:

```javascript
class MyComponent extends React.Component {
    constructor(){
         this.setEstate({
            data: data
        });
    }

    componentDidMount(){
       ...
    }
}
```
