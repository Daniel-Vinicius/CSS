# 33 - Propriedades position e z-index

[link](http://cfbcursos.com.br/css3-33-position/)

**Propriedades position e z-index**

**POSITIONNNNN**

1- Static 
 é o padrão, e não tem top nem left. `position: static;`

2- Absolute
 se posiciona em relação ao seu container. `position: absolute;`

3- Relative
 se posiciona em relação ao elemento anterior que for static, caso não tenha nenhum se posiciona em relação ao container.
 `position: relative;`

4- Fixed
 se posiciona em relação a janela, leva em conta a janela, window. `position: fixed;`

**Z-INDEX**
z-index define qual elemento se sobrepõe ao outro, recebe um número, e o padrão é o último elemento do html tem o maior z index. `z-index: 10;`


**Html:**

```html
<body>
  <div id="d0">
    <div id="d1"> Olá Daniel</div>
    <div id="d2"> A manhã estará ensolarado com temperatura amena</div>
  </div>
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
  font-size: 20px;
}

div {
  border: 1px solid #ffffff;
  background-color: #58880a;
}

#d0 {
  width: 700px;
  height: 500px;
  background-color: #1c92d6;
  position: absolute;
  top: 100px;
  left: 50px;
}

#d1, #d2 {
  width: 300px;
  height: 150px;
}

#d1 {
  position: absolute;
  top: 250px;
  left: 30%;
}

#d2 {
  position: absolute;
  top: 225px;
  left: 33%;
}
```
