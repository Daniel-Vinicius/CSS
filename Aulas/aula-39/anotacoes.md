# 39 - Transition - parte 2

[link](http://cfbcursos.com.br/css3-38-e-39-transicoes/)

**Transition - parte 2**

1- Transition Delay

Dá um Delay pra começar e parar uma Transition

2- Aplicar Transitions Diferentes para cada propriedade
```css
div { transition: color 0.8s, background-color 0.1s, transform 1s; }
```

Ex: 

```css
p {
  width: 300px;
  height: 250px;
  border: 5px solid #ff891b;
  border-radius: 10px;
  padding: 10px;
  text-align: justify;
  transition: color 0.8s, background-color 0.1s, transform 1s; /*2- Aplicar Transitions Diferentes para cada propriedade*/
  transition-delay: 1s; /*1- Transition Delay*/
  transition-timing-function: ease-out;
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
  <div>
    <div class="spin"></div>
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
  flex-direction: column;
}

p {
  width: 300px;
  height: 250px;
  border: 5px solid #ff891b;
  border-radius: 10px;
  padding: 10px;
  text-align: justify;
  transition: color 0.8s, background-color 0.1s, transform 1s;
  transition-delay: 1s;
  transition-timing-function: ease-out;
}

p:hover {
  background-color: #172496;
  color: #ff891b;
  transform: rotate(360deg);
}

/* Spinner */

.spin {
  width: 60px;
  height: 60px;
  border: 8px solid #535353;
  border-radius: 100%;
  border-left-color: #e65e1f;
  animation: spin 1s linear infinite;
  margin-top: 30px;
}

@keyframes spin {
  to {
    transform: rotate(360deg);
  }
}
```
