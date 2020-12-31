# 54 - Unidades de medidas (cm, mm, pc, in) - Parte 4

[link](http://cfbcursos.com.br/css3-51525354-unidades-de-medida/)

**CM, MM, PC, IN**

**CM, MM, PC, IN** **Não São Recomendadas** para serem utilizadas na web devido aos seus problemas de responsividade.


* **1cm** = 37.7952px
* **1mm** = 3.7795px
* **1in** = 96px
* **1pc** = 16px
* **1pt** = 1.333

---

## Codeguins

---

```html
<body>
  <p id="p1">CFB Cursos - p1</p>
  <p id="p2">CFB Cursos - p2</p>
  <p id="p3">CFB Cursos - p3</p>

  <div id="d1"></div>
  <div id="d2"></div>
  <div id="d3"></div>
</body>
```


```css
html, body {
  padding: 0px;
  margin: 0px;
  background-color: #2f2f2f;
  color: #fff;
  font-family: Arial, sans-serif;
}

p:first-child {
  margin-top: 100px;
}

p {
  margin-left: 50%;
}

#p1 {
  /* Pixels */
  font-size: 20px;
}

#p2 {
  /*(pontos) 1pt = 1,333px */
  font-size: 20pt;
}

#p3 {
  /*(paicas) 1pc = 16px */
  font-size: 1pc;
}

div {
  border: 1px solid #ffffff;
  margin-left: 50%;
}

#d1 {
  /* Centimetro */
  width: 2.54cm;
  height: 2.54cm;
}

#d2 {
  /* 1 Milimetro = 10/100cm */
  width: 25.4mm;
  height: 25.4mm;
}

#d3 {
  /* 1 Polegada = 2.54cm */
  width: 1in;
  height: 1in;
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