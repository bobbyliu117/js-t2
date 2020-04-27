# js-t2

## [REF Udemy WebComponent](https://www.udemy.com/course/web-components-stenciljs-build-custom-html-elements)

### Naming must have one `-` sign
```js
customElements.define('uc-tooltip', Tooltip);
```

### Element attached in `connectedCallback` Lifecycle
1. DOM operation here (w/o shadowDOM)
2. Add listeners here
```js
connectedCallback() {
  this.appendChild(tooltipIcon);
  tooltipIcon.addEventListener('mouseenter', this._show.bind(this));
}
```

### [`textContent` vs. `innerText`](https://stackoverflow.com/a/35213639)
innerText wont't show `display:none` -> less efficient

### hasAttribute
```js
if(this.hasAttribute('text')) {
  this._tip = this.getAttri
}
```

### Attributes vs. Properties
![Imgur](https://i.imgur.com/cxMT8wb.png)


