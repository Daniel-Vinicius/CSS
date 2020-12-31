# 53 - Unidades de medidas (vw, vh, ex) - Parte 3

[link](http://cfbcursos.com.br/css3-51525354-unidades-de-medida/)

**VW, VH, EX**

**EX Não é recomendada** para ser utilizada devido aos seus problemas de quebra de layout.
EX é igual ao EM só que para letras minúsculas.

**VW, VH**
* Um **VW** é igual 1/100 da largura da janela ou viewport width.
* Um **VH** é igual 1/100 da altura da janela ou viewport height.

---

## Exemplo com EX:

---

```html
 <body>
   <div id="d3"></div>
    <p>xcfb</p>
   <div id="d4"></div>
    <p>XCFB</p>
 </body>
```


```css
/* Exemplo de EM e EX */

html, body {
  padding: 0px;
  margin: 0px;
  background-color: #2f2f2f;
  color: #fff;
  font-family: Arial, sans-serif;
  font-size: 30px;
}


div, p {
  display: inline-block;
}

p {
  font-size: 10em;
  border: 1px solid #fff;
}

#d3 {
  width: 10ex;
  /* EX é igual ao EM só que para letras minúsculas */
  height: 10ex;
  background-color: #cf2d2d;
}

#d4 {
  width: 10em;
  height: 10em;
  background-color: #2da9cf;
}
```
---

## Exemplo com VW e VH:

---

```html
<body>
  <div id="d1">
    <div id="d2"></div>
  </div>
</body>
```


```css
/* Exemplo de VH e VW: */

html, body {
  padding: 0px;
  margin: 0px;
  background-color: #2f2f2f;
  color: #fff;
  font-family: Arial, sans-serif;
  font-size: 30px;
}


div {
  border: 5px solid #ffffff;
  border-radius: 10px;
}

#d1 {
  /* sempre que usar VW ou VH use box-sizing: border-box; */
  box-sizing: border-box;
  background-color: #1e6dd4;
  padding: 30px;
  /* 100/100 da largura da janela ou viewport width       */
  width: 100vw;
  /* 100/100 da altura da janela ou viewport height         */
  height: 100vh;
}

#d2 {
  background-color: #d41e1e;
  width: 50%;
  height: 50%;
}
```

---

  <table>
    <tbody>
      <tr>
        <td><strong>Unidade</strong></td>
        <td><strong>Descrição</strong></td>
      </tr>
      <tr>
        <td>em</td>
        <td>Unidade relativa ao tamanho do font-size anterior, aumenta ou diminui a fonte em relação a fonte-size, se
          elemento A tem font-size:15px e elemento B tem font-size:2em, então o tamanho do elemento B é igual a 30px.
          (15px X 2em = 30px)&nbsp; (5px X 4em = 20px)&nbsp; (2px X 1.5em = 3px)</td>
      </tr>
      <tr>
        <td>ex</td>
        <td>Unidade relativa à altura da letra x em font-size anterior.</td>
      </tr>
      <tr>
        <td>ch</td>
        <td>Unidade relatiza à largura do numeral zero do font-size anterior.</td>
      </tr>
      <tr>
        <td>rem</td>
        <td>Unidade relativa ao font-size do elemento raiz.</td>
      </tr>
      <tr>
        <td>vw</td>
        <td>Unidade relativa a 1% da largura da janela.</td>
      </tr>
      <tr>
        <td>vh</td>
        <td>Unidade relativa a 1% da altura da janela.</td>
      </tr>
      <tr>
        <td>vmin</td>
        <td>Unidade relativa a 1% da altura ou largura da janela, o que for menor.</td>
      </tr>
      <tr>
        <td>vmax</td>
        <td>Unidade relativa a 1% da altura ou largura da janela, o que for maior.</td>
      </tr>
      <tr>
        <td>%</td>
        <td>Porcentagem.</td>
      </tr>
      <tr>
        <td>cm</td>
        <td>Unidade absoluta relacionada a centímetros.</td>
      </tr>
      <tr>
        <td>mm</td>
        <td>Unidade absoluta relacionada a milímetros.</td>
      </tr>
      <tr>
        <td>in</td>
        <td>Unidade absoluta relacionada a polegadas. (1in = 96px = 2.54cm)</td>
      </tr>
      <tr>
        <td>px</td>
        <td>Unidade absoluta relacionada a pixels. (1px = 1/96th of 1in)</td>
      </tr>
      <tr>
        <td>pt</td>
        <td>Unidade absoluta relacionada a pontos. (1pt = 1/72 of 1in)</td>
      </tr>
      <tr>
        <td>pc</td>
        <td>Unidade absoluta relacionada a picas, pronuncia-se “paicas”. (1pc = 12pt)</td>
      </tr>
    </tbody>
  </table>