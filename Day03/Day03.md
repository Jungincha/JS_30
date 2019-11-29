# Update CSS Variables with JS

### CSS variables
Declares a custom property. It is very useful when it contains values that are reused

#### How to declare

```js
USE `--`
ELEMENT_OR_CLASS {
  --basic-color: blue;
}
```
#### How to access
USE `var()` function 
```js
ELEMENT_OR_CLASS {
  background: var(--basic-color);
}
```


### CSS :root Selector
It is the root element of the document. Meaning `html` selector but higher
1. You can set default CSS property on basic document
```js
:root {
  background: pink;
}
```
2. You can set grobal CSS property using CSS variables
```js
:root {
  --base-fontsize: 10px;
  --base-background: yellow;
}
```

### Document.documentElement
root element of the `document`<br>
`<html>` for **HTML** documents

