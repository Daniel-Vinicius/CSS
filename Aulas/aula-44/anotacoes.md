# 44 - Box-sizing

[link](http://cfbcursos.com.br/css3-44-box-sizing/)

**Box-sizing**

1- Box-sizing

Quando você tem elementos que tem padding, border, outline, etc... eles se somam ao tamanho da largura do elemento, isso as vezes pode ser um problema e para isso existe a propriedade border-sizing.

Ela pode receber os seguintes valores: 
1- content-box é o padrão e soma border, padding, etc... a largura do elemento.
2- border-box é um valor que aplica a border, padding, etc.... ao elemento, porém não os somam a largura.

Ex: 

```css
#d1 {
  width: 300px;
  height: 200px;
  border: 10px solid #e72c2c;
  padding: 25px;
  box-sizing: border-box;
}

#d2 {
  width: 300px;
  height: 200px;
  border: 10px solid #1879e9;
  padding: 25px;
  box-sizing: content-box;
}
```

**Html:**

```html
<body>
  <div id="d1">Canal Fessor Bruno</div>
  <div id="d2">Canal Fessor Bruno</div>
</body>
```

**Css:**

```css
body {
  color: #fff;
  font-family: Arial, sans-serif;
  padding: 0px;
  margin: 100px;
  background-color: #2f2f2f;
  font-weight: 500;
}

#d1 {
  width: 300px;
  height: 200px;
  border: 10px solid #e72c2c;
  padding: 25px;
  box-sizing: border-box;
}

#d2 {
  width: 300px;
  height: 200px;
  border: 10px solid #1879e9;
  padding: 25px;
  box-sizing: content-box;
}
```
