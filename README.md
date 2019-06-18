# VSO Shortlink JavaScript Bookmarklet

`http://*.vso.io/`

Display in `prompt`:

```js
javascript:[,,o,v,c,,,e,n]=location.href.split(/[\.\/]/g);v=='visualstudio'&&c=='com'&&e=='edit'&&prompt('Copied!',`http://${o}.vso.io/${n}`)&&false
```

Copy to clipboard:



Version without `prompt` using just the Clipboard API:

```js
javascript:[,,o,v,c,,,e,n]=location.href.split(/[\.\/]/g);v=='visualstudio'&&c=='com'&&e=='edit'&&navigator.clipboard.writeText(`http://${o}.vso.io/${n}`).then(()=>location.hash='copied').catch(e=>location.hash=e.toString())&&false
```

Display in page:

```js
javascript:[,,o,v,c,,,e,n]=location.href.split(/[\.\/]/g);v=='visualstudio'&&c=='com'&&e=='edit'&&`<a href="http://${o}.vso.io/${n}">${n}</a>`
```
