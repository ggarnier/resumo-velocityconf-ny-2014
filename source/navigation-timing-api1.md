## Navigation Timing API

https://developer.mozilla.org/en-US/docs/Navigation_timing

![Timing overview](images/timing-overview.png)

```javascript
window.performance.timing;
// retorno:
{
  connectEnd: 1412379511942,
  connectStart: 1412379511010,
  domComplete: 1412379514540,
  domContentLoadedEventEnd: 1412379514254,
  domContentLoadedEventStart: 1412379514243,
  domInteractive: 1412379514242,
  domLoading: 1412379512583,
  domainLookupEnd: 1412379511010,
  domainLookupStart: 1412379511010,
  fetchStart: 1412379510754,
  loadEventEnd: 1412379514543,
  loadEventStart: 1412379514541,
  navigationStart: 1412379510754,
  redirectEnd: 0,
  redirectStart: 0,
  requestStart: 1412379511942,
  responseEnd: 1412379512566,
  responseStart: 1412379512366,
  secureConnectionStart: 1412379511209,
  unloadEventEnd: 0,
  unloadEventStart: 0
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
