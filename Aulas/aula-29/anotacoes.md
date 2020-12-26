# 29- Display Parte 4

[link](http://cfbcursos.com.br/css3-262728-e-29-display/)
[Joguinho](https://flexboxfroggy.com/)

**Com o Joguinho De cima eu aprendi muito sobre flexbox, se você esquecer e só jogar de novo**

**Display Flex 2**

Aula Mais Importante de Display

1- Com Display Flex a Propriedade Display será aplicada somente ao Container
2- flex-wrap com valor wrap quebra a linha ao invés de diminuir o tamanho dos elementos filhos, quando não há espaço suficiente

3- Para usar flex-wrap é recomendável um max-width no container, e também um width nos elementos filhos

4- Tanto o justify-content quanto o align-items só funcionam no display flex

5- justify-content alinha horizontalmente em linha
6- align-items alinha verticalmente em linha


**_Note que quando a direção é em coluna, justify-content muda para a vertical e align-items para a horizontal._**


7- flex: 1; nos elementos filhos ajustam o tamnho em porcentagem, baseado no tamanho do container e em quantos irmãos ele tem. Ex: 1 container 4 divs flex:1; nas divs é igual a width: 25%;

8- Quando se usa flex: 1; não é possível setar largura

9- As duas propriedades flex-direction e flex-wrap são usadas tão frequentemente juntas que uma propriedade abreviada flex-flow foi criada para combiná-las.
Essa propriedade aceita o valor das duas propriedades separados por um espaço.
Por examplo, você pode usar flex-flow: row wrap para aplicar a direção de linha e quebrar em múltiplas linhas.

10- align-content

Você pode usar align-content para definir como múltiplas linhas devem ser espaçadas uma das outras. Essa propriedade recebe os seguintes valores:

flex-start: Linhas são agrupadas no topo do container.
flex-end: Linhas são agrupadas no fundo do container.
center:Linhas são agrupadas no centro vertical do container.
space-between: Linhas são posicionadas com espaço igual entre elas.
space-around: Linhas são posicionadas com espaço igual em torno delas.
stretch: Linhas se esticam para preencher o container.
Isso pode ser confuso, mas align-content determina o espaçamento entre linhas, enquanto align-items determina como as linhas como um todo são alinhadas dentro do container. Quando há só uma linha, align-content não tem nenhum efeito.

ex: 
``css #algo { order: 1 } /* alinha totalmente a direita se for uma linha e totalmente a cima caso for uma coluna */``

11- align-self

é igual align items mas para somente um elemento específico

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
  /* flex-flow: column wrap */
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
