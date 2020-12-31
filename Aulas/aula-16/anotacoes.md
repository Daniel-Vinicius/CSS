# 16- Sombras

link: http://cfbcursos.com.br/css3-16-sombras-shadow/

Sombras:

1- Em textos a propriedade é a `text-shadow` que recebe os parâmetros:

1- Distância Horizontal 2- Distância Vertical 3- Blur 4- Cor

Exemplo: `text-shadow: 5px 5px 2px #0a91ff42;`

2- Em Elementos a propriedade é a `box-shadow` que recebe os mesmos parâmetros

Exemplo: `box-shadow: -8px -8px 0px #ffffff70;`

---

```css
body {
  background-color: #181717;
  margin: 0px;
  color: #fff;
  font-family: sans-serif;
}

h1 {
  margin-top: 75px;
  margin-left: 350px;

  color: #0a91ff;
  font-size: 50pt;
  font-family: Arial;
  text-shadow: 5px 5px 2px #0a91ff42;
  /* text-shadow: 5px 5px 2px #0a91ff42, 10px 10px 2px #ba0aff75; */
}

div {
  width: 300px;
  height: 300px;
  border: 10px solid #ffffff;
  border-radius: 10px;
  margin-left: 400px;
  background-color: #d82626;
  padding: 20px;

  box-shadow: -8px -8px 0px #ffffff70;
}
```
