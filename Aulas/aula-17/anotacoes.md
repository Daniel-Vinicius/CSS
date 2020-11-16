# 17- Formatações de textos

link: http://cfbcursos.com.br/css3-17-formatacoes-para-textos-paragrafos/

Formatações de textos

---

color – cor
A propriedade color configura a cor do texto, podemos usar qualquer uma das formas de criação de cores que aprendemos.

Exemplo:

```
.p1 {
  color: #b40000;
}
```

---

text-align – alinhamento
Esta propriedade define o alinhamento do texto.


Os valores possíveis para text-align são:

left à Esquerda
right à Direita
center à Centro
justify justo entre a direita e a esquerda

Exemplo:

```
.p1 {
  color: #b40000;
  text-align: left;
}
```

---

text-decoration – Decoração
Configura o método de decoração do texto, a decoração são tipos de linhas como abaixo do texto, acima do texto ou riscado.

Os valores possíveis para text-decoration são:

none; sem linhas
underline; linha embaixo
overline; linha em cima
line-through; riscado

Exemplo: 

```
.p1 {
  color: #b40000;
  text-align: left;
  text-decoration: none;
}
```

---

text-transform – Transformações
Com esta propriedade podemos configurar letras em maiúsculas, minúsculas e primeiras letras em maiúsculo.

Os valores possíveis para text-transform são:

uppercase;  Converte em maiúsculo
lowercase;  Converte em minúsculo
capitalize; Converte as primeiras letras em maiúsculo

Exemplo: 

```
.p1 {
  color: #b40000;
  text-align: left;
  text-decoration: none;
  text-transform: uppercase;
}
```

---

text-indent – Endentação
Este parâmetro configura a endentação da primeira linha, definindo o tamanho do espaçamento do parágrafo.

Exemplo:

```
.p1 {
  color: #b40000;
  text-align: left;
  text-decoration: none;
  text-transform: uppercase;
  text-indent: 10px;
}
```

---

letter-spacing – Espaçamento entre as letras
Com letter-spacing podemos configurar o espaçamento entre as letras. O valor padrão é 0px.

Exemplo:

```
.p1 {
  color: #b40000;
  text-align: left;
  text-decoration: none;
  text-transform: uppercase;
  text-indent: 10px;
  letter-spacing: 1px;
}
```

---

line-height – Espaçamento entre as linhas
A propriedade line-height especifica distância entre as linhas de um texto. O valor padrão é 1 linha.

Exemplo:

```
.p1 {
  color: #b40000;
  text-align: left;
  text-decoration: none;
  text-transform: uppercase;
  text-indent: 10px;
  letter-spacing: 1px;
  line-height: 4;
}
```

---

direction – Direção do texto
Usando a propriedade direction podemos definir a direção do texto da esquerda para direita ou da direita para esquerda.

Podemos usar os valores:

rtl à Right To Left (Direita para Esquerda)
ltr à Left To Right (Esquerda para Direita)

Exemplo:

```
.p1 {
  color: #b40000;
  text-align: left;
  text-decoration: none;
  text-transform: uppercase;
  text-indent: 10px;
  letter-spacing: 1px;
  line-height: 4;
  direction: rtl;
}
```

---

word-spacing – Espaçamento entre as palavras
Configuração do espaçamento entre as palavras do texto. O valor padrão é 0px.

Exemplo:

```
.p1 {
  color: #b40000;
  text-align: left;
  text-decoration: none;
  text-transform: uppercase;
  text-indent: 10px;
  letter-spacing: 1px;
  line-height: 4;
  direction: rtl;
  word-spacing: 10px;
}
```

---

white-space
A propriedade white-space especifica como o texto dos elementos `<p>` vão se comportar.

Os valores possíveis para white-space são:

normal;  É o valor padrão
nowrap;  Não obdece seu limite

Exemplo:

```
.p1 {
  color: #b40000;
  text-align: left;
  text-decoration: none;
  text-transform: uppercase;
  text-indent: 10px;
  letter-spacing: 1px;
  line-height: 4;
  direction: rtl;
  word-spacing: 10px;
  white-space: normal;
}
```

---

overflow – CSS3 – Texto transbordado
A propriedade overflow configura como será o comportamento em casos de texto transbordado para fora dos limites especificados

Veja os valores possíveis.

visible -> O texto transbordado permanece visível, é a propriedade padrão.
hidden -> O texto transbordado fica oculto.
scroll -> Disponibiliza uma barra de rolagem para rolar o texto transbordado.
auto -> Automaticamente define se será mostrada ou não a barra de rolagem.

Exemplo:

```
.p1 {
  color: #b40000;
  text-align: left;
  text-decoration: none;
  text-transform: uppercase;
  text-indent: 10px;
  letter-spacing: 1px;
  line-height: 4;
  direction: rtl;
  word-spacing: 10px;
  white-space: normal;
  overflow: auto;
}
```

---

word-break – CSS3 – Quebra a palavra
Quebra a palavra caso ela não caiba no seu container, usando a separação de sílabas correta.

Exemplo:

```
.p1 {
  color: #b40000;
  text-align: left;
  text-decoration: none;
  text-transform: uppercase;
  text-indent: 10px;
  letter-spacing: 1px;
  line-height: 4;
  direction: rtl;
  word-spacing: 10px;
  white-space: normal;
  overflow: auto;
  word-break: break-all;
}
```

---

text-align-last – CSS3 – Alinhamento da última linha do texto
Define como será o alinhamento da última linha do parágrafo, independente do alinhamento ao texto.

Podemos usar right, left e center

Exemplo:

```
.p1 {
  color: #b40000;
  text-align: left;
  text-decoration: none;
  text-transform: uppercase;
  text-indent: 10px;
  letter-spacing: 1px;
  line-height: 4;
  direction: rtl;
  word-spacing: 10px;
  white-space: normal;
  overflow: auto;
  word-break: break-all;
  text-align-last:center;

}
```