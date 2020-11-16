# 13- Margens e centralização

link: http://cfbcursos.com.br/css3-13-margens-e-centralizacao/

Margens:

São Basicamente o código Abaixo

```
#d1 {
    background-color: #0ea7ff;

    margin-top: 120px;
    margin-right: 60px;
    margin-bottom: 100px;
    margin-left: 70px;

    /*
    Também pode-se fazer assim:

    margin: 120px 60px 100px 70px;

    equivalente há:

    margin-top: 120px;
    margin-right: 60px;
    margin-bottom: 100px;
    margin-left: 70px;

    */
}
```

Alinhar elementos ao centro usando Margen Automática:

Deve-se estar setado o height e o width

e depois é só colocar margin Automática
Como no código abaixo

```
div {

    height: 500px;
    width: 500px;
    margin: auto;
}
```

Alinhar texto ao centro:

Note que estamos alinhando o texto ao centro e não o Parágrafo

```
p {
   text-align: center;
}
```


Retirar margin padrão da página: 

```
body {
    margin: 0px;
}

```