4- background - Parte 1

link: http://cfbcursos.com.br/css3-4567-imagem-de-fundo-background-image/


**Podemos ter 2 ou mais imagens de background separando por vírgula tanto na hora de chamar quanto na hora de estilizar
**

**Geralmente a largura vem primeiro depois vem a altura


Eixo X é Horizontal e Y Vertical**


```
body {
  background-image: url(Imagem.png), url(Imagem2.jpg);
  background-size: 500px;
  background-repeat: no-repeat; // para não repetir a imagem
  background-position: 400px 100px, 100px 200px;
  /* background-repeat: repeat-x; */
  /* background-repeat: repeat-y; */
  /* background-size: 200px 50px; // 400px na largura e 50 px na altura*/
  background-color: #111111;
}

p {
    background-image: url(Imagem2.jpg);
    background-repeat: repeat-x;
    background-size: 200px;
    background-position: 50px 0px;
    font-size: 40px;
    color: #FFF;
    font-family: sans-serif;
}

```