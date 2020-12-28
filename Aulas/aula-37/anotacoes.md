# 37 - Continuação pseudo-elementos (first-letter, fisrt-line, selection)

[link](http://cfbcursos.com.br/css3-36-e-37-pseudo-elementos-after-e-before/)

**Continuação pseudo-elementos (first-letter, fisrt-line, selection)**

1- Selection

Quando você passa o mouse sobre um texto e ele faz algo como por exemplo mudar de cor.

Ex: 

```css
::selection {
  color: #1f74f3;
}
```

2- Primeira linha e Primeira Letra

Aplica alguma estilização a primeira linha ou letra.

Ex:

```css
p::first-letter {
  color: #1f74f3;
}

p::first-line {
  background-color: #1f74f356;
}
```

**Html:**

```html
<body>
  <div>
    <p>Lorem, ipsum dolor sit amet consectetur adipisicing elit. Mollitia nobis optio laborum alias esse, ad repellat
      labore qui rem commodi autem consectetur amet animi voluptates ex cupiditate ducimus inventore dolorum. Lorem
      ipsum
      dolor sit amet consectetur adipisicing elit. Nam ea temporibus illo et soluta ab, doloribus ratione? Voluptatibus
      harum, enim sequi soluta rem iure quae quaerat ea cumque? Soluta, id? Lorem ipsum, dolor sit amet consectetur
      adipisicing elit. Non inventore illum mollitia voluptate atque at quo, eaque eius laudantium animi officia earum
      sequi rem optio nemo iusto porro similique recusandae? Lorem ipsum dolor sit amet consectetur adipisicing elit.
      Molestiae, laboriosam. Dignissimos expedita necessitatibus vel dolor reiciendis at, natus enim nihil illum
      aspernatur minima voluptatem pariatur excepturi, minus obcaecati officiis rerum.</p>
    <p>Algo de CSS Aleatório</p>
    <p>Algo de CSS Aleatório</p>
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
  flex-direction: column;
  align-items: center;
}

p {
  font-size: 14px;
}

p::first-letter {
  color: #1f74f3;
}

p::first-line {
  background-color: #1f74f356;
}

::selection {
  color: #1f74f3;
}
```
