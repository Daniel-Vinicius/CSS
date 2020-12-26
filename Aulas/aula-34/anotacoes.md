# 34 - Propriedades float e clear

[link](http://cfbcursos.com.br/css3-34-float-e-clear/)

**Propriedades float e clear**

1- Float
Tenho 2 elementos, e quero que o primeiro fique a direita, não posso usar margin nem padding para não quebrar o display que já está sendo usado para outra coisa, e a ordem do html afeta outras coisas. Aí uso o Float que serve para indicar onde irá flutuar determinado elemento. Como o order do flex, mas sem o flex.

Ex:

```css
#img1 {
  float: right;
}

#img2 {
  float: left;
}
```

2- Pode ser que algum elemento da tela que esteja embaixo, em resoluções mais altas seja afetado pelo float e para isso não acontecer existe o clear. Que não permite que o float seja aplicado a determinado elemento.

Ex: 

```css
.fix {
  clear: both; /* both = nas duas, tem também o right e o left */
  border-top: 1px solid #eeeeee;
  text-align: center;
}
```

**Html:**

```html
<body>
  <img id="img1" src="imga.jpg"> <img id="img2" src="imga.jpg">

  <p>Lorem ipsum dolor, sit amet consectetur adipisicing elit. Dignissimos architecto recusandae</p>
  <p>Lorem ipsum dolor, sit amet consectetur adipisicing elit. Dignissimos architecto recusandae</p>
  <p>Lorem ipsum dolor, sit amet consectetur adipisicing elit. Dignissimos architecto recusandae</p>

  <h3 class="fix">Loremt dicta facere alias nulla sit velit deserunt architecto!
  </h3>
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

p {
  text-align: center;
}

img {
  border: 5px solid #ffffff;
}

#img1 {
  float: left;
}

#img2 {
  float: right;
}

.fix {
  clear: both;
  border-top: 1px solid #eeeeee;
  text-align: center;
}
```
