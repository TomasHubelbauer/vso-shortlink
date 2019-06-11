# VSO Shortlink

`http://*.vso.io/`

JavaScript bookmarklet:

```js
javascript:parts = location.href.split(/[\.\/]/g); if (parts[3] === 'visualstudio' && parts[4] === 'com' && parts[8] === 'edit') alert(`http://${parts[2]}.vso.io/${parts[9]}`)
```
