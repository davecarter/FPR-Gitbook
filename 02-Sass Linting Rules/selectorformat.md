### SelectorFormat

The selector format **naming convention** used here is based in [SUIT CSS](https://github.com/suitcss/suit/blob/master/doc/naming-conventions.md)

It must match the following RegEx:
`^(?:[a-zA-Z0-9]*)\-[A-Z]{1}[a-z][a-zA-Z0-9]*(?:\-[a-z][a-zA-Z0-9]*)?(?:\-\-[a-z][a-zA-Z0-9]*)?$`

Perhaps you prefer to see an example:

```
.pre-MyComponent {}
.pre-MyComponent.is-animating {}
.pre-MyComponent--modifier {}

.pre-MyComponent-element {}
.pre-MyComponent-anotherElement {}

```