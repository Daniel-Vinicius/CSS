# 22- Transformações 3D

link: http://cfbcursos.com.br/css3-22-transformacoes-3d/

**Transformações 3D**


As transformações 3D manipulam: `translação, rotação, escala, ângulo, origin e perpectiva` elementos através de suas 

propriedades: 

```css

  perspective: 150px; // se coloca no container, controla perspectiva
  
  transform: translate(200px, 100px);
  transform: rotate(45deg);
  transform: scale(1);
  transform: skew(20deg, 10deg);  // Primeiro o X e depois o Y
  transform-origin: 100% 0%;

```


**Script:**

``` html
    <script>
      var y,
        n = 0,
        ny = 0,
        rotYINT;

      function rotateYDIV() {
        y = document.getElementById("d1");
        clearInterval(rotYINT);
        rotYINT = setInterval("startYRotate()", 10);
      }

      function startYRotate() {
        ny = ny + 1;
        y.style.transform = "rotateY(" + ny + "deg)";
        if (ny == 180 || ny >= 360) {
          clearInterval(rotYINT);
          if (ny >= 360) {
            ny = 0;
          }
        }
      }
    </script>

```


**Css:**

```css
body {
  color: #fff;
  font-family: Arial, sans-serif;
  margin: 0px;
  padding: 0px;
  background-color: #2f2f2f;

  perspective: 150px
}

#d1 {
  margin-left: 40%;
  margin-right: -50%;
  margin-top: 50px;

  width: 200px;
  height: 200px;
  border: 5px solid #fff;
  border-radius: 100px;
  background: linear-gradient(to left, #0051ff, #91e20e, #ae00ff);

  transform: translate(200px, 200px);
  transform-origin: 200px 200px;
}


```