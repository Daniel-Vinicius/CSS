# 25- Outline

link: http://cfbcursos.com.br/css3-25-outline/

**Outline**


propriedade:

```css
  outline: solid 10px #c04242;
  outline-offset: 10px;
```

**Html:**

```html
<!DOCTYPE html>
<html lang="pt-br">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <link rel="stylesheet" href="style.css" />
    <title>Curso de CSS</title>
  </head>
  <body>
    <div id="d1">Div 1</div>
    <div id="d2">Div 2</div>
  </body>
</html>

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

div {
  width: 300px;
  height: 300px;
  background-color: #c04242;
  border: 15px solid #ffffff;
  border-radius: 10px;
  margin-left: 200px;
  margin-top: 70px;
  padding: 10px;
  text-align: center;
  display: inline-block;
  outline: solid 10px #c04242;
  outline-offset: 10px;
}
```
