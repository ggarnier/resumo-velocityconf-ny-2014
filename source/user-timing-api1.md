## User Timing API

http://www.sitepoint.com/discovering-user-timing-api/
http://www.w3.org/TR/user-timing/

Instrumentação de operações sob demanda

```javascript
// Marca o início de uma operação
window.performance.mark("startOperation");

doSomethingSlow();

// Marca o fim da operação
window.performance.mark("endOperation");

// Calcula as medições
window.performance.measure("slowOperation", "startOperation", "endOperation");
```
