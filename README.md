# VSO Shortlink

`http://*.vso.io/`

JavaScript bookmarklet:

```js
javascript:parts = location.href.split(/[\.\/]/g); if (parts[3] === 'visualstudio' && parts[4] === 'com' && parts[8] === 'edit') alert(`http://${parts[2]}.vso.io/${parts[9]}`)
```

- Try to use the https://developer.mozilla.org/en-US/docs/Web/API/Clipboard_API for automatic copying
  It should could as a secure context since the VSO instance is on HTTPS
