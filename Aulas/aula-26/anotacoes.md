# 26- Display Parte 1

[link](http://cfbcursos.com.br/css3-262728-e-29-display/)

**Display**


propriedade:

```css
#d1 {
  display: inline; // Não ocupa tudo e permite mais de 1 na mesma linha
}

#s1 {
  display: inline-block; // Ocupa tudo e permite mais de 1 na mesma linha
}

#d2 {
  display: none;         // Não Ocupa nada e nem aparece
 /* visibility: hidden; */
}

#s2 {
  display: block;      // Ocupa tudo e não permite mais de 1 na mesma linha
}
```

**Html:**

```html
<body>
  <div id="d1">Div 1</div>
  <span id="s1">Span 1</span>

  <div id="d2">Div 2</div>
  <span id="s2">Span 2</span>
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

div, span {
  border: 1px solid #ffffff;
  border-radius: 10px;
  margin: 50px;
  padding: 10px;
  width: 200px;
  height: 200px;
}

#d1 {
  display: inline;
}

#s1 {
  display: inline-block;
}

#d2 {
  display: none;
 /* visibility: hidden; */
}

#s2 {
  display: block;
}

```
