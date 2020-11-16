# 11- bordas (border) - Parte 4

link: http://cfbcursos.com.br/css3-11-imagens-nas-bordas-border-image/

Border Image

O border image funciona assim: primeiro você passa onde está a imagem,
depois você passa qual é o fatiamento da imagem no caso o fatiamento e 30 porque cada bolinha da imagem tem 30 px
e por último você passa ou round ou stretch sendo q round repete o fatiamento até preencher todo o conteúdo e 
stretch o estica

````
p {
   color: #ffffff;
   font-family: sans-serif;
   background-color: #9a11f5;
}

body {
    background-color: #181717
}

p {
    border: 30px solid;
    border-image: url(Imagem.webp) 30 round;
    border-radius: 90px;
}
````