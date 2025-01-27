# Flex

Para o Align-Items e o Justify-Content funcionarem é necessário uma altura e largura definida no container.
As propriedades Align-Items e o Justify-Content devem ser colocadas nos containers e dessa forma alinhando seus filhos.

Para o height: 100% funcionar em containers você deve fazer isso:

```css
html, body {
  margin: 0;
  height: 100%;
}
```

**CSS**

```css
body {
  color: #f8f8f8;
  font-family: Arial, sans-serif;
  padding: 0px;
  background-color: #222222;
  font-weight: 500;
  font-size: 15px;
}

html, body {
  margin: 0;
  height: 100%;
}

.container {
  display: flex;
  justify-content: center;
  align-items: center;
  flex-wrap: wrap;
  height: 100%;
  width: 100%;
  flex-direction: column;
}

.hs {
  display: flex;
  flex-direction: row;
  justify-content: flex-start;
  align-items: flex-start;
  min-width: 200px;
  min-height: 100px;
  color: #ff6347;
}

.divs {
  display: flex;
  flex-direction: row;
  min-width: 400px;
  min-height: 200px;
  align-items: flex-start;
  justify-content: flex-start
}

.div {
  border: 5px solid #ffffff;
  background-color: #ff6347;
  border-radius: 5px;
  margin: 20px;
  /**/
  display: flex;
  justify-content: center;
  align-items: center;
  width: 200px;
  height: 100px;
  min-width: 200px;
  max-width: 200px;
}

.input {
  min-width: 320px;
  min-height: 30px;
  border-radius: 10px;
  border: 0px solid #ff6347;
  outline: none;
  align-items: center;
  justify-content: center;
  background-color: #ffffff;
  color: #ff6347;
}

.input::placeholder {
  text-align: center;
  color: #ff6347;
  font-weight: 500;
  opacity: 0.8;
}

.button {
  min-width: 200px;
  min-height: 40px;
  border-radius: 10px;
  border: none;
  outline: none;
  background-color: #ff6347;
  color: #fff;
  cursor: pointer;
}

.button:hover {
  transition: 0.5s;
  background-color: #ffffff;
  color: #ff6347;
}

::selection {
  background-color: #ffb4b4;
  color: #ffffff;
}
```