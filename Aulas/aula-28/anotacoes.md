# 28- Display Parte 3

[link](http://cfbcursos.com.br/css3-262728-e-29-display/)

**Display Flex**

Aula Mais Importante de Display

1- Com Display Flex a Propriedade Display será aplicada somente ao Container
2- flex-wrap com valor wrap quebra a linha ao invés de diminuir o tamanho dos elementos filhos, quando não há espaço suficiente

3- Para usar flex-wrap é recomendado um max-width no container, e também um width nos elementos filhos

4- Tanto o justify-content quanto o align-items só funcionam no display flex
5- justify-content alinha horizontalmente 
6- align-items alinha verticalmente

7- flex: 1; nos elementos filhos ajustam o tamnho em porcentagem, baseado no tamanho do container e em quantos irmãos ele tem. Ex: 1 container 4 divs flex:1; nas divs é igual a width: 25%;

8- Quando se usa flex: 1; não é possível setar largura

propriedade:

```css
#s1 {
  border: 10px solid #ffffff;
  border-radius: 10px;
  margin: 20px;
  padding: 20px;
  background-color: #ff6347;

  display: flex;      /* 1 */
  flex-wrap: wrap;    /* 2 */
  max-width: 100%;    /* 3.1 */
  justify-content: center;
  /* flex-direction: column; */
}

#s1 > div {
  border: 5px solid #ffffff;
  border-radius: 10px;
  margin: 5px;
  padding: 5px;
  color: #303030;
  background-color: #ffffff;

  /* flex: 1; */  /* 7 */
  width: 200px;  /* 3.2 */
  text-align: center;
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
  max-width: 100%;

  display: flex;
  flex-wrap: wrap;
  justify-content: center;
  /* flex-direction: column; */
}

#s1 > div {
  border: 5px solid #ffffff;
  border-radius: 10px;
  margin: 5px;
  padding: 5px;
  color: #303030;
  background-color: #ffffff;

  /* flex: 1; */
  width: 200px;
  text-align: center;
}

#s1 > div:hover {
  transition: 0.5s;
  outline: 10px solid #ff6347;
  background-color: #ff6347;
  color: #fff;
}
```
