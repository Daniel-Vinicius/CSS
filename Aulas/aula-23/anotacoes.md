# 23- Formatações para Listas

link: http://cfbcursos.com.br/css3-23-formatacoes-para-listas/

**Formatações para Listas**

As Formatações para Listas manipulam: `o estilo de lista` através de sua

propriedade:

```css
ul {
  /* list-style-image:url(
    "./seta-direita.png"
  ); Imagem */

  list-style: none;
  /* Sem nada */
}
```

**Html:**

```html
  <body>
    <ol>
      <li>HTML5</li>
      <li>Javascript</li>
      <li>CSS</li>
      <li>jQuery</li>
      <li>PHP</li>
      <li>MySQL</li>
    </ol>
<div class="linha"></div>
    <ul>
      <li>HTML5</li>
      <li>Javascript</li>
      <li>CSS</li>
      <li>PHP</li>
      <li>MySQL</li>
    </ul>
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

ol,
ul {
  margin-left: 500px;

  /* list-style-image:url(
    "./seta-direita.png"
  ); Imagem */

  list-style: none;
  /* Sem nada */
}

.linha {
  height: 5px;
  background-color: #f0f0f0;
  width: 100%;
  border-radius: 10px;
}
```
