# 49 - @media - Layout Responsivo - Parte 2

[link](http://cfbcursos.com.br/css3-484950-media-layouts-responsivos/)

**@media**

@media é uma propriedade css que retorna true ou false com base em verificações e caso seja verdadeira aplica alguma formatação a algum elemento.

Nesta segunda aula treinamos um pouco da propriedade @media.


**Html:**

```html
<body>
  <section>
    <nav>
      <ul>
        <li>Menu 1</li>
        <li>Menu 2</li>
        <li>Menu 3</li>
      </ul>
    </nav>
    <article>
      <h1>Canal Fessor Bruno</h1>
      <p>As regras media permitem configurar diferentes regras CSS para diferentes tipos de mídia, diante da necessidade
        de facilicar a configuração do site para se adaptar bem em dispositivos de diferentes tamanhos, dai vem o
        conceito de design responsivo ou layout responsivo.

        Pode ter várias configurações de estilo para um mesmo site, para que se adapte aos diversos dispositivos,
        podemos ter estilos para computadores, celulares, impressão, televisão, tablets, etc.</p>
      <div>
        <h1>Playlists publicadas</h1>
        <ul>
          <li>C++</li>
          <li>HTML / HTML5</li>
          <li>PHP</li>
          <li>CSS</li>
          <li>Photoshop</li>
          <li>Flash</li>
          <li>Unity</li>
          <li>Projeto Site Completo</li>
          <li>NostalWindows</li>
        </ul>
      </div>

      <div>
        <h1>Em breve...</h1>
        <ul>
          <li>Arduino</li>
          <li>Javascript</li>
          <li>jQuery</li>
          <li>C#</li>
          <li>Desenvolvimento para Android</li>
          <li>Python</li>
          <li>Mais C++</li>
          <li>Mais Unity</li>
          <li>SketchUp</li>
          <li>Autocad</li>
        </ul>
      </div>

    </article>
  </section>
</body>
```

**Css:**

```css
body {
  color: #fff;
  font-family: Arial, sans-serif;
  background-color: #2f2f2f;
  font-weight: 500;
}

nav {
  width: 200px;
  float: left;
}

nav ul {
  margin: 0px;
  padding: 0px;
}

nav li {
  background-color: #dd5555;
  color: #fff;
  border: 1px solid #dddddd;
  border-radius: 4px;
  list-style-type: none;
  margin: 4px;
  padding: 2px;
}

article {
  margin-left: 210px;
}

@media screen and (min-width: 0px) and (max-width: 500px) {
  nav {
    width: 100%;
  }
  article {
    margin-left: 4px;
  }
  article p {
    text-align: justify;
  }
  nav li {
    font-size: 20px;
  }
}

@media screen and (min-width: 501px) and (max-width: 800px) {
  nav li {
    font-size: 20px;
  }
  article div {
    float: left;
  }
}
```

<h3> As propriedades possíveis de utilização como valor para expressão de verificação em <strong> @media </strong> estão mostradas na tabela a seguir.
</h3>

  <table>
    <tbody>
      <tr>
        <td><strong>Value</strong></td>
        <td><strong>Description</strong></td>
      </tr>
      <tr>
        <td>aspect-ratio</td>
        <td>A proporção entre a largura ea altura da janela de visualização</td>
      </tr>
      <tr>
        <td>color</td>
        <td>O número de bits por componente de cor para o dispositivo de saída</td>
      </tr>
      <tr>
        <td>color-index</td>
        <td>Quantidade de cores que o dispositivo pode exibir</td>
      </tr>
      <tr>
        <td>device-aspect-ratio</td>
        <td>A proporção entre a largura ea altura que o dispositivo pode exibir</td>
      </tr>
      <tr>
        <td>device-height</td>
        <td>Medida da altura do dispositivo, por exemplo a tela do computador</td>
      </tr>
      <tr>
        <td>device-width</td>
        <td>Medida da largura do dispositivo, por exemplo a tela do computador</td>
      </tr>
      <tr>
        <td>grid</td>
        <td>Se o dispositivo é um grid ou bitmap</td>
      </tr>
      <tr>
        <td>height</td>
        <td>Altura da janela</td>
      </tr>
      <tr>
        <td>max-aspect-ratio</td>
        <td>A proporção máxima entre largura e altura da área da tela</td>
      </tr>
      <tr>
        <td>max-color</td>
        <td>O número de bits máximo por componente de cor para o dispositivo de saída</td>
      </tr>
      <tr>
        <td>max-color-index</td>
        <td>Quantidade máxima de cores que o dispositivo pode exibir</td>
      </tr>
      <tr>
        <td>max-device-aspect-ratio</td>
        <td>A proporção máxima entre a largura ea altura que o dispositivo pode exibir</td>
      </tr>
      <tr>
        <td>max-device-height</td>
        <td>Medida máxima da altura do dispositivo, por exemplo a tela do computador</td>
      </tr>
      <tr>
        <td>max-device-width</td>
        <td>Medida máxima da largura do dispositivo, por exemplo a tela do computador</td>
      </tr>
      <tr>
        <td>max-height</td>
        <td>Altura máxima da janela</td>
      </tr>
      <tr>
        <td>max-monochrome</td>
        <td>O número de bits máximo por componente de cor para o dispositivo de saída monocromático</td>
      </tr>
      <tr>
        <td>max-resolution</td>
        <td>Resolução máxima do dispositivo, em dpi ou dpcm</td>
      </tr>
      <tr>
        <td>max-width</td>
        <td>Largura máxima da janela</td>
      </tr>
      <tr>
        <td>min-aspect-ratio</td>
        <td>A proporção mínima entre largura e altura da área da tela</td>
      </tr>
      <tr>
        <td>min-color</td>
        <td>O número de bits mínimo por componente de cor para o dispositivo de saída</td>
      </tr>
      <tr>
        <td>min-color-index</td>
        <td>Quantidade mínima de cores que o dispositivo pode exibir</td>
      </tr>
      <tr>
        <td>min-device-aspect-ratio</td>
        <td>A proporção mínima entre a largura ea altura que o dispositivo pode exibir</td>
      </tr>
      <tr>
        <td>min-device-width</td>
        <td>Medida mínima da largura do dispositivo, por exemplo a tela do computador</td>
      </tr>
      <tr>
        <td>min-device-height</td>
        <td>Medida mínima da altura do dispositivo, por exemplo a tela do computador</td>
      </tr>
      <tr>
        <td>min-height</td>
        <td>Altura mínima da janela</td>
      </tr>
      <tr>
        <td>min-monochrome</td>
        <td>O número de bits mínimo por componente de cor para o dispositivo de saída monocromático</td>
      </tr>
      <tr>
        <td>min-resolution</td>
        <td>Resolução mínima do dispositivo, em dpi ou dpcm</td>
      </tr>
      <tr>
        <td>min-width</td>
        <td>Largura mínima da janela</td>
      </tr>
      <tr>
        <td>monochrome</td>
        <td>O número de bits por componente de cor para o dispositivo de saída em dispositivo monocromático</td>
      </tr>
      <tr>
        <td>orientation</td>
        <td>Orientação do dispositivo, retrato ou paisagem</td>
      </tr>
      <tr>
        <td>overflow-block</td>
        <td>Conteúdo transborda para fora do bloco principal</td>
      </tr>
      <tr>
        <td>overflow-inline</td>
        <td>Quando o conteúdo que transborda a janela ao longo da linha</td>
      </tr>
      <tr>
        <td>resolution</td>
        <td>Resolução do dispositivo, em dpi ou dpcm</td>
      </tr>
      <tr>
        <td>scan</td>
        <td>Processo de escanemanto/varredura da tela</td>
      </tr>
      <tr>
        <td>update-frequency</td>
        <td>Quão rápido o dispositivo pode atualizar o conteúdo mostrado, frquência de atualização da tela</td>
      </tr>
      <tr>
        <td>width</td>
        <td>Largura da janela</td>
      </tr>
    </tbody>
  </table>