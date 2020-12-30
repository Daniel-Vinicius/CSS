# 45 - Filter - Parte 1

[link](http://cfbcursos.com.br/css3-4546-e-47-filter/)

**Filter**

Filter é uma propriedade que aplica filtros as imagens, como por exemplo controlar o brilho, contraste, escala de cinza, embaçamento,
etc...

Nesta Primeira Aula Vimos os Valores sobre: 

* 1- Brilho é controlado pelo valor **brightness** e recebe um valor em porcentagem. Ex: `filter: brightness(200%);`.
* 2- Contraste é controlado pelo valor **contrast** e recebe um valor em porcentagem. Ex: `filter: contrast(400%);`.
* 3- Escala de Cinza é controlado pelo valor **grayscale** e recebe um valor em porcentagem de até 100%. Ex: `filter: grayscale(100%);`.
* 4- Embaçamento é controlado pelo valor **blur** e recebe um valor em px. Ex: `filter: blur(5px);`.

Ex: 

```css
.logo1 {
  filter: grayscale(100%);
  margin-top: 60px;
  margin-left: 20px;
  margin-bottom: 60px;
  margin-right: 40px;
}

.logo2 {
  filter: blur(5px);
  margin-top: 60px;
  margin-left: 20px;
  margin-bottom: 60px;
  margin-right: 40px;
}

.logo3 {
  filter: brightness(200%);
  margin-top: 60px;
  margin-left: 160px;
  margin-bottom: 60px;
  margin-right: 40px;
}

.logo4 {
  filter: contrast(400%);
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
</body>
```

**Css:**

```css
body {
  color: #fff;
  font-family: Arial, sans-serif;
  padding: 0px;
  background-color: #6f00ff;
  font-weight: 500;
  display: flex;
  justify-content: center;
  align-items: center;
  flex-wrap: wrap;
  margin: 0px;
  overflow: hidden;
}

.logo1 {
  filter: grayscale(100%);
  margin-top: 60px;
  margin-left: 20px;
  margin-bottom: 60px;
  margin-right: 40px;
}

.logo2 {
  filter: blur(5px);
  margin-top: 60px;
  margin-left: 20px;
  margin-bottom: 60px;
  margin-right: 40px;
}

.logo3 {
  filter: brightness(200%);
  margin-top: 60px;
  margin-left: 160px;
  margin-bottom: 60px;
  margin-right: 40px;
}

.logo4 {
  filter: contrast(400%);
  margin-top: 60px;
  margin-left: 20px;
  margin-bottom: 60px;
  margin-right: 40px;
}
```
