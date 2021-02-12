# Aula 1 Grid Layout

Aprendemos basicamente isso:

- _grid-template-columns_ é uma propriedade que controla a quantidade e largura de colunas de algum display grid. No exemplo tenho 2 colunas. A primeira tem **250px** de largura, a segunda tem a largura redimensionada automaticamente com o valor auto.

---

- _grid-template-rows_ é uma propriedade que controla a quantidade e altura de linhas de algum display grid. No exemplo tenho 2 linhas. A primeira tem **200px** de altura, a segunda tem a altura não especificada com o valor auto, isso significa que a altura das linhas são regidas pelo tamanho dos elementos filhos.

```css
.container {
  display: grid;
  grid-template-columns: 250px auto;
  grid-template-rows: 200px auto;
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
    <div class="item" id="item2">Div Item 6</div>
    <div class="item">Div Item 7</div>
    <div class="item">Div Item 8</div>
    <div class="item">Div Item 9</div>
  </div>
</body>
```
