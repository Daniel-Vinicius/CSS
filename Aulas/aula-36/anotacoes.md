# 36 - Pseudo-elementos After e Before

[link](http://cfbcursos.com.br/css3-36-e-37-pseudo-elementos-after-e-before/)

**Pseudo-elementos After e Before**

1- After

Coloca uma imagem ou um texto depois de algum elemento.

Ex: 

```css
.texto::after {
  content: " ------ Tchau Gurizadaaa";
}
```

2- Before

Coloca uma imagem ou um texto antes de algum elemento.

Ex:

```css
.imagem::before {
  content: url(imga.jpg);
}
```

**Html:**

```html
<body>
  <p class="texto imagem">Algo de CSS Aleatório</p>
  <p class="texto imagem">Algo de CSS Aleatório</p>
  <p class="texto imagem">Algo de CSS Aleatório</p>
</body>
```

**Css:**

```css
body {
  color: #fff;
  font-family: Arial, sans-serif;
  padding: 0px;
  margin: 0px;
  background-color: #2f2f2f;
  font-weight: 500;
  display: flex;
  flex-direction: column;
  align-items: center;
}

.imagem::before {
  content: url(imga.jpg);
}

.texto::after {
  content: " ------ Tchau Gurizadaaa";
}
```
