# 41 - Animation - parte 2

[link](http://cfbcursos.com.br/css3-40-e-41-animacoes/)

**Animation - parte 2**

1- Animation

Além de From e To também é possível fazer animations com quadro chave. 
Dessa forma de fazer animations você diz o que quer fazer por porcentagem.
No exemplo abaixo eu disse que quando o tempo da animation chegar aos 50% eu quero que a propriedade top seja 50px.

Ex: 

```css
@keyframes anima {
  0% {
    left: 0px;
    top: 300px;
  }
  25% {
    left: 900px;
    top: 300px;
  }
  50% {
    left: 900px;
    top: 50px;
  }
  51% {
    background-color: #2f2f2f;
    top: 50px;
  }
  75% {
    background-color: #379eda;
    top: 50px;
  }
  100% {
    background-color: #2f2f2f;
    top: 300px;
  }
}
```

Novas Propriedades para executar animations:

* animation-iteration-count - Dita quantas vezes uma animação será executada pode receber números ou infinite.
* animation-play-state - Controla o estado da animação se ela está executando ou não. Pode receber os valores running que é o padrão ou também o paused.

* animation-direction - Controla o sentido da animação, pode receber os valores normal que é o padrão, reverse que troca o sentido da animação para anti-horário e alternate que alterna os dois sentidos a cada execução.

```css
p {
  animation-name: anima;
  animation-duration: 8s;
  animation-timing-function: ease-out, ease-in;
  /* Quantas vezes vai rodar? */
  animation-iteration-count: infinite;
  /* Controla o Estado da animação running é o padrão e tem o paused */
  animation-play-state: running;
  /* reverse troca o sentido, alternate troca o sentido a cada execução */
  animation-direction: alternate;
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

@keyframes anima {
  0% {
    left: 0px;
    top: 300px;
  }
  25% {
    left: 900px;
    top: 300px;
  }
  50% {
    left: 900px;
    top: 50px;
  }
  51% {
    background-color: #2f2f2f;
    top: 50px;
  }
  75% {
    background-color: #379eda;
    top: 50px;
  }
  100% {
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
  animation-name: anima;
  animation-duration: 8s;
  animation-timing-function: ease-out, ease-in;
  /* Quantas vezes vai rodar? */
  animation-iteration-count: infinite;
  /* Controla o Estado da animação running é o padrão e tem o paused */
  animation-play-state: running;
  /* reverse troca o sentido, alternate troca o sentido a cada execução */
  animation-direction: alternate;
}
```
