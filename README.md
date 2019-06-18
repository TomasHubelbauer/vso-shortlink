# VSO Shortlink JavaScript Bookmarklet

`http://*.vso.io/`

## Display in `prompt`

```js
javascript:[,,o,v,c,,,e,n]=location.href.split(/[\.\/]/g);v+c+e=='visualstudiocomedit'&&prompt('Copied!',`http://${o}.vso.io/${n}`)&&false
```

## Copy to the clipboard

```js
javascript:[,,o,v,c,,,e,n]=location.href.split(/[\.\/]/g);v+c+e=='visualstudiocomedit'&&navigator.clipboard.writeText(`http://${o}.vso.io/${n}`).then(()=>location.hash='copied').catch(e=>location.hash=e.toString())&&false
```

## Display in the page

```js
javascript:[,,o,v,c,,,e,n]=location.href.split(/[\.\/]/g);v+c+e=='visualstudiocomedit'&&`<a href="http://${o}.vso.io/${n}">${n}</a>`
```
