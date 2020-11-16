# 18- Formatações para fontes

link: http://cfbcursos.com.br/css3-18-formatacoes-para-fontes/

Formatações para fontes

---

Font Face: 

Você baixa a fonte, dá um nome e usa.

```
@font-face {
  font-family: Poxa;
  src: url(POXADA.TTF)
}

```

---

Google Fonts

Você cola a referência no index.html:

```
<link rel="preconnect" href="https://fonts.gstatic.com" />
    <link
      href="https://fonts.googleapis.com/css2?family=Nunito&display=swap"
      rel="stylesheet"
    />
```

e usa: 

```
p {
  margin: 50px;
  color: #ffffff;
  font-family: Nunito, Nunito-Regular, Poxa;
  font-weight: normal;
  font-size: 50px;
  /* font-style: italic; */
  /* font-variant: small-caps; */
}
```

---

1- font-size; é o tamanho da fonte 
2- font-weight; controla o negrito
3- font-variant: small-caps; deixa a fonte com um estilo diferente
4- font-style: italic; controla o itálico
5- font-family; controla a família de fontes