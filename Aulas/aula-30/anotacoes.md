# 30- Display Parte 5

[link](http://cfbcursos.com.br/css3-262728-e-29-display/)
[Joguinho](https://flexboxfroggy.com/)

**Com o Joguinho De cima eu aprendi muito sobre flexbox, se você esquecer e só jogar de novo**

**Display Flex 3**

1- Order

order funciona para você alinhar algo específico com flex em alguma posição. 
No exemplo abaixo a d1 ocupa posição da d2 e vice-versa
Exemplo: 

```css
#d1 {
  order: 2;
  width: 100px;
}

#d2 {
  order: 1;
  width: 100px;
}

#d3 {
  order: 3;
  width: 100px;
}

#d4 {
  order: 4;
  width: 100px;
}

#d5 {
  order: 5;
  width: 100px;
}

#d6 {
  order: 6;
  width: 100px;
}
```

2- Flex

Flex é uma metapropriedade que engloba as 3 propriedades: flex-grow, flex-shrink e flex-basis nesta exata ordem. O padrão é 

```css 
#id {
 flex: 0 1 auto;
 }
```

3- Flex Grow

flex-grow dita se vai ou não esticar, ocupar o espaço vazio. Recebe os valores 1 caso vá esticar e 0 caso não esticará. O padrão é `0`.

```css 
#id {
  flex-grow: 1;
 }
```

4- Flex Shrink

flex-shrink dita se vai ou não contrair, ocupar o espaço vazio. Recebe os valores 1 caso vá contrair e 0 caso não contrairá. O padrão é `1`

```css 
#id {
  flex-shrink: 1;
 }
```

5- Flex Basis

 flex-basis dita quantos porcento de largura ou altura o elemento filho vai  ocupar do elemento pai, o padrão é `auto` que ocupa o espaço que definido e para de crescer, 
 flex-basis sobreescreve o flex-grow e a largura.

```css 
#id {
  flex-basis: 100%;
 }
```

**Html:**

```html
<body>
  <section id="s1">
    <div id="d1">DIV 1</div>
    <div id="d2">DIV 2</div>
    <div id="d3">DIV 3</div>
    <div id="d4">DIV 4</div>
    <div id="d5">DIV 5</div>
    <div id="d6">DIV 6</div>
  </section>
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

#s1 {
  border: 10px solid #ffffff;
  border-radius: 10px;
  margin: 20px;
  padding: 20px;
  background-color: #ff6347;
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
  align-items: center;
}

#s1>div {
  border: 5px solid #ffffff;
  border-radius: 10px;
  margin: 5px;
  padding: 5px;
  color: #303030;
  background-color: #ffffff;
  height: 100px;
}

#s1>div:hover {
  transition: 0.5s;
  outline: 10px solid #ff6347;
  background-color: #ff6347;
  color: #fff;
}

#d1 {
  order: 1;
  width: 100px;
}

#d2 {
  order: 2;
  width: 100px;
}

#d3 {
  order: 3;
  width: 100px;
}

#d4 {
  order: 4;
  width: 100px;
}

#d5 {
  order: 5;
  width: 100px;
}

#d6 {
  order: 6;
  width: 100px;
}
```
