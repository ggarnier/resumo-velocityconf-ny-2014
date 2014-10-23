## User Timing API

```javascript
window.performance.getEntriesByName("slowOperation");
// ou window.performance.getEntriesByType("measure");
[{
  duration: 7444.391000026371,
  entryType: "measure",
  name: "slowOperation",
  startTime: 191147.77599996887
}, ...]

// Remove todas as marcações
window.performance.clearMarks();

// Remove a medição "slowOperation"
window.performance.clearMeasure("slowOperation");
```
