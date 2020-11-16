# 19- Formatações para links

link: http://cfbcursos.com.br/css3-19-formatacoes-para-links/

Formatações para links:

```
body {
  background-color: #181717;
  color: #fff;
  font-family: Arial, sans-serif;
}

#primeiro {
  margin-top: 150px;
}

a {
  font-size: 30px;
  margin-bottom: 20px;
  margin-left: 500px;
  display: block;
  color: #ffffff;
  text-decoration: none;
}

a:link { 
  /*Não Visitado*/
  color: #5d08cc;
}

a:visited {
  /*Visitado*/
  color: #67cc08;
}

/* a:active {
  Momento do clique não vísivel
  color: #cecb20;
} 
*/

a:hover {
  /*Mouse em Cima*/
  transition: 2s;
  color: #089cff;
}

```