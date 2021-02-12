# Aula 3 Grid Layout

Aprendemos basicamente isso:

- _grid-column-start_ é uma propriedade aplicada aos elementos filhos que determina em qual coluna tal elemento vai iniciar.

- _grid-column-end_ é uma propriedade aplicada aos elementos filhos que determina qual coluna não se pode passar. Ex: não se pode passar a 4 então o elemento vai ocupar até a 3.

- _grid-column_ é uma propriedade que abrevia **grid-column-start** e **grid-column-end**.

Sintaxe:  
` /* grid-column: 1 / 4; 1 de start e 4 de end */`.

É possível usar span que só serve para grid-column e diz até onde tal elemento expande:  
`grid-column: 1 / span 4; span serve para dizer até onde tal item expande`.

Exemplo span: tal item precisa ocupar 4 de 8 colunas.

`grid-column: 4 / span 8`

---

- _grid-row-start_ é uma propriedade aplicada aos elementos filhos que determina em qual linha tal elemento vai iniciar.

- _grid-row-end_ é uma propriedade aplicada aos elementos filhos que determina qual linha não se pode passar. Ex: não se pode passar a 4 então o elemento vai ocupar até a 3.

- _grid-row_ é uma propriedade que abrevia **grid-row-start** e **grid-row-end**.

Ex:

```css
div {
  grid-row-start: 1;
  grid-row-end: 3;
  /* Vai Até o 3 e NÃO inclui o 3, logo ocupa 2 linhas */
  grid-row: 1 / 3;
}
```

---

```css
.item1 {
  /* grid-column-start: 1;
  grid-column-end: 3; Vai Até o 3 e NÃO inclui o 3, logo ocupa 2 colunas */
  /* grid-column: 1 / 4; 1 de start e 4 de end */
  /* grid-column: 1 / span 4; span serve para dizer até onde tal item expande, só serve para grid-column */

  grid-row-start: 1;
  grid-row-end: 3;
  /* Vai Até o 3 e NÃO inclui o 3, logo ocupa 2 linhas */
  grid-row: 1 / 3;
}
```

```html
<body>
  <div class="container">
    <div class="item item1">Div Item 1</div>
    <div class="item item2">Div Item 2</div>
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
