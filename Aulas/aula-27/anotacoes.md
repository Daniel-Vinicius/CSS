# 27- Display Parte 2

[link](http://cfbcursos.com.br/css3-262728-e-29-display/)

**Display**


propriedade:

```css
  display: table-cell;
  text-align: center;           /* Faz o papel de justify-content ele alinha horizontalmente ao centro */
  vertical-align: middle;      /* Faz o Papel de align-items ele alinha verticalmente ao centro */

  /* display: flex; Tanto o justify-content quanto o align-items só funcionam no display flex
  justify-content: center;
  align-items: center; */
```

**Html:**

```html
<body>
  <p>Algo de CSS Aleatório</p>

  <div>DIV</div>

  <ol>
    <ul>
      <li>Cor</li>
      <li>Forma</li>
      <li>Objeto</li>
    </ul>
    <ul>
      <li>Verde</li>
      <li>Quadrado</li>
      <li>Caneta</li>
    </ul>
    <ul>
      <li>Vermelho</li>
      <li>Círculo</li>
      <li>Microfone</li>
    </ul>
  </ol>

</body>
```

**Css:**

```css
body {
  color: #fff;
  font-family: Arial, sans-serif;
  padding: 0px;
  background-color: #2f2f2f;
  font-weight: 500;
  font-size: 20px;
}

div {
  background-color: #ff6347;
  border: 10px solid #ffffff;
  border-radius: 10px;
  width: 200px;
  height: 200px;
  /* line-height: 200px; line-height = altura da linha */

  display: table-cell;
  text-align: center;           /* Faz o papel de justify-content ele alinha horizontalmente ao centro */
  vertical-align: middle;      /* Faz o Papel de align-items ele alinha verticalmente ao centro */

  /* display: flex; Tanto o justify-content quanto o align-items só funcionam no display flex
  justify-content: center;
  align-items: center; */
}

ol, ul, li {
  border: 1px solid #FFFFFF;
  margin: 0px;
  padding: 10px;
}

ol {
  display: table;
  width: 80%;
  margin-top: 20px;
}

ul {
  display: table-row;
}

li {
  display: table-cell;
  text-align: center;
}

```
