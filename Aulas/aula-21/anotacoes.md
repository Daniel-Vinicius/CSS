# 21- Transformações 2D

link: http://cfbcursos.com.br/css3-21-transformacoes-2d/

**Transformações 2D**


As transformações 2D manipulam: `translação, rotação, escala, ângulo e origin` elementos através de suas 

propriedades: 

```
transform: translate(200px, 100px);
transform: rotate(45deg);
transform: scale(1),
transform: skew(20deg, 10deg); Primeiro o X e depois o Y */,
transform-origin: 100% 0%;
```


**HTML:**

```html
  <body>
    <div id="d1">Olá</div>
  </body>
```


**Css:**

```css
body {
  color: #fff;
  font-family: Arial, sans-serif;
  margin: 0px;
  padding: 0px;
  background-color: #2f2f2f;
}

#d1 {
  margin: 50px;
  width: 200px;
  height: 200px;
  border: 5px solid #fff;
  /* transform: translate(200px, 100px); */
  /* transform: rotate(45deg); */
  /* transform: scale(1) translate(200px, 100px); */
  /* transform: skewX(-20deg); */
  /* transform: skewY(10deg); */
  /* transform: skew(20deg, 10deg); Primeiro o X e depois o Y */
  /* transform: matrix(scaleX, skewY, skewX, scaleY, translateX, translateY); */
  /* transform: matrix(1.2 , -0.2, 0.3, 1.2, 400, 100); */
  /* transform-origin: 100% 0%; */
  /* transform: rotate(20deg); */
}

```