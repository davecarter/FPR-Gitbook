### No New Object
**Error** > The `Object` constructor is used to create new generic objects in JavaScript, such as:

```javascript
var myObject = new Object();
```

However, this is no different from using the more concise object literal syntax:

```javascript
var myObject = {};
```
For this reason, many prefer to always use the object literal syntax and never use the `Object` constructor.

While there are no performance differences between the two approaches, the byte savings and conciseness of the object literal form is what has made it the de facto way of creating new objects.

The following patterns are considered problems:

```javascript
var myObject = new Object(); /*error The object literal notation {} is preferrable.*/

var myObject = new Object;   /*error The object literal notation {} is preferrable.*/
```

The following patterns are not considered problems:

```javascript
var myObject = new CustomObject();
var myObject = {};
```
