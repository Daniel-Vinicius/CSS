# 43 - Resize

[link](http://cfbcursos.com.br/css3-43-resize/)

**Resize**

1- Resize

Resize faz com que uma div possa ser redimensionada em tempo de execução.

Existe a Propriedade `resize: both;`

Também recebe os valores horizontal e vertical

Você pode definir um valor mínimo para width ou height com min-width ou min-height

Ex: 

```css
div {
  background-color: #d63f3f;
  min-width: 300px;
  width: 300px;
  height: 300px;
  border-radius: 10px;
  padding: 10px;
  resize: both; /* Aquiiii */
  overflow: auto;
  display: flex;
  margin: 100px;
}
```

**Html:**

```html
  <section>
    <div>Lorem ipsum dolor sit amet consectetur adipisicing elit. Asperiores, inventore voluptate eum ad laborum ex,
      minus
      ab nisi adipisci est, atque ea expedita incidunt voluptates voluptatem exercitationem consequuntur quasi
      repudiandae?
      Lorem ipsum dolor sit amet consectetur adipisicing elit. Asperiores, inventore voluptate eum ad laborum ex, minus
      ab nisi adipisci est, atque ea expedita incidunt voluptates voluptatem exercitationem consequuntur quasi
      repudiandae?
      Lorem ipsum dolor sit amet consectetur adipisicing elit. Asperiores, inventore voluptate eum ad laborum ex, minus
      ab nisi adipisci est, atque ea expedita incidunt voluptates voluptatem exercitationem consequuntur quasi
      repudiandae?
      Lorem ipsum dolor sit amet consectetur adipisicing elit. Asperiores, inventore voluptate eum ad laborum ex, minus
      ab nisi adipisci est, atque ea expedita incidunt voluptates voluptatem exercitationem consequuntur quasi
      repudiandae?</div>
    <div class="img">
      <img src="img.png" alt="">
    </div>
  </section>

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

section {
  display: flex;
  justify-content: center;
  flex-wrap: wrap;
}

div {
  background-color: #d63f3f;
  min-width: 300px;
  width: 300px;
  height: 300px;
  border-radius: 10px;
  padding: 10px;
  resize: both;
  overflow: auto;
  display: flex;
  margin: 100px;
}

div::-webkit-scrollbar-track {
  background-color: #2e2929;
}

div::-webkit-scrollbar {
  width: 6px;
}

div::-webkit-scrollbar-thumb {
  background-color: #ff8888;
}

.img>img {
  width: 100%;
  height: 100%;
}

.img {
  overflow: hidden;
  background-color: transparent;
}

div:hover {
  border: 3px solid #ffffff;
}
```
