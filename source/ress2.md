## Responsive com media queries

- estilos customizados por tamanho de tela
- arquivo CSS fica cada vez maior

```css
.thumb {
  width: 180px;
  height: 108px;
}

@media (max-width: 978px) and (min-width: 711px) {
  .thumb {
    width: 134px;
    height: 80px;
  }
}

@media (max-width: 710px) {
  .thumb {
    width: 140px;
    height: 84px;
  }
}
```
