# Introdução a criação de websites com HTML5 e CSS3

## Estrutura básica

  

    <!DOCTYPE html> 
    <html>
	    <head>
		    <meta>
		    <title></title>
	    </head>
	    <body>
	    </body>
    </html>


A primeira linha do documento deve ser o `<!DOCTYPE html>`, apesar de parecer um elemento HTML ela apenas diz ao navegador que ele está lidando com um arquivo do tipo HTML. Os elementos HTML vêm logo abaixo.

### `<html>`

A tag html é a raiz do seu documento, todos os elementos HTML devem estar dentro dela. E nela nós informamos ao navegador qual é o idioma desse nosso documento, através do atributo `lang`, para o português brasileiro usamos `pt-BR`.

### `<head>`

A tag `head` contém elementos que serão lidos pelo navegador, como os metadados - um exemplo é o charset, que é a codificação de caracteres e a mais comum é a UTF-8, o JavaScript com a tag script, o CSS através das tags style e link - veremos a diferença quando falarmos sobre CSS - e o título da página com a tag `title`.

### `<body>`

E dentro da tag `body` colocamos todo o conteúdo visível ao usuário: textos, imagens, vídeos.

## Semântica

A semântica nos permite descrever mais precisamente o nosso conteúdo, agora um bloco de texto não é apenas uma div, agora é um article e tem mais significado assim. E temos vários elementos para ressignificar as divs, por exemplo:
<section>

Representa uma seção genérica de conteúdo quando não houver um elemento mais específico para isso.

    <header>
    <article>
    <aside>
    <footer>
    <h1>-<h6>