# 48 - @media - Layout Responsivo - Parte 1

[link](http://cfbcursos.com.br/css3-484950-media-layouts-responsivos/)

**@media**

@media é uma propriedade css que retorna true ou false com base em verificações e caso seja verdadeira aplica alguma formatação a algum elemento.

@media pode receber 4 propriedades primárias em relação aos tipos de dispositivos:

* 1- Todos tipos de dispositivos `@media all {}`
* 2- Telas `@media screen {}`
* 3- Para Leitores de Arquivos Digitais `@media speech {}`
* 4- Para Impressão `@media print {}`

---

Também é possível alterar formatações com base na orientação do dispositivo:

* 1- Paisagem `@media (orientation: landscape) {}`
* 2- Retrato `@media (orientation: portrait) {}`

---

**Html:**

```html
<body>
  <img src="logo.png">
</body>
```

**Css:**

```css
img {
  width: 80%;
}

body {
  background-color: #222;
}

@media screen and (min-width: 0px) and (max-width: 800px) and (orientation: portrait) {
  body {
    background-color: #c22f2f;
  }
  img {
    width: 100%;
  }
}

@media screen and (min-width: 0px) and (max-width: 800px) and (orientation: landscape) {
  body {
    background-color: #3879db;
  }
  img {
    width: 100%;
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