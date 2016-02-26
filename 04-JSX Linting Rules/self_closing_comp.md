### React/self-closing-comp
**Error** > Prevent extra closing tags for components without children.

Components without children can be self-closed to avoid unnecessary extra closing tag.

The following patterns are considered errors:

```
const MyComp = <TitleComponent name='This is a title'></TitleComponent>
```

The following patterns **are not** considered errors:

```
const MyComp = <TitleComponent name='This is a title' />
```
