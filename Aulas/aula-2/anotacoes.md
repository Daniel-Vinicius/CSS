# 2- Seletores CSS

[link](http://cfbcursos.com.br/css3-2-seletores-css/)

1- Tag

```css
p {
    color: #d42828;
    font-size: 20px;
}
```

2- Id

```css
#p1 {
    color: #0ba6ff
}
```

3- Classe 

```css
.txt {
    align-items:  center;
}
```

4- Várias tags: 

```css
span, p {
    font-size: 20px
}
```

5- tags filhas: 

```css
span p {
    font-size: 20px
}
```

## Tabela Muitos Seletores

---


  <table>
    <tbody>
      <tr>
        <td><strong>Seletor CSS</strong></td>
        <td><strong>Exemplo</strong></td>
        <td><strong>Descrição</strong></td>
      </tr>
      <tr>
        <td><a href="http://www.w3schools.com/cssref/sel_class.asp">.class</a>e</td>
        <td>.intro</td>
        <td>Seleciona todos os elemtnso que usam a classe intro / class=”intro”</td>
      </tr>
      <tr>
        <td><a href="http://www.w3schools.com/cssref/sel_id.asp">#id</a></td>
        <td>#primeiroNome</td>
        <td>Seleciona o element com o id primeiroNome / id=”primeiroNome”</td>
      </tr>
      <tr>
        <td><a href="http://www.w3schools.com/cssref/sel_all.asp">*</a></td>
        <td>*</td>
        <td>Seleciona todos os elementos</td>
      </tr>
      <tr>
        <td><a href="http://www.w3schools.com/cssref/sel_element.asp">element</a>o</td>
        <td>p</td>
        <td>Seleciona todos os elementos com a tag &lt;p&gt;</td>
      </tr>
      <tr>
        <td><a href="http://www.w3schools.com/cssref/sel_element_comma.asp">elemento,element</a>o</td>
        <td>div, p</td>
        <td>Seleciona todos os elementos &lt;div&gt; e &lt;p&gt;</td>
      </tr>
      <tr>
        <td><a href="http://www.w3schools.com/cssref/sel_element_element.asp">elemento&nbsp;element</a>o</td>
        <td>div p</td>
        <td>Seleciona todos os elementos &lt;p&gt; que estão dentro de elementos &lt;div&gt;</td>
      </tr>
      <tr>
        <td><a href="http://www.w3schools.com/cssref/sel_element_gt.asp">elemento&gt;element</a>o</td>
        <td>div &gt; p</td>
        <td>Seleciona todos os elementos &lt;p&gt; onde o pai seja um elemento &lt;div&gt;</td>
      </tr>
      <tr>
        <td><a href="http://www.w3schools.com/cssref/sel_element_pluss.asp">elemento+element</a>o</td>
        <td>div + p</td>
        <td>Seleciona todos os elementos &lt;p&gt; que estão posicionados imediatamente após o elemento &lt;div&gt;</td>
      </tr>
      <tr>
        <td><a href="http://www.w3schools.com/cssref/sel_gen_sibling.asp">elemento1~elemento2</a></td>
        <td>p ~ ul</td>
        <td>Seleciona todos os elementos &lt;ul&gt; que são precedidos por um elemento &lt;p&gt;</td>
      </tr>
      <tr>
        <td><a href="http://www.w3schools.com/cssref/sel_attribute.asp">[attributo]</a></td>
        <td>[target]</td>
        <td>Seleciona todos os elementos com o atributo target</td>
      </tr>
      <tr>
        <td><a href="http://www.w3schools.com/cssref/sel_attribute_value.asp">[atributo=valor]</a></td>
        <td>[target=_blank]</td>
        <td>Seleciona todos os elementos com o atributo target configurado em _blank / target=”_blank”</td>
      </tr>
      <tr>
        <td><a href="http://www.w3schools.com/cssref/sel_attribute_value_contains.asp">[atributo~=valor]</a></td>
        <td>[title~=curso]</td>
        <td>Seleciona todos os elementos cujo o atributo title contenha a palavra “curso”</td>
      </tr>
      <tr>
        <td><a href="http://www.w3schools.com/cssref/sel_attribute_value_lang.asp">[atributo|=valor]</a></td>
        <td>[lang|=pt]</td>
        <td>Seleciona todos os elementos com um valor de atributo lang começando com “pt”</td>
      </tr>
      <tr>
        <td><a href="http://www.w3schools.com/cssref/sel_attr_begin.asp">[atributo^=valor]</a></td>
        <td>a[href^=”https”]</td>
        <td>Seleciona cada elemento &lt;a&gt; cujo valor do atributo href começa com “https”</td>
      </tr>
      <tr>
        <td><a href="http://www.w3schools.com/cssref/sel_attr_end.asp">[atributo$=valor]</a></td>
        <td>a[href$=”.rar”]</td>
        <td>Seleciona cada elemento &lt;a&gt; cujo valor do atributo href termina com “.rar”</td>
      </tr>
      <tr>
        <td><a href="http://www.w3schools.com/cssref/sel_attr_contain.asp">[atributo*=valor]</a></td>
        <td>a[href*=”cursos”]</td>
        <td>Seleciona a cada &lt;uma&gt; elemento cujo valor do atributo href contenha a substring “cursos”</td>
      </tr>
      <tr>
        <td><a href="http://www.w3schools.com/cssref/sel_active.asp">:active</a></td>
        <td>a:active</td>
        <td>Seleciona o link ativo</td>
      </tr>
      <tr>
        <td><a href="http://www.w3schools.com/cssref/sel_after.asp">::after</a></td>
        <td>p::after</td>
        <td>Insira algo depois do conteúdo de cada elemento</td>
      </tr>
      <tr>
        <td><a href="http://www.w3schools.com/cssref/sel_before.asp">::before</a></td>
        <td>p::before</td>
        <td>Insira algo antes do conteúdo de cada elemento</td>
      </tr>
      <tr>
        <td><a href="http://www.w3schools.com/cssref/sel_checked.asp">:checked</a></td>
        <td>input:checked</td>
        <td>Seleciona todos os elementos &lt;input&gt; que tem a propriedade checked</td>
      </tr>
      <tr>
        <td><a href="http://www.w3schools.com/cssref/sel_disabled.asp">:disabled</a></td>
        <td>input:disabled</td>
        <td>Seleciona todos os elementos &lt;input&gt; que tem a propriedade disabled</td>
      </tr>
      <tr>
        <td><a href="http://www.w3schools.com/cssref/sel_empty.asp">:empty</a></td>
        <td>p:empty</td>
        <td>Seleciona todos os elementos &lt;p&gt; que não tem filhos (incluindo os nós de texto)</td>
      </tr>
      <tr>
        <td><a href="http://www.w3schools.com/cssref/sel_enabled.asp">:enabled</a></td>
        <td>input:enabled</td>
        <td>Seleciona todos os elementos &lt;input&gt; que tem a propriedade enabled</td>
      </tr>
      <tr>
        <td><a href="http://www.w3schools.com/cssref/sel_firstchild.asp">:first-child</a></td>
        <td>p:first-child</td>
        <td>Seleciona todos os elementos &lt;p&gt; que são first-child de seu elemento pai</td>
      </tr>
      <tr>
        <td><a href="http://www.w3schools.com/cssref/sel_firstletter.asp">::first-letter</a></td>
        <td>p::first-letter</td>
        <td>Seleciona a primeira letra de cada elemento &lt;p&gt;</td>
      </tr>
      <tr>
        <td><a href="http://www.w3schools.com/cssref/sel_firstline.asp">::first-line</a></td>
        <td>p::first-line</td>
        <td>Selects the first line of every &lt;p&gt; element</td>
      </tr>
      <tr>
        <td><a href="http://www.w3schools.com/cssref/sel_first-of-type.asp">:first-of-type</a></td>
        <td>p:first-of-type</td>
        <td>Seleciona a primeira linha de cada elemento &lt;p&gt;</td>
      </tr>
      <tr>
        <td><a href="http://www.w3schools.com/cssref/sel_focus.asp">:focus</a></td>
        <td>input:focus</td>
        <td>Seleciona o elemento de entrada que tem o foco</td>
      </tr>
      <tr>
        <td><a href="http://www.w3schools.com/cssref/sel_hover.asp">:hover</a></td>
        <td>a:hover</td>
        <td>Selecione os links que o tem a propriedade hover configurada</td>
      </tr>
      <tr>
        <td><a href="http://www.w3schools.com/cssref/sel_in-range.asp">:in-range</a></td>
        <td>input:in-range</td>
        <td>Seleciona elementos de entrada com um valor dentro de um intervalo especificado</td>
      </tr>
      <tr>
        <td><a href="http://www.w3schools.com/cssref/sel_invalid.asp">:invalid</a></td>
        <td>input:invalid</td>
        <td>Seleciona todos os elementos &lt;input&gt; que tem a propriedade invalid</td>
      </tr>
      <tr>
        <td><a href="http://www.w3schools.com/cssref/sel_lang.asp">:lang(language)</a></td>
        <td>p:lang(en)</td>
        <td>Seleciona todos os elementos &lt;p&gt; com um atributo lang igual a “en” (inglês)</td>
      </tr>
      <tr>
        <td><a href="http://www.w3schools.com/cssref/sel_last-child.asp">:last-child</a></td>
        <td>p:last-child</td>
        <td>Seleciona todos os elementos &lt;p&gt; que é o último filho do seu elemento pai</td>
      </tr>
      <tr>
        <td><a href="http://www.w3schools.com/cssref/sel_last-of-type.asp">:last-of-type</a></td>
        <td>p:last-of-type</td>
        <td>Seleciona todos os elementos &lt;p&gt; que é o último elemento &lt;p&gt; de seu elemento pai</td>
      </tr>
      <tr>
        <td><a href="http://www.w3schools.com/cssref/sel_link.asp">:link</a></td>
        <td>a:link</td>
        <td>Seleciona todos os links não clicados</td>
      </tr>
      <tr>
        <td><a href="http://www.w3schools.com/cssref/sel_not.asp">:not(selector)</a></td>
        <td>:not(p)</td>
        <td>Seleciona todos os elementos que não são um elemento &lt;p&gt;</td>
      </tr>
      <tr>
        <td><a href="http://www.w3schools.com/cssref/sel_nth-child.asp">:nth-child(n)</a></td>
        <td>p:nth-child(2)</td>
        <td>Seleciona o elemento &lt;p&gt; que é o segundo filho de seu elemento pai</td>
      </tr>
      <tr>
        <td><a href="http://www.w3schools.com/cssref/sel_nth-last-child.asp">:nth-last-child(n)</a></td>
        <td>p:nth-last-child(2)</td>
        <td>Seleciona o elemento &lt;p&gt; que é o segundo filho de seu elemento pai, a contar do último elemento filho
        </td>
      </tr>
      <tr>
        <td><a href="http://www.w3schools.com/cssref/sel_nth-last-of-type.asp">:nth-last-of-type(n)</a></td>
        <td>p:nth-last-of-type(2)</td>
        <td>Seleciona o elemento &lt;p&gt; que é o segundo elemento &lt;p&gt; de seu elemento pai, a contar do último
          elemento filho</td>
      </tr>
      <tr>
        <td><a href="http://www.w3schools.com/cssref/sel_nth-of-type.asp">:nth-of-type(n)</a></td>
        <td>p:nth-of-type(2)</td>
        <td>Seleciona o elemento &lt;p&gt; que é o segundo elemento &lt;p&gt; de seu elemento pai</td>
      </tr>
      <tr>
        <td><a href="http://www.w3schools.com/cssref/sel_only-of-type.asp">:only-of-type</a></td>
        <td>p:only-of-type</td>
        <td>Seleciona todos os elementos &lt;p&gt; de seu elemento pai</td>
      </tr>
      <tr>
        <td><a href="http://www.w3schools.com/cssref/sel_only-child.asp">:only-child</a></td>
        <td>p:only-child</td>
        <td>Seleciona todos os elementos &lt;p&gt; que só tem um elemento como filho</td>
      </tr>
      <tr>
        <td><a href="http://www.w3schools.com/cssref/sel_optional.asp">:optional</a></td>
        <td>input:optional</td>
        <td>Seleciona elementos input com nenhum atributo “required”</td>
      </tr>
      <tr>
        <td><a href="http://www.w3schools.com/cssref/sel_out-of-range.asp">:out-of-range</a></td>
        <td>input:out-of-range</td>
        <td>Seleciona elementos input com um valor fora de um intervalo especificado</td>
      </tr>
      <tr>
        <td><a href="http://www.w3schools.com/cssref/sel_read-only.asp">:read-only</a></td>
        <td>input:read-only</td>
        <td>Seleciona elementos input com o atributo “readonly” especificado</td>
      </tr>
      <tr>
        <td><a href="http://www.w3schools.com/cssref/sel_read-write.asp">:read-write</a></td>
        <td>input:read-write</td>
        <td>Seleciona elementos input com o atributo “readonly” NÃO especificado</td>
      </tr>
      <tr>
        <td><a href="http://www.w3schools.com/cssref/sel_required.asp">:required</a></td>
        <td>input:required</td>
        <td>Seleciona elementos input com o atributo “required” especificado</td>
      </tr>
      <tr>
        <td><a href="http://www.w3schools.com/cssref/sel_root.asp">:root</a></td>
        <td>:root</td>
        <td>Seleciona o elemento raiz do documento</td>
      </tr>
      <tr>
        <td><a href="http://www.w3schools.com/cssref/sel_selection.asp">::selection</a></td>
        <td>::selection</td>
        <td>Selecciona a parte de um elemento que é selecionado pelo usuário</td>
      </tr>
      <tr>
        <td><a href="http://www.w3schools.com/cssref/sel_target.asp">:target</a></td>
        <td>#noticias:target</td>
        <td>Seleciona o elemento #noticias atual (clicou em um URL que contém esse nome de âncora)</td>
      </tr>
      <tr>
        <td><a href="http://www.w3schools.com/cssref/sel_valid.asp">:valid</a></td>
        <td>input:valid</td>
        <td>Seleciona todos os elementos input com um valor válido</td>
      </tr>
      <tr>
        <td><a href="http://www.w3schools.com/cssref/sel_visited.asp">:visited</a></td>
        <td>a:visited</td>
        <td>Seleciona todos os links visitados</td>
      </tr>
    </tbody>
  </table>