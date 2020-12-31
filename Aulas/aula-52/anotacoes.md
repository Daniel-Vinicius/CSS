# 52 - Unidades de medidas (pixel e em) - Parte 2

[link](http://cfbcursos.com.br/css3-51525354-unidades-de-medida/)

**REM e %**

REM e % são unidades de medidas que podem ser aplicadas a qualquer elemento.
Um REM é igual ao tamanho da fonte do elemento :root ou html, font-size por padrão no html é 16px.
A % é referente a porcentagem do elemento pai

* **ATENÇÃOOOOO** REM não funcionará caso a font-size estiver no elemento pai, a font-size deve estar EXPLÍCITAMENTE NO ELEMENTO ROOT OU HTML DESSA FORMA:


```css
:root {
  font-size: 10px;
}

/* OU */

html {
  font-size: 10px;
}
```

Exemplo:

Note que no exemplo abaixo `#d1 tem 60x60rem` que equivale a `600x600px` pois no elemento `html` a propriedade `font-size` está setada com `10px`, logo mudando a `font-size` o tamanho de `#d1` também muda. O elemento de classe container tem 100% da largura e altura.


Note que `#d4` tem a altura e largura setadas como 75%, 75% de seu elemento pai que é `#d3`, ou seja a porcentagem é referente a porcentagem do elemento pai.


---

**Html:**

```html
<body>
  <section class="container">
    <div id="d1">
      <div id="d2">
        <div id="d3">
          <div id="d4"></div>
        </div>
      </div>
    </div>
  </section>
</body>
```

**Css:**

```css
html {
  font-size: 10px;
}

html, body {
  width: 100%;
  height: 100%;
  padding: 0;
  margin: 0;
  background-color: #2f2f2f;
  box-sizing: border-box;
}

.container {
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
  align-items: center;
  width: 100%;
  height: 100%;
  font-family: Arial, sans-serif;
  font-size: 10px;
  color: #fff;
}

div {
  border: 5px solid #ffffff;
  border-radius: 10px;
  margin: 10px;
  padding: 10px;
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
  align-items: center;
  box-sizing: border-box;
}

#d1 {
  background-color: #1e6dd4;
  height: 60rem;
  width: 60rem;
}

#d2 {
  background-color: #d41e1e;
  width: 75%;
  height: 75%;
}

#d3 {
  background-color: #fbff15;
  width: 75%;
  height: 75%;
}

#d4 {
  background-color: #179e13;
  width: 75%;
  height: 75%;
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