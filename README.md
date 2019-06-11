# VSO Shortlink

`http://*.vso.io/`

JavaScript bookmarklet:

```js
javascript:[,,o,v,c,,,,e,n]=location.href.split(/[\.\/]/g);v=='visualstudio'&&c=='com'&&e=='edit'&&navigator.clipboard.writeText(`http://${o}.vso.io/${n}`)&&prompt('Copied!', `http://${o}.vso.io/${n}`)&&false
```
