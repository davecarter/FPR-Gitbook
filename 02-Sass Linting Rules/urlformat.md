### UrlFormat

URLs should not contain protocols or domain names.

Including protocols or domains in URLs makes them brittle to change, and also
unnecessarily increases the size of your CSS documents, reducing performance.

**Bad: protocol and domain present**

```scss
background: url('https://example.com/assets/image.png');
```

**Good**

```scss
background: url('assets/image.png');
```