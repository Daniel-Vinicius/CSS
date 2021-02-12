# Aula 2 Grid Layout

Aprendemos basicamente isso:

- _gap_ é uma propriedade que funciona com margin, porém aplicado no container pai.

---

- _column-gap_ é um gap somente para as colunas.

---

- _row-gap_ é um gap somente para as linhas.

```css
.container {
  display: grid;
  grid-template-columns: auto auto auto;
  /* row-gap: 20px;
  column-gap: 20px; */
  gap: 20px;
  /* gap: 4px 40px; Linhas depois colunas */
}
```

```html
<body>
  <div class="container">
    <div class="item">Div Item 1</div>
    <div class="item">Div Item 2</div>
    <div class="item">Div Item 3</div>
    <div class="item">Div Item 4</div>
    <div class="item">Div Item 5</div>
    <div class="item">Div Item 6</div>
    <div class="item">Div Item 7</div>
    <div class="item">Div Item 8</div>
    <div class="item">Div Item 9</div>
  </div>
</body>
```
