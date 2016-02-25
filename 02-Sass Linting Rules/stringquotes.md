### StringQuotes

String literals should be written with single quotes unless using double quotes
would save on escape characters.

The reason why we prefer single quotes is because are easier to type (no shift key needed) in most keyboards.

**Bad: double quotes**

```scss
content: "hello";
```

**Good: single quotes**

```scss
content: 'hello';
```

**Good: double quotes prevent the need for escaping single quotes**

```scss
content: "'hello'";
```