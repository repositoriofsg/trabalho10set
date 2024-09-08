# Consolidação de CSS

**Colaboradores**: Marcio Barcellos, Igor ...., Felipe...

<br><br>
### Capítulo 4: Tipografia

Fontes web: Font-family, fallback fonts.<br>
**Fallback font é a fonte alternativa que será utilizada se a fonte especificada no CSS não puder ser carregada.**
```html
font-family: "Times New Roman", Times, serif;
```

Google Fonts e fontes personalizadas.
No código abaixo será carregado a fonte do Google Montserrat e se ela não estiver disponível será carregada uma fonte da família sans-serif.

```html
<head>
<link rel="stylesheet" href="https://fonts.googleapis.com/css?family=Montserrat">
<style>
body {
  font-family: "Montserrat", sans-serif;
}
</style>
</head>
```

Propriedades tipográficas: Tamanho, altura da linha (line-height), espaçamento entre letras (letter-spacing) e entre palavras (word-spacing).

```html
font-size: 0.875em;
line-height: 30px;
letter-spacing: 1px;
word-spacing: 5px;
```

Estilização de texto: Negrito, itálico, sublinhado, alinhamento, decoração e transformação.

```html
<b>Texto em negrito</b>
<i>Texto em itálico</i>
<u>Texto sublinhado</u>
<p align="center">Texto alinhado no centro</p>
text-decoration: line-through; /* Adiciona uma linha no meio do texto */
text-transform: lowercase; /* Transforma o texto para minúsculo */
```
Prática 4 - [https://repositoriofsg.github.io/trabalho10set/pratica4/](https://repositoriofsg.github.io/trabalho10set/pratica4/)
<br>*Criar um layout de texto para um artigo, explorando fontes e estilos.*



### Capítulo 5: Box Model e Layout

Box Model: Margem (margin), borda (border), padding, conteúdo.
```html
div {
  width: 300px;
  border: 15px solid green;
  padding: 50px;
  margin: 20px;
}
```

Box-sizing: Content-box vs. border-box.
```html
box-sizing: content-box; /* Largura e altura somente são aplicados ao conteúdo do elemento */
box-sizing: border-box; /* Largura e altura são aplicados em todas as partes do elemento; conteúdo, preenchimento e bordas */
```


Display: Block, inline, inline-block.
```html
p.exemplo1 {
  display: block;
  }
p.exemplo2 {
  display: inline;
  }
p.exemplo3 {
  display: inline-block;
  }
```

Manipulação de largura e altura.
```html
div {
  width: 500px;
  height: 200px;
}
```
Prática 5 - [https://repositoriofsg.github.io/trabalho10set/pratica5/](https://repositoriofsg.github.io/trabalho10set/pratica5/)
<br>*Criar um layout simples aplicando conceitos do Box Model e do display.*



### Capítulo 6: Flexbox

Conceito de Flexbox.<br>
**Modo mais eficaz de distribuir e alinhar espaços entre intes em um container, mesmo quando as dimensões dos itens não estão especificadas.**

Container flex:<br>
**display, flex-direction, flex-wrap, flex-flow, justify-content, align-items, align-content, gap, row-gap, column-gap.**

Itens flex:<br>
**Order, flex-grow, flex-shrink, flex-basis, flex, align-self.**


Propriedades do container flex:
```html
display: flex;
flex-direction: row | row-reverse | column | column-reverse;
flex-wrap: nowrap | wrap | wrap-reverse;
flex-flow: column wrap;
justify-content: flex-start | flex-end | center | space-between...;
align-items: stretch | flex-start | flex-end | center | baseline...;
align-content: flex-start | flex-end | center | space-between...;
gap: 10px;
row-gap: 10px;
column-gap: 20px;
```

Propriedades dos itens flex:
```html
order: 5;
flex-grow: 4
flex-shrink: 3;
flex-basis: auto;
align-self: auto | flex-start | flex-end | center | baseline | stretch;
```


Prática 6 - [https://repositoriofsg.github.io/trabalho10set/pratica6/](https://repositoriofsg.github.io/trabalho10set/pratica6/)
<br>*Criar um layout de galeria de imagens utilizando Flexbox.*
