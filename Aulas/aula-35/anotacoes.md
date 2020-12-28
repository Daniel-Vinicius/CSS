# 35 - Overflow

[link](http://cfbcursos.com.br/css3-35-overflow/)

**Overflow**

1- Overflow
Controla o comportamento do container em relação aos elementos que extrapolam o tamanho do container.

Valores Possíveis:

```css
.container {
  overflow: visible;  /* é o valor padrão e mostra o conteúdo que extrapolar o container */   
  overflow: hidden;   /* não mostra o conteúdo que extrapolar o container */  
  overflow: scroll;   /* mostra uma barra de rolagem para rolar e visualizar o conteúdo do container */
  overflow: auto;     /* mostra uma barra de rolagem caso necessário  */
}
```

2- Estilizar a Barra de Rolagem

```css
/* Escolhe a Cor de Fundo da Barra de rolagem */
#d1::-webkit-scrollbar-track {
  background-color: #2e2929;
}

/* Escolhe a Largura da Barra de rolagem */
#d1::-webkit-scrollbar {
  width: 6px;
}

/* Escolhe a Cor da Barra de rolagem ativa */
#d1::-webkit-scrollbar-thumb {
  background-color: #9410c9;
}
```

**Html:**

```html
<body>
  <div id="d1">
    <img id="img1" src="imga.jpg">
    <p>Em linguística, a noção de texto é ampla e ainda aberta a uma definição mais precisa. Grosso modo, pode ser
      entendido como manifestação linguística das ideias de um autor, que serão interpretadas pelo leitor de acordo com
      seus conhecimentos linguísticos e culturais. Seu tamanho é variável.
      O interesse pelo texto como objeto de estudo gerou vários trabalhos importantes de teóricos da Linguística
      Textual, que percorreram fases diversas cujas características principais eram transpor os limites da frase
      descontextualizada da gramática tradicional e ainda incluir os relevantes papéis do autor e do leitor na
      construção de textos.
      Um texto pode ser escrito ou oral e, em sentido lato, pode ser também não verbal.
      Texto crítico é uma produção textual que parte de um processo reflexivo e analítico gerando um conteúdo com
      crítica construtiva e bem fundamentada.
      Em artes gráficas, o texto é a parte verbal, linguística, por oposição às ilustrações.
      Todo texto tem que ter alguns aspectos formais, ou seja, tem que ter estrutura, elementos que estabelecem relação
      entre si. Dentro dos aspectos formais temos a coesão e a coerência, que dão sentido e forma ao texto.Embora a
      coesão não seja condição suficiente para que enunciados se constituam em textos,
      são os elementos coesivos que lhes dão maior legibilidade e evidenciam as relações entre seus diversos
      componentes, a coerência depende da coesão.</p>
  </div>
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
  overflow: auto;
}

#img1 {
  border: 5px solid #9410c9;
  border-radius: 10px;
}

#d1 {
  border: 8px solid #ffffff;
  border-radius: 10px;
  padding: 20px;
  margin-top: 20px;
  /**/
  width: 300px;
  height: 400px;
  position: absolute;
  left: 40%;
  overflow: auto;
  display: flex;
  flex-direction: column;
}

/* Escolhe a Cor de Fundo da Barra de rolagem */

#d1::-webkit-scrollbar-track {
  background-color: #2e2929;
}

/* Escolhe a Largura da Barra de rolagem */

#d1::-webkit-scrollbar {
  width: 6px;
}

/* Escolhe a Cor da Barra de rolagem ativa */

#d1::-webkit-scrollbar-thumb {
  background-color: #9410c9;
}

/* Body */

body::-webkit-scrollbar-track {
  background-color: #2e2929;
}

body::-webkit-scrollbar {
  width: 6px;
}

body::-webkit-scrollbar-thumb {
  background-color: #9410c9;
}
```
