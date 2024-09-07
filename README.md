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

em construção