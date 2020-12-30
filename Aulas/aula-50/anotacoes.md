# 50 - @media - Layout Responsivo - Parte 3

[link](http://cfbcursos.com.br/css3-484950-media-layouts-responsivos/)

**@media**

@media é uma propriedade css que retorna true ou false com base em verificações e caso seja verdadeira aplica alguma formatação a algum elemento.

Nesta terceira aula treinamos bastante da propriedade @media.


**Html:**

```html
<html lang="pt-br">

<head>
  <title>CFB Veículos</title>
  <meta charset="utf-8" />
  <link rel="stylesheet" href="style.css" />
</head>

<body>

  <header>
    <img src="imgs/logo.svg">
    <nav>
      <a class="btmenu" href="#" target="_self">home</a>
      <a class="btmenu" href="#" target="_self">carros</a>
      <a class="btmenu" href="#" target="_self">contato</a>
      <a class="btmenu" href="#" target="_self">localização</a>
    </nav>
  </header>

  <section class="banner">
    <img src="imgs/banner.jpg" />
  </section>

  <section class="buscador">
    <p>Encontre um veículo</p>
    <form name="fbuscador" id="fbuscador" action="" method="post">
      <div>
        <label>Selecione a marca</label>
        <select name="marca" id="id_marcas">
          <option value="">Fiat</option>
          <option value="">Gol</option>
        </select>
      </div>
      <div>
        <label>Selecione o modelo</label>
        <select name="modelo" id="id_modelos">
          <option value="">Toro 2018</option>
          <option value="">Gol Bola 2011</option>
        </select>
      </div>
      <div>
        <input value="BUSCAR" class="btmenu">
      </div>
    </form>
  </section>

  <section id="destaques">
    <a class="destaque" href="#" target="_self" title="Mostrar veículos"><img src="imgs/carros.png"></a>
    <a class="destaque" href="#" target="_self" title="Página de contatos"><img src="imgs/contato.png"></a>
    <a class="destaque" href="#" target="_self" title="Nossa localização"><img src="imgs/local.png"></a>
  </section>

  <footer>
    <p>Site desenvolvido pelo Canal Fessor Bruno para curso online</p>
  </footer>

</body>

</html>
```

**Css:**

```css
/*Reset básico*/

* {
  margin: 0px;
  padding: 0px;
  outline: 0px;
  font-size: 100%;
  background: transparent;
  box-sizing: border-box;
  color: #ffffff;
}

option {
  background-color: #222;
}

body {
  font-family: sans-serif Arial;
  background-color: #222;
  overflow: scroll;
  overflow-x: hidden;
}

/*HEADER*/

header, section, footer {
  display: flex;
  justify-content: space-between;
  padding-left: 20px;
  padding-right: 20px;
  font-family: sans-serif Arial;
}

header {
  background: #000;
  align-items: center;
}

header img {
  width: 301px;
  height: 111px;
  margin: 10px 0px;
}

header nav {
  display: flex;
}

.btmenu {
  text-decoration: none;
  display: flex;
  width: 120px;
  height: 30px;
  margin: 2px;
  padding: 1px 5px 1px 5px;
  background-color: #222;
  border-radius: 10px;
  color: #bbb;
  font-family: Arial;
  font-size: 10px;
  cursor: pointer;
  border: 0px;
  text-transform: uppercase;
  outline: none;
  justify-content: center;
  align-items: center;
}

.btmenu:hover {
  background-color: #c22;
  color: #FFF;
}

.banner {
  padding: 0px;
  overflow: hidden;
  justify-content: center;
  align-items: center;
}

.buscador {
  margin: 10px 0px;
  flex-direction: column;
  align-items: center;
}

.buscador p {
  width: 800px;
  display: flex;
  margin-top: 10px;
  justify-content: flex-start;
  align-items: center;
}

.buscador form {
  width: 800px;
  border: 1px solid #888888;
  padding: 10px;
  display: flex;
  margin: 10px 0px;
  justify-content: space-between;
  align-items: center;
}

.destaque {
  margin: auto;
  padding: 50px;
  background: #000;
  border-radius: 100%;
}

.destaque:hover {
  background: #c22;
}

footer {
  margin-top: 10px;
  background: #353535;
  padding-top: 20px;
  padding-bottom: 20px;
  color: #fff;
}

@media screen and (max-device-width: 500px) and (orientation: portrait) {
  header, section, footer {
    padding-left: 3%;
    padding-right: 3%;
  }
  header {
    flex-direction: column;
  }
  header img {
    width: 100%;
    height: 100%;
  }
  header nav {
    flex-direction: column;
    width: 100%;
  }
  .btmenu {
    width: 100%;
    height: 80px;
    font-size: 30px;
  }
  .banner, footer, #destaques {
    display: none;
  }
  .buscador p, .buscador form {
    width: 100%;
  }
  .buscador p, select, label {
    justify-content: center;
    margin: 10px;
    font-weight: bold;
    font-size: 30px;
    font-family: Arial, sans-serif;
  }
  .buscador select, label {
    font-size: 20px;
    font-family: Arial, sans-serif;
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