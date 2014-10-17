## Hosted libraries

Ex: jQuery da CDN do Google

```javascript
  var sNew = document.createElement("script");
  sNew.async = true;
  sNew.src = "http://ajax.googleapis.com/ajax/libs/jquery/1.5.1/jquery.min.js";
  var s0 = document.getElementsByTagName('script')[0];
  s0.parentNode.insertBefore(sNew, s0);

  window.jQuery ||
    document.write('<script src="/path/to/your/jquery" />');
```
