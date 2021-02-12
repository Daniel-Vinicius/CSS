# Aula 4 Grid Layout

Aprendemos basicamente isso:

- _grid-area_ é uma meta propriedade que abrevia na exata ordem:

  ```css
  div {
    grid-row-start: 1;
    grid-column-start: 1;
    grid-row-end: 4;
    grid-column-end: 4;
    grid-area: 1 / 1 / 4 / 4;
  }
  ```

---

```css
body {
  background-color: #222222;
  color: #fff;
  font-family: Arial;
}

html,
body {
  height: 100vh;
  width: 100vw;
  box-sizing: border-box;
}

* {
  box-sizing: border-box;
  margin: 0px;
  outline: 0px;
}

button {
  cursor: pointer;
}

.container {
  display: grid;
  grid-template-columns: auto auto;
  width: 100vw;
  height: 100vh;
  align-items: center;
  justify-content: center;
  padding: 30px;
  gap: 20px;
}

.item {
  background-color: #ff4848;
  border: 5px solid #ffffff;
  border-radius: 10px;
  display: flex;
  justify-content: center;
  align-items: center;
  width: 100%;
  height: 100%;
}

.area1 {
  /*
  grid-row-start 
  grid-column-start
  grid-row-end
  grid-column-end
  */
  grid-area: 1 / 1 / 4 / 4;
}

.area2 {
  /* grid-area: 4 /4 / 0 / 9; */
}

#i {
  /* height: 100vh;
  width: 200px; */
}
```

```html
<body>
  <div class="container">
    <div class="item area1">Div Item 1</div>
    <div class="item">Div Item 2</div>
    <div class="item">Div Item 3</div>
    <div class="item">Div Item 4</div>
    <div class="item">Div Item 5</div>
    <div class="item area2" id="i">Div Item 6</div>
    <div class="item">Div Item 7</div>
    <div class="item">Div Item 8</div>
    <div class="item">Div Item 9</div>
    <div class="item">Div Item 10</div>
  </div>
</body>
```
