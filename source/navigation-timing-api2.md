## Navigation Timing API

```javascript
window.performance.timing;
{
  connectEnd: 1412379511942,
  connectStart: 1412379511010,
  domComplete: 1412379514540,
  domContentLoadedEventEnd: 1412379514254,
  domContentLoadedEventStart: 1412379514243,
  ...
}
```

Tempo total para carregar a página:

```javascript
var perfData = window.performance.timing;
perfData.loadEventEnd - perfData.navigationStart;
```

Tempo de resposta de um request:

```javascript
var perfData = window.performance.timing;
perfData.responseEnd - perfData.requestStart;
```
