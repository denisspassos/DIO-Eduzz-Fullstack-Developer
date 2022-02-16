# Introdução a criação de websites com HTML5 e CSS3

## Estrutura básica do HTML5

  

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

## Outras tags muito usadas

### `<p>`
Pepresenta um parágrafo, mas ele não suporta apenas texto, podemos adicionar imagens, código, vídeos e vários outros tipos de conteúdo dentro dele.

### `<a>`
Significa anchor/âncora, ele representa um hyperlink, é ele que interliga vários conteúdos e páginas na web.

O elemento a tem vários atributos, mas vamos focar em dois, o href e o target.

O href representa o hyperlink para onde sua âncora aponta, pode ser uma página do seu ou de outro site, um e-mail e até mesmo um telefone, os dois últimos precisam dos prefixos mailto: e tel:, respectivamente.

O target neste momento vai servir para nos ajudar a abrir nossos links em outra aba do navegador usando o valor _blank.

### `<img>`
A web também é feita de imagens e para representá-las temos o elemento <img>, ele é um daqueles elementos sem tag de fechamento.

O elemento img é bem simples, contendo apenas 2 atributos próprios, o src e o alt.

O src é obrigatório e guarda o caminho para a imagem que você quer mostrar na página.

O alt não é obrigatório mas é altamente recomendado por melhorar a acessibilidade, ele mostra a descrição da imagem caso ela não carregue e leitores de tela usam esse atributo para descrever a imagem para o usuário saber o que ela significa.

### `Listas: <ul>, <ol> e <li>`
O elemento ul cria uma lista não ordenada, onde a ordem dos elementos não é importante, e é representada com pontos, círculos ou quadrados.

O <ol> serve para criar lista ordenadas, nessas a ordem importa, portanto elas são representadas com números, algarismos romanos ou letras.

E o elemento li é um item dentro de uma dessas listas. Um <li> pode conter vários tipos de conteúdos, como parágrafos, imagens e até outras listas.

### Semântica

A semântica nos permite descrever mais precisamente o nosso conteúdo, agora um bloco de texto não é apenas uma div, agora é um article e tem mais significado assim. E temos vários elementos para ressignificar as divs, por exemplo:

    <section>
    <header>
    <article>
    <aside>
    <footer>
    <h1>-<h6>

## CSS3
### ID x Classe
ID: é representado pelo símbolo # (hash) seguido de um nome para esse ID.

    .header {
        padding: 10px;
    }

Classe: a classe é representada de forma parecida do ID, mas é precedida por um ponto em vez do hash.

    #header {
        padding: 10px;
    }


A diferença mais importante entre eles é a forma como devem ser usados: o ID só pode ser usado uma vez em uma página HTML enquanto a classe não tem restrições.

### Box-model
O navegador representa cada elemento HTML como uma caixa retangular, isso é o box-model. E com CSS nós alteramos a aparência dessa caixa (largura, altura, cor de fundo, etc.). Essa caixa é composta por 4 áreas: 
- Conteúdo (content): 
	É o que o seu bloco representa, um texto, uma imagem, um vídeo;
- Borda (border);
- Padding: Espaçamento entre as bordas e o conteúdo. A diferença para as margens é que declarações de imagem de fundo funcionam nele.
- Margem (margin): Espaçamento entre elementos.
