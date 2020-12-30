# 51 - Unidades de medidas (pixel e em) - Parte 1

[link](http://cfbcursos.com.br/css3-51525354-unidades-de-medida/)

**PX e EM**

PX e EM são unidades de medidas que podem ser aplicadas a qualquer elemento.
Um EM é igual a quantidade de medida do elemento pai.

Exemplo:

```html
  <section class="pai">
    <p id="pp1">Texto 1</p>
    <p id="pp2">Texto 2</p>
  </section>
```

```css
.pai {
  font-size: 1px;
}

#pp1 {
  font-size: 40px;
}

#pp2 {
  font-size: 40em;
}
```

Note que no exemplo acima os dois elementos p tem a mesma font-size.

**Html:**

```html
<body>
  <p id="p1">CFB Cursos</p>
  <p id="p2">CFB Cursos</p>
  <p id="p3">CFB Cursos</p>

  <div id="d1"></div>
  <div id="d2"></div>
</body>
```

**Css:**

```css
html {
  font-size: 20px;
}

body {
  color: #fff;
  font-family: Arial, sans-serif;
  padding: 0px;
  margin: 0px;
  background-color: #2f2f2f;
  font-weight: 500;
  overflow: auto;
  font-size: 2em;
}

div {
  display: inline-block;
  border: 5px solid #ffffff;
  width: 300px;
  border-radius: 10px;
}

#d1 {
  background-color: #1e6dd4;
  height: 80px;
}

#d2 {
  background-color: #d41e1e;
  height: 2em;
}

h1, h2, h3, h4, h5, h6, p {
  margin: 40px;
  font-size: 0.75em;
}

#p3 {
  font-size: 30px;
  color: #9523d6;
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