15- Preenchimentos Gradientes

link: http://cfbcursos.com.br/css3-15-cores-gradientes/

```
body {
  background-color: #181717;
  margin: 0px;
  color: #fff;
  font-family: sans-serif;
}

#d1 {
  border: 10px solid #ffffff;
  border-radius: 10px;
  margin: auto;
  margin-top: 50px;
  padding: 10px;
  width: 300px;
  height: 300px;

  background: linear-gradient(47deg, #0051ff 0%, #91e20e 40%, #ae00ff 80%);

  /*

  47deg = 47 graus de angulos

  Também é possivel fazer isso:

    background: linear-gradient(to top, #0051ff, #91e20e, #ae00ff);
    background: linear-gradient(to right, #0051ff, #91e20e, #ae00ff);
    background: linear-gradient(to bottom, #0051ff, #91e20e, #ae00ff);
    background: linear-gradient(to left, #0051ff, #91e20e, #ae00ff);

 */
}

#d2 {
  border: 10px solid #ffffff;
  border-radius: 10px;
  margin: auto;
  margin-top: 20px;
  margin-bottom: 50px;
  padding: 10px;
  width: 300px;
  height: 300px;

  background: radial-gradient(#0ddb9d 0%, #ff0278 60%, #000000 80%);
}

```