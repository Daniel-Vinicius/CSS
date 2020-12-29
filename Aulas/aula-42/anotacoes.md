# 42 - Colunas

[link](http://cfbcursos.com.br/css3-42-colunas/)

**Colunas**

1- Colunas

Colunas Dividem Texto Verticalmente.
Podemos controlar espaçamento entre as colunas, colocar linhas e quantidade de colunas

Ex: 

```css
p {
  column-gap: 50px;
  column-rule: 5px outset #730aeb;
  columns: 4;
}
```

**Html:**

```html
<body>
  <p>Lorem ipsum dolor, sit amet consectetur adipisicing elit. Sed placeat id veniam rerum dicta ipsa error at laborum,
    sint dolorum architecto harum quibusdam fugiat veritatis velit distinctio, cumque esse laboriosam.
    Lorem ipsum dolor, sit amet consectetur adipisicing elit. Sed placeat id veniam rerum dicta ipsa error at laborum,
    sint dolorum architecto harum quibusdam fugiat veritatis velit distinctio, cumque esse laboriosam.
    Lorem ipsum dolor, sit amet consectetur adipisicing elit. Sed placeat id veniam rerum dicta ipsa error at laborum,
    sint dolorum architecto harum quibusdam fugiat veritatis velit distinctio, cumque esse laboriosam.
    Lorem ipsum dolor, sit amet consectetur adipisicing elit. Sed placeat id veniam rerum dicta ipsa error at laborum,
    sint dolorum architecto harum quibusdam fugiat veritatis velit distinctio, cumque esse laboriosam.
    Lorem ipsum dolor, sit amet consectetur adipisicing elit. Sed placeat id veniam rerum dicta ipsa error at laborum,
    sint dolorum architecto harum quibusdam fugiat veritatis velit distinctio, cumque esse laboriosam.
    Lorem ipsum dolor, sit amet consectetur adipisicing elit. Sed placeat id veniam rerum dicta ipsa error at laborum,
    sint dolorum architecto harum quibusdam fugiat veritatis velit distinctio, cumque esse laboriosam.
    Lorem ipsum dolor, sit amet consectetur adipisicing elit. Sed placeat id veniam rerum dicta ipsa error at laborum,
    sint dolorum architecto harum quibusdam fugiat veritatis velit distinctio, cumque esse laboriosam.
    Lorem ipsum dolor, sit amet consectetur adipisicing elit. Sed placeat id veniam rerum dicta ipsa error at laborum,
    sint dolorum architecto harum quibusdam fugiat veritatis velit distinctio, cumque esse laboriosam.
    Lorem ipsum dolor, sit amet consectetur adipisicing elit. Sed placeat id veniam rerum dicta ipsa error at laborum,
    sint dolorum architecto harum quibusdam fugiat veritatis velit distinctio, cumque esse laboriosam.
    Lorem ipsum dolor, sit amet consectetur adipisicing elit. Sed placeat id veniam rerum dicta ipsa error at laborum,
    sint dolorum architecto harum quibusdam fugiat veritatis velit distinctio, cumque esse laboriosam.
    Lorem ipsum dolor, sit amet consectetur adipisicing elit. Sed placeat id veniam rerum dicta ipsa error at laborum,
    sint dolorum architecto harum quibusdam fugiat veritatis velit distinctio, cumque esse laboriosam.
    Lorem ipsum dolor, sit amet consectetur adipisicing elit. Sed placeat id veniam rerum dicta ipsa error at laborum,
    sint dolorum architecto harum quibusdam fugiat veritatis velit distinctio, cumque esse laboriosam.</p>
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

p {
  position: relative;
  left: 175px;
  top: 0px;
  width: 1200px;
  height: 500px;
  border: 1px solid #ffffff;
  border-radius: 10px;
  padding: 10px;
  text-align: justify;
  columns: 4;
  column-gap: 50px;
  column-rule: 5px outset #730aeb;
}
```
