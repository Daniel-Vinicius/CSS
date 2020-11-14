9- bordas (border) - Parte 2

link: http://cfbcursos.com.br/css3-10-bordas-arredondadas-border-radius/

Border Radius

````

p {
   color: #ffffff;
   font-family: sans-serif;
}

body {
    background-color: #181717
}

#d1, #d2 {
    margin: 60px;
    background-color: #8003d3;
    width: 400px;
    height: 100px;
}

#d1 {
    float: left;
    padding: 20px;

    border: #ffffff solid 10px;
    border-radius: 40px;
}

#d2 {
    float: right;
    padding: 20px;

    border: #ffffff solid 10px;
    border-radius: 2px 30px 20px 10px;
 /* border-radius: 60% 10% 30% 20% */
}

/*
Border Radius

1- Superior Esquerdo   2- Superior Direito   3- Inferior Direito   4- Inferior Esquerdo
/*

````