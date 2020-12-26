# 31- Display Flex Desafio

[link](http://cfbcursos.com.br/css3-31-desafiodisplayflex/)

**Display Flex Desafio**

Consegui Fazer em Meia Hora

**Html:**

```html
<body>
  <header>
    <h1>Cabeçalho do site</h1>
  </header>

  <nav>
    <a>Menu 1</a>
    <a>Menu 2</a>
    <a>Menu 3</a>
    <a>Menu 4</a>
    <a>Menu 5</a>
    <a>Menu 6</a>
  </nav>

  <section>
    <div>CFB1</div>
    <div>CFB2</div>
    <div>CFB3</div>
    <div>CFB4</div>
    <div>CFB5</div>
    <div>CFB6</div>
    <div>CFB7</div>
    <div>CFB8</div>
    <div>CFB9</div>
    <div>CFB10</div>
  </section>

  <footer>
    <p>Canal Fessor Bruno</p>
  </footer>

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
  font-size: 20px;
}

h1 {
  text-align: center;
}

.nav {
  display: flex;
  flex-wrap: wrap;
  background-color: #b93232;
  padding: 10px;
  height: 100px;
  margin-bottom: 60px;
  justify-content: center;
  align-items: center;
}

.nav>a {
  font-size: 20px;
  cursor: pointer;
  margin-right: 40px;
  width: 100px;
  min-width: 100px;
  display: flex;
  justify-content: center;
  align-items: center;
}

.section {
  display: flex;
  align-items: center;
  flex-wrap: wrap;
  justify-content: center;
}

.div {
  border: 5px solid #da2222;
  border-radius: 5px;
  width: 200px;
  height: 100px;
  min-width: 200px;
  max-width: 200px;
  margin: 20px;
  display: flex;
  justify-content: center;
  align-items: center;
}

.footer {
  display: flex;
  justify-content: center;
  background-color: #e2e2e2;
  flex-grow: 1;
  color: #000000;
  font-weight: 600;
  min-width: 100%;
}
```
