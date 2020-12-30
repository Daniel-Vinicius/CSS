# 46 - Filter - Parte 3

[link](http://cfbcursos.com.br/css3-4546-e-47-filter/)

**Filter**

Filter é uma propriedade que aplica filtros as imagens, como por exemplo controlar a
Sombra, Matriz, Inversão de Cores, Opacidade, Saturação, Sepia, etc...

Nesta Segunda Aula Vimos os Valores sobre:

* 1- Sombra é controlada pelo valor **drop-shadow** e recebe um valor em
``filter: drop-shadow(distanciaHorizontal distanciaVertical tamanho cor);``. 

Ex:
 ```css
 .logo1 {
   /* Sombra Estilo de Brilho */
    filter: drop-shadow(0px 0px 10px #8409d0);
    /* Sombra Estilo de Sombra */
    filter: drop-shadow(5px 5px 2px #8409d0);
 }
```

---

* 2- Matriz é controlada pelo valor **hue-rotate** e recebe um valor em graus. Ex: `filter: hue-rotate(307deg);`.

---

* 3- Inversão de Cores é controlada pelo valor **invert** e recebe os valores 0 ou 1. Ex: `filter: invert(1);`.

---

* 4- Opacidade é controlada pelo valor **opacity** e recebe um valor em porcentagem entre 0 e 100%. Ex: `filter: opacity(10%);`.

---

* 5- Saturação é controlada pelo valor **saturate** e recebe um valor em porcentagem. Ex: `filter: saturate(800%);`.

---

* 6- Sepia é controlada pelo valor **sepia** e recebe um valor em porcentagem entre 0 e 100%. Ex: `filter: sepia(100%);`.

---

Ex: 

```css
.logo1 {
  /* Sintaxe: filter: drop-shadow(distanciaHorizontal distanciaVertical tamanho cor);*/
  /* Sombra Estilo de Brilho */
  /* filter: drop-shadow(0px 0px 10px #8409d0); */
  /* Sombra Estilo de Sombra */
  filter: drop-shadow(5px 5px 2px #8409d0);
  /**/
  margin-top: 60px;
  margin-left: 20px;
  margin-bottom: 60px;
  margin-right: 40px;
}

.logo2 {
  filter: hue-rotate(307deg);
  margin-top: 60px;
  margin-left: 20px;
  margin-bottom: 60px;
  margin-right: 40px;
}

.logo3 {
  filter: invert(1);
  margin-top: 60px;
  margin-left: 160px;
  margin-bottom: 60px;
  margin-right: 40px;
}

.logo4 {
  filter: opacity(10%);
  margin-top: 60px;
  margin-left: 20px;
  margin-bottom: 60px;
  margin-right: 40px;
}

.logo5 {
  filter: saturate(800%);
  margin-top: 60px;
  margin-left: 20px;
  margin-bottom: 60px;
  margin-right: 40px;
}

.logo6 {
  width: 300px;
  filter: sepia(100%);
  margin-top: 60px;
  margin-left: 20px;
  margin-bottom: 60px;
  margin-right: 40px;
}
```

**Html:**

```html
<body>
  <img class="logo1" src="logo.png">
  <img class="logo2" src="logo.png">
  <img class="logo3" src="logo.png">
  <img class="logo4" src="logo.png">
  <img class="logo5" src="logo.png">
  <img class="logo6" src="foto.jpeg">
</body>
```

**Css:**

```css
body {
  color: #fff;
  font-family: Arial, sans-serif;
  padding: 0px;
  background-color: #1e1e1f;
  font-weight: 500;
  display: flex;
  justify-content: center;
  align-items: center;
  flex-wrap: wrap;
  margin: 0px;
}

.logo1 {
  /* Sintaxe: filter: drop-shadow(distanciaHorizontal distanciaVertical tamanho cor);*/
  /* Sombra Estilo de Brilho */
  /* filter: drop-shadow(0px 0px 10px #8409d0); */
  /* Sombra Estilo de Sombra */
  filter: drop-shadow(5px 5px 2px #8409d0);
  /**/
  margin-top: 60px;
  margin-left: 20px;
  margin-bottom: 60px;
  margin-right: 40px;
}

.logo2 {
  filter: hue-rotate(307deg);
  margin-top: 60px;
  margin-left: 20px;
  margin-bottom: 60px;
  margin-right: 40px;
}

.logo3 {
  filter: invert(1);
  margin-top: 60px;
  margin-left: 160px;
  margin-bottom: 60px;
  margin-right: 40px;
}

.logo4 {
  filter: opacity(10%);
  margin-top: 60px;
  margin-left: 20px;
  margin-bottom: 60px;
  margin-right: 40px;
}

.logo5 {
  filter: saturate(800%);
  margin-top: 60px;
  margin-left: 20px;
  margin-bottom: 60px;
  margin-right: 40px;
}

.logo6 {
  width: 300px;
  filter: sepia(100%);
  margin-top: 60px;
  margin-left: 20px;
  margin-bottom: 60px;
  margin-right: 40px;
}
```
