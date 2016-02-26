### New-cap
**Error** > Require Constructors to Use Initial Caps. 

The `new` operator in JavaScript creates a new instance of a particular type of object. That type of object is represented by a constructor function. 

Since constructor functions are just regular functions, the only defining characteristic is that `new` is being used as part of the call. Native JavaScript functions begin with an uppercase letter to distinguish those functions that are to be used as constructors from functions that are not. Many style guides recommend following this pattern to more easily determine which functions are to be used as constructors.

```javascript
var friend = new Person();
```

This rule is aimed at helping to distinguish regular functions from constructor functions. As such, it warns whenever it sees new followed by an identifier that isn't capitalized or whenever it sees capitalized function called directly without new operator.

The following patterns are considered problems:

```javascript
var friend = new person(); /*error A constructor name should not start with a lowercase letter.*/
var colleague = Person();  /*error A function with a name starting with an uppercase letter should only be used as a constructor.*/
```

The following patterns are **not** considered problems:

```javascript
var colleague = Person();
var colleague = foo.Person();
var colleague = foo.bar.Person();
```

