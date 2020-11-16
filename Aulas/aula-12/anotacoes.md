# 12- Cores RGB e transparência (alpha)

link: http://cfbcursos.com.br/css3-12-cores-rgb-transparencia/


Transparência

a transparencia funciona assim:

Ex: 

   `` background-color: rgba(217, 255, 0, 1); ``


Percebe que está rgba e o último número é entre 0 e 1
sendo 1 100% de opacidade e 0 transparente
logo 0.50 e 50% transparente entendeu?

Boa !!



````

p {
   color: #ffffff;
   font-family: sans-serif;
   background-color: #9a11f5;
   font-size: 20px;
   margin: 10px;
   border-radius: 20px;
   padding: 10px;
   max-width: 400px;
}

body {
    background-color: #181717
}

div {
    position: absolute;
    top: 60px;
    left: 300px;
    bottom:10px;
    width: 500px;
    height: 500px;
    background-color: rgba(217, 255, 0, 1);
    border-radius: 20px;
}

````