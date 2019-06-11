# VSO Shortlink

`http://*.vso.io/`

JavaScript bookmarklet:

```js
javascript:p=location.href.split(/[\.\/]/g);p[3]==='visualstudio'&&p[4]==='com'&&p[8]==='edit'&&navigator.clipboard.writeText(`http://${p[2]}.vso.io/${p[9]}`)&&prompt('Copied!', `http://${p[2]}.vso.io/${p[9]}`)&&false
```
