# 55 - Inherit e Initial

[link](http://cfbcursos.com.br/css3-55-inherit-e-initial/)

**Inherit e Initial**

**Inherit e Initial** são valores universais que podem ser passados a qualquer propriedade.


* **Inherit** = Valor referente aquela propriedade no css do pai, vem selecionado por padrão.

* **Initial** = Valor padrão do browser.

---

## Código

---

```html
<html lang="pt-br">

<head>
  <title>Curso de CSS</title>
  <meta charset="utf-8" />
  <link rel="stylesheet" href="style.css" />
</head>

<body>
  <div id="d1">
    <h1>CFB Cursos - Curso de CSS</h1>
    <p>CFB Cursos - Curso de CSS</p>
  </div>
  <div id="d2">
    <h1>CFB Cursos - Curso de CSS</h1>
    <p>CFB Cursos - Curso de CSS</p>
  </div>
  <div id="d3">
    <h1>CFB Cursos - Curso de CSS</h1>
    <p>CFB Cursos - Curso de CSS</p>
  </div>
</body>

</html>
```


```css
* {
  color: #7ec200;
}

html {
  padding: 0px;
  margin: 0px;
  background-color: #2f2f2f;
  color: #fff;
  font-family: Arial, sans-serif;
}

body {
  background-color: #bedcff;
  color: #002950;
}

#d1 {
  color: #ff17ec;
}

#d2 {
  color: #ff3c0b;
}

#d3 {
  color: #198bb8;
}

h1, p {
  color: inherit;
  font-family: initial;
}
```