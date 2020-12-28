# 38 - Transition - parte 1

[link](http://cfbcursos.com.br/css3-38-e-39-transicoes/)

**Transition - parte 1**

1- Transition

Faz uma transição e recebe um valor em segundos. Pode ser configurada mais detalhadamente com o transition-timing-function que por sua vez controla o estilo de uma transição. Por exemplo uma transição que começa rápido e termina devagar como o ease-out ou ao contrário ease-in. Uma que vai sempre na mesma velocidade como linear ou uma que vai rápido no meio, o padrão como o ease.

Ex: 

```css
p {
  width: 300px;
  height: 250px;
  border: 5px solid #ff891b;
  border-radius: 10px;
  padding: 10px;
  text-align: justify;
  transition: 2s;
  /* É o padrão, o melhor, ease e ease-in-out */
  /* transition-timing-function: ease; */
  /* Linear vai na mesma velocidade */
  /* transition-timing-function: linear; */
  /* Easy IN vai devagar no começo */
  /* transition-timing-function: ease-in; */
  /* Easy OUT vai devagar no final */
  /* transition-timing-function: ease-out; */
  /* Cubic Bezier personalizável */
  /* transition-timing-function: cubic-bezier(0.075, 0.82, 0.165, 1); */
}

p:hover {
  width: 500px;
  height: 120px;
  background-color: #172496;
  color: #ff891b;
}
```

**Html:**

```html
<body>
  <div>
    <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Asperiores, corrupti excepturi. Error neque temporibus
      porro, est facere totam consequatur repudiandae alias at in atque fuga accusamus, perferendis exercitationem
      minima
      culpa.
      Lorem ipsum dolor sit amet consectetur adipisicing elit. Asperiores, corrupti excepturi. Error neque temporibus
      porro, est facere totam consequatur repudiandae alias at in atque fuga accusamus, perferendis exercitationem
      minima
      culpa.</p>
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
}

div {
  display: flex;
  align-items: center;
  justify-content: center;
}

p {
  width: 300px;
  height: 250px;
  border: 5px solid #ff891b;
  border-radius: 10px;
  padding: 10px;
  text-align: justify;
  transition: 2s;
  /* É o padrão, o melhor, ease e ease-in-out */
  /* transition-timing-function: ease; */
  /* Linear vai na mesma velocidade */
  /* transition-timing-function: linear; */
  /* Easy IN vai devagar no começo */
  /* transition-timing-function: ease-in; */
  /* Easy OUT vai devagar no final */
  /* transition-timing-function: ease-out; */
  /* Cubic Bezier personalizável */
  /* transition-timing-function: cubic-bezier(0.075, 0.82, 0.165, 1); */
}

p:hover {
  width: 500px;
  height: 120px;
  background-color: #172496;
  color: #ff891b;
}
```
