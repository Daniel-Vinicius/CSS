# 24- Formatações para Tabelas

link: http://cfbcursos.com.br/css3-24-formatando-tabelas/

**Formatações para Tabelas**

propriedades:

``` css
  width: 500px;
  table-layout: fixed;
  border-collapse: collapse;
```

**Html:**

```html
<table>
      <tr>
        <th>Peça</th>
        <th>Valor</th>
        <th>Estoque</th>
      </tr>
      <tr>
        <td>Processador</td>
        <td>R$ 800,00</td>
        <td>30</td>
      </tr>
      <tr>
        <td>Memória</td>
        <td>R$ 150,00</td>
        <td>55</td>
      </tr>
      <tr>
        <td>HD</td>
        <td>R$ 320,00</td>
        <td>20</td>
      </tr>
      </table>

```

**Css:**

```css
body {
  color: #fff;
  font-family: Arial, sans-serif;
  padding: 0px;
  background-color: #2f2f2f;
  font-weight: 500;
  font-size: 20px;
}

 th {
  border: 1px solid #ffffff;
  padding: 5px;
  color: #03a6cf;
  font-weight: bold;
  background-color: #ffffff
}

td {
  border: 1px solid #ffffff;
  padding: 10px;
  color: #FFFFFF;
  font-weight: lighter;
}

table {
  width: 500px;
  table-layout: fixed;
  border-collapse: collapse;
  margin: auto
}

tr:nth-child(even) {
  background-color: #007e7e
}

div {
  height: 200px;
  border: none;
  border-radius: 10px;
  width: 200px;

  margin: 30px;
  margin-left: 500px;
  padding: 30px;

  background: #555555
}

div:nth-child(even) {
  background: linear-gradient(to left, #0051ff, #91e20e, #ae00ff);}

```
