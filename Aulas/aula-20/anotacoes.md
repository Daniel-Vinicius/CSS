# 20- Criando menu HTML links + CSS

link: http://cfbcursos.com.br/css3-20-criando-um-menu/

**Criando um Menu:**

**HTML:**

```
    <nav>
      <a target="_blank" href="https://google.com">Home</a>
      <a target="_blank" href="https://google.com">Preços</a>
      <a target="_blank" href="https://google.com">Contato</a>
      <a target="_blank" href="https://google.com">Quem Somos</a>
      <a target="_blank" href="https://google.com">Trabalhe conosco</a>
      <a target="_blank" href="https://google.com">Clientes</a>
    </nav>
```

**Index:**

```
      <object id="objMenu" data="menu.html"></object>

```

**Css:**

```
body {
  color: #fff;
  font-family: Arial, sans-serif;
  margin: 0px;
  background: url(Imagem2.jpg) no-repeat;
  background-position: 100px 0px;
  background-size: 1024px;
  background-color: #03a4eeb9;
}

#objMenu {
  width: 100%;
  margin: 0px;
  padding: 0px;
}

a {
  text-decoration: none;
  background-color: #ffffff;
  color: #03a4ee;
  padding: 0px;
  margin: 0px;
  display: table-cell;
  text-align: center;
  vertical-align: middle;
  width: 200px;
  height: 50px;
  font-size: 15px;
}

a:hover {
  transition: 0.5s;
  color: #FFFFFF;
  background-color: #03a4eeb9;
}

nav {
  margin: 10px;
  width: 1200px;
  height: 50px;
  border: 5px solid #03a4ee;
  border-radius: 4px;
}

```