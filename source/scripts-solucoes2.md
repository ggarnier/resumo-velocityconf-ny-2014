## soluções

Carregamento assíncrono

```javascript
(function(d, s, id) {
  var js, fjs = d.getElementsByTagName(s)[0];
  if (d.getElementById(id)) { return; }
  js = d.createElement(s); js.id = id;
  js.src = "//cdn.example.com/script.js";
  fjs.parentNode.insertBefore(js, fjs);
})(document, 'script', 'vf-js');
```

ou, nos browsers mais modernos:

```html
<script async defer src="//cdn.example.com/script.js" />
```
