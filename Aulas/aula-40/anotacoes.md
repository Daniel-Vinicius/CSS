# 40 - Animation - parte 1

[link](http://cfbcursos.com.br/css3-40-e-41-animacoes/)

**Animation - parte 1**

1- Animation

Para realizar animações com css existe uma propriedade chamada @keyframes que é onde você escreve uma animation.
No From você coloca as propriedades para o começo da animation. Já no To você coloca as propriedades para o final da animation. 

Ex: 

No exemplo abaixo **anima1** é o nome da animation, e ela movimenta o elemento que a executa em left de 0px até 900px.

```css
@keyframes anima1 {
  from {
    left: 0px;
  }
  to {
    left: 900px;
  }
}
```

Para executar uma ou mais animations existem as propriedades: 

* animation-name - Recebe os nomes das animações que você quer executar em ordem separadas por vírgula.

* animation-duration - Recebe um valor em segundos para duração de cada animation ou um único valor de duração para todas as animations separadas por vírgula.

* animation-delay - Esse é o delay para começar cada uma das animações separadas por vírgula.
* animation-timing-function - Esse é o estilo da ou das animations separadas por vírgula.

```css
p {
  animation-name: anima1, anima2, anima3, anima4;
  /* Também pode abreviar só com 2s pra todos */
  animation-duration: 2s, 2s, 2s, 2s;
  /* Esse é o delay para começar cada uma das animações */
  animation-delay: 0s, 2s, 4s, 6s;
  /* As duas primeiras animations recebem ease-out e as duas últimas recebem ease-in */
  animation-timing-function: ease-out, ease-in;
}
```


**Html:**

```html
<body>
  <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Harum debitis ullam error officia repellat unde cupiditate
    delectus. Necessitatibus optio blanditiis deserunt suscipit vero sunt recusandae est facere excepturi ut? Itaque.
  </p>
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
}

@keyframes anima1 {
  from {
    left: 0px;
  }
  to {
    left: 900px;
  }
}

@keyframes anima2 {
  from {
    top: 300px;
  }
  to {
    top: 50px;
  }
}

@keyframes anima3 {
  from {
    background-color: #2f2f2f;
    top: 50px;
  }
  to {
    background-color: #379eda;
    top: 50px;
  }
}

@keyframes anima4 {
  from {
    background-color: #379eda;
    top: 50px;
  }
  to {
    background-color: #2f2f2f;
    top: 300px;
  }
}

p {
  position: relative;
  left: 900px;
  top: 300px;
  width: 260px;
  height: 260px;
  /**/
  background-color: #2f2f2f;
  border: 3px solid #379eda;
  border-radius: 10px;
  padding: 10px;
  text-align: justify;
  /**/
  /* Animações que você quer executar em ordem */
  animation-name: anima1, anima2, anima3, anima4;
  /* Também pode abreviar só com 2s pra todos */
  animation-duration: 2s, 2s, 2s, 2s;
  /* Esse é o delay para começar cada uma das animações */
  animation-delay: 0s, 2s, 4s, 6s;
  /* Esse é o estilo da animation */
  animation-timing-function: ease-out, ease-in;
}
```
