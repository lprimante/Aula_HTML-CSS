# Aula de HTML & CSS

Sejam bem vindos as aulas de HTML e CSS, para iniciar, vamos relembrar alguns conceitos básicos?

Link do projeto desenvolvido durante a aula: [Regaste Pet](https://github.com/lprimante/resgate-pet)

## HTML de A a Z

HTML é uma abreviação de Hyper Text Markup Language (linguagem de marcação em hipertexto). Isso mesmo, HTML não é uma linguagem de programação, pois não tem lógica (algoritmos, processos, etc). Ele cria a estrutura de uma página ou aplicação web, determinando a separação de layout e seu conteúdo. Os sites, nos seus primórdios, eram basicamente feitos de html puro! Da uma olhadinha nesse site dos anos 90 que continua até hoje no ar:

![Site do Space Jam de 1996](/images/layout-spacejam-96.jpg)

Fonte: https://www.spacejam.com/1996/

Outros exemplos:
http://www.goetzskyvu.com/GOETZ_THEATRE/GOETZ_SHOW_&_TIMES.html
https://www.lingscars.com/

### Como ganha vida?

Antes de começar a codar, você precisa criar o arquivo html:

index.html

Depois, arquivo criado, você inicia com a estrutura básica:

```HTML
<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Documento</title>
    <link rel="stylesheet" href="styles.css" />
</head>
<body>
</body>
<script src="myscript.js"> </script>
</html>
```

Quem lembra da música:cabeça, ombro, joelho e pé?" É neste flow que o html se estrutura.

### Meta Tags

As <meta> tags definem metadados de um documento HTML, ou seja, informações que vão dentro do elemento <head> e normalmente são usadas para especificar um conjunto de caracteres, descrição da página, palavras-chave, autor do documento e configurações do navegador.

```HTML
<!-- Define palavras-chave para motores de busca-->
<meta name="keywords" content="HTML, CSS, JavaScript">

<!--Define uma descrição da sua página da web-->
<meta name="description" content="Aula de HTML de A a Z">

<!--Define o autor de uma página-->
<meta name="author" content="Maria Silva">

<!--Atualiza o documento a cada 30 segundos-->
<meta http-equiv="refresh" content="30">

<!--Configurando a janela de visualização para que seu site fique bem em todos os dispositivos-->
<meta name="viewport" content="width=device-width, initial-scale=1.0">
```

### Tags (Etiquetas)

Dentro do body, colocamos as tags (etiquetas) que referenciam os elementos no html. Vejam o exemplo a seguir, a tag <p> referencia um elemento de parágrafo.

`<p>Eu sou um parágrafo!</p>`

Algumas tags precisam ser abertas e fechadas, para que estejam certas, como no exemplo acima. Outras são autocontidas, não precisando de tag de fechamento, como é o caso da tag <img> que referencia uma imagem:

`<img src="http://seusite.com/imagem.jpg" />`

### Principais tags

| Tags HMTL                                                  | O que faz?                                                                                                                                                                   |
| ---------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| html, head, body                                           | Utilizada para definir a rela&ccedil;&atilde;o entre o documento e algum recurso externo                                                                                     |
| link                                                       | Localizada na head &eacute; utilizada para definir a rela&ccedil;&atilde;o entre o documento e algum recurso externo                                                         |
| title                                                      | Localizada na head, define o t&iacute;tulo do documento                                                                                                                      |
| main                                                       | Representa o conte&uacute;do de maior relev&acirc;ncia dentro de uma p&aacute;gina                                                                                           |
| header                                                     | Utilizada para representar o cabe&ccedil;alho do documento                                                                                                                   |
| nav                                                        | Utilizada para definir um conjunto de links de navega&ccedil;&atilde;o                                                                                                       |
| section                                                    | Utilizada para criar se&ccedil;&otilde;es dentro de um documento e geralmente cont&eacute;m um t&iacute;tulo                                                                 |
| article                                                    | Utilizada para fazer um artigo dentro de um conte&uacute;do, geralmente se utiliza um t&iacute;tulo e s&atilde;o independentes                                               |
| aside                                                      | Se&ccedil;&otilde;es muitas vezes representadas como barras laterais, relacionado ao conte&uacute;do do seu entorno, que poderia ser considerado separado do conte&uacute;do |
| div                                                        | Utilizada para divis&atilde;o do conte&uacute;do                                                                                                                             |
| footer                                                     | Utilizada para representar o rodap&eacute; do documento                                                                                                                      |
| a                                                          | Utilizada para inserir links                                                                                                                                                 |
| h1 a h6, p, span                                           | Tags para definir t&iacute;tulos e textos                                                                                                                                    |
| img                                                        | Utilizada para inserir imagem                                                                                                                                                |
| video                                                      | Utilizada para inserir um v&iacute;deo                                                                                                                                       |
| audio                                                      | Utilizada para inserir conte&uacute;do de som                                                                                                                                |
| iframe                                                     | Utilizado para incorporar um documento HTML dentro de outro                                                                                                                  |
| form, input, placeholders, checkbox, radiobuttons, buttons | Utilizadas para elementos de um formul&aacute;rio                                                                                                                            |
| thead, tbody, td, th, tr                                   | Utilizadas para elementos de uma tabela                                                                                                                                      |
| ul, li, ol                                                 | Utilizadas para criar listas ordenadas e n&atilde;o ordenadas                                                                                                                |

### Semântica

Semântica é um estudo a respeito do significado/sentido de palavras, frases ou expressões dentro de um contexto. Na programação ela está relacionada ao significado de uma parte do código. Por exemplo: Qual a finalidade/função que esse elemento tem no HTML? O HTML semântico torna as informações de um site bem explicadas para o computador, facilitando o entendimento de leitores de acessibilidade, e ajudando mecanismos de pesquisa a captarem palavras-chave importantes que identificam a página com mais facilidade, indexando com preferência nas buscas.

![HTML Semantico](/images/html-semantico.jpg)

Algumas tag são mais semãnticas do que outras e é importante ficar atenta a elas.

**Leia mais aqui:**

[HTML Semântico: Conheça os elementos semânticos da HTML5](https://www.devmedia.com.br/html-semantico-conheca-os-elementos-semanticos-da-html5/38065)

### Atributos

![Atributo de uma tag](/images/atributo-tag.png)

Um Atributo é uma característica associada ao Elemento HTML. Ele é usado para dar alguma ‘qualidade’ para o Elemento e é posicionado no interior da Etiqueta ou Tag de início. Cada Atributo recebe um valor para configurar essa característica que será dada ao Elemento. Cada Elemento pode ter associado a si alguns pares de Atributos=”valor” dentro de sua Tag inicial.

`<img src="img_girl.jpg" alt="Girl in a jacket" width="500" height="600" />`

### Atributos Globais

Atributos globais são aqueles que todos elementos podem ter:

| Atributo        | Descri&ccedil;&atilde;o                                                                                   |
| --------------- | --------------------------------------------------------------------------------------------------------- |
| accesskey       | Especifica uma tecla de atalho para ativar/focar um elemento                                              |
| contenteditable | Especifica se o conte&uacute;do de um elemento &eacute; edit&aacute;vel ou n&atilde;o                     |
| data\-\*        | Usado para armazenar dados personalizados privados para a p&aacute;gina ou aplicativo                     |
| dir             | Especifica a dire&ccedil;&atilde;o do texto para o conte&uacute;do em um elemento                         |
| draggable       | Especifica se um elemento pode ser arrastado ou n&atilde;o                                                |
| hidden          | Especifica que um elemento ainda n&atilde;o &eacute; ou n&atilde;o &eacute; mais relevante                |
| id              | Especifica um ID exclusivo para um elemento                                                               |
| lang            | Especifica o idioma do conte&uacute;do do elemento                                                        |
| spellcheck      | Especifica se o elemento deve ter sua ortografia e gram&aacute;tica verificadas ou n&atilde;o             |
| style           | Especifica um estilo CSS embutido para um elemento                                                        |
| tabindex        | Especifica a ordem de tabula&ccedil;&atilde;o de um elemento                                              |
| title           | Especifica informa&ccedil;&otilde;es extras sobre um elemento                                             |
| translate       | Especifica se o conte&uacute;do de um elemento deve ser traduzido ou n&atilde;o                           |
| class           | Especifica um ou mais nomes de classe para um elemento \(refere\-se a uma classe em uma folha de estilo\) |

### Site para referência:

https://spria.softcoders.net/
https://demo-egenslab.b-cdn.net/html/hotelina/?c=1
https://demo.web3canvas.com/themeforest/proland/index_kickstarter.html
https://new.axilthemes.com/demo/template/abstrak/onepage-1.html
https://new.axilthemes.com/demo/template/abstrak/onepage-3.html

## Estilizando com CSS

CSS é abreviação de Cascading Style Sheet (folha de estilos em cascata). É a linguagem que define estilos para o HTML, portanto, não se trata de linguagem de programação. CSS tem "cascata" no nome, devido a sua forma de determinar a propriedade de um elemento - levando em consideração hierarquia de seletores e de chamadas de estilo (CSS Interno, CSS inline e CSS externo).

### CSS Interno

Uma folha de estilo interna pode ser usada se uma única página HTML tiver um estilo único.
O estilo interno é definido dentro do elemento
`<style>` dentro da seção `<head>`

```HTML
<!DOCTYPE html>
<html>
    <head>
        <style>
            body {
                background-color: red;
            }

            h1 {
                color: blue;
                margin-left: 40px;
            }
        </style>
    </head>
    <body>

        <h1>This is a heading</h1>
        <p>This is a paragraph.</p>

    </body>
</html>
```

### CSS Inline

Um estilo embutido pode ser usado para aplicar um estilo único para um único elemento.
Para usar estilos embutidos, adicione o atributo style ao elemento relevante. O atributo style pode conter qualquer propriedade CSS.

```HTML
<!DOCTYPE html>
<html>
    <head>
        <title>Documento</title>
    </head>
    <body>

        <h1 style="color:blue;text-align:center;">This is a heading</h1>
        <p style="color:red;">This is a paragraph.</p>

    </body>
</html>
```

### CSS Externo

Para fazer o link de um arquivo .css em um documento .html, devemos inserir a tag no do documento, com o href do caminho do arquivo.

```HTML
<!DOCTYPE html>
<html>
  <head>
    <link rel="stylesheet" href="css/style.css" />
  </head>
  <body></body>
</html>
```

Dentro do arquivo .css, a anatomia é:

![Sintaxe do CSS](/images/css-declaration.png)

**Como colocar comentários em CSS:**

`/* Sou um comentário CSS */`

### Ordem em cascata

Qual estilo será usado quando houver mais de um estilo especificado para um elemento HTML?
Todos os estilos em uma página serão "cascateados" em uma nova folha de estilo "virtual" de acordo com as seguintes regras, onde o número um tem a prioridade mais **alta**:

- CSS inline (atributo dentro de um elemento HTML)
- Folhas de CSS externas e internas (na seção principal)
- CSS padrão do navegador

Portanto, um estilo embutido tem a prioridade mais alta e substituirá os estilos externos e internos e os padrões do navegador.

### Box Model

O box model nos permite adicionar uma borda ao redor dos elementos e definir o espaço entre os elementos.

![Box Model de CSS](/images/CSS-Box-Model.jpg)

- Conteúdo - O conteúdo da caixa, onde o texto e as imagens aparecem
- Preenchimento - Limpa uma área ao redor do conteúdo. O forro é transparente
- Borda - Uma borda que contorna o preenchimento e o conteúdo
- Margem - Limpa uma área fora da fronteira. A margem é transparente

> 320px (largura)
>
> - 20px (padding esquerdo + direito)
> - 10px (border esquerda + direita)
> - 0px (margin esquerda + direita)
>   = 350px

Ao usar a propriedade `box-sizing: border-box` auxilia para que largura e/ou altura internas não sejam somadas a largura e/ou altura do seu elemento final.

> 320px (largura)
>
> - 20px (padding esquerdo + direito)
> - 10px (border esquerda + direita)
> - 0px (margin esquerda + direita)
>   = 320px

### Estilizando elementos

```CSS
p {
    color: red;
    font-family: arial;
    font-size: 14px;
    text-decoration: underline;
    background-color: gray;
    padding-bottom: 15px;
    margin-top: 30px;
}

nav {
    background-color: blue;
    padding: 10px;
    margin: 15px 0;
}

nav a {
    text-decoration: none;
    color: white;
    padding-left: 19px;
    padding-right: 19px;
    border: 1px solid gray;
    border-radius: 5px;
}
```

## CSS Avançado

### Como aplicar cores

As cores podem ser definidas para textos, backgrounds, borders, etc.

**Por nome**
CSS/HTML suporta 140 nomes de cores padrão:
![Cor por nome no CSS](/images/CSS-color-name.png)

**RGB x HEX**

> rgb ( vermelho, verde , azul )

No RGB cada parâmetro (vermelho, verde e azul) define a intensidade da cor entre 0 e 255

> #rrggbb

No HEX a estrutura rr (vermelho), gg (verde) e bb (azul) são valores hexadecimais entre 00 e ff (o mesmo que decimal 0-255)

Exemplo:
![RGB e HEX no CSS](/images/CSS-RGB-HEX.png)

[RGB na prática](/exemplos/rgb.html)

[HEX na prática](/exemplos/hex.html)

**Opacidade**

RGBA

> rgba( vermelho, verde , azul, alfa )
> O parâmetro alfa é um número entre 0,0 (totalmente transparente) e 1,0 (nada transparente)

![Opacidade de cores no CSS](/images/CSS-opacidade.png)

[RGBA na prática](/exemplos/rgba.html)

### Posicionando elementos

#### Position

A propriedade position especifica o tipo de método de posicionamento usado para um elemento.

Existem cinco valores de posição diferentes:

- static (posição padrão dos elementos)
- relative
- fixed
- absolute
- sticky

Os elementos são então posicionados usando as propriedades superior, inferior, esquerda e direita. No entanto, essas propriedades não funcionarão a menos que a propriedade position seja definida primeiro. Eles também funcionam de forma diferente dependendo do valor da posição.

[Exemplos de position na prática](/exemplos/position.html)

**Macete de centralização:**

Funciona apenas para elementos do tipo `display: block`

Defina um tamanho para seu elemento através da propriedade `width` e defina `margin: 0 auto`

[Exemplo de centralização na prática](/exemplos/centralizando.html)

#### Float

A propriedade float é usada para posicionar e formatar o conteúdo, por exemplo, deixar uma imagem flutuar à esquerda do texto em um container.

A propriedade float pode ter um dos seguintes valores:

- left - O elemento flutua à esquerda de seu contêiner
- right - O elemento flutua à direita de seu contêiner
- none - O elemento não flutua (será exibido exatamente onde ocorre no texto). Isso é padrão
- inherit - O elemento herda o valor float de seu pai

[Exemplo de float na prática: em seu uso mais simples, a propriedade float pode ser usada para quebrar o texto em torno das imagens.](/exemplos/float.html)

[Mais exemplos de uso do float](https://www.w3schools.com/css/css_float_examples.asp)

### Seletores

Seletores CSS são usados ​​para "encontrar" (ou selecionar) os elementos HTML que você deseja estilizar.

Podemos dividir os seletores CSS em cinco categorias:

[- Seletores simples (selecione elementos com base no nome, id, classe)]()

```HTML
<!DOCTYPE html>
<html lang="pt-br">
<head>
<style>
section {
    margin: 150px 0;
}
#contato {
    padding: 10px;
}
.blue {
    color: blue;
}
</style>
</head>
<body>

<h1>Exemplo seletores simples</h1>

<section id="contato">
    <p class="blue">Selecione o elemento pelo nome da tag, classe ou id</p>
</section>

</body>
</html>
```

[- Seletores de combinação (selecione elementos com base em um relacionamento específico entre eles)](https://www.w3schools.com/css/css_combinators.asp)

- seletor descendente (espaço)
- seletor filho (>)
- seletor irmão adjacente (+)
- seletor geral de irmãos (~)

```HTML
<!DOCTYPE html>
<html lang="pt-br">
<head>
<style>
section#contato  {
    margin: 150px 0;
}
p.blue {
    color: blue;
}
section + p {
    color: violet;
}
section > p {
    color: violet;
}
</style>
</head>
<body>

<h1>Exemplo seletores de combinação</h1>

<section id="contato">
    <p class="blue">Selecione o elemento pelo nome da tag, classe ou id</p>
    <p>Selecione elementos diferentes a depender da especificidade do seletor</p>
</section>

<p>Eu sou irmão da section</p>

</body>
</html>
```

[- Seletores de pseudo-classe (selecionar elementos com base em um determinado estado)](https://www.w3schools.com/css/css_pseudo_classes.asp)

- Estilizar um elemento quando um usuário passa o mouse sobre ele
- Estilize links visitados e não visitados de maneira diferente
- Estilize um elemento quando ele estiver em foco

```HTML
<!DOCTYPE html>
<html lang="pt-br">
<head>
<style>
section#contato  {
    margin: 150px 0;
}
p.blue {
    color: blue;
}
p.blue:hover {
    color: red;
}
</style>
</head>
<body>

<h1>Exemplo seletores de pseudo-classe</h1>

<section id="contato">
    <p class="blue">Selecione o elemento pelo nome da tag, classe ou id</p>
    <p>Selecione elementos diferentes a depender da especificidade do seletor</p>
</section>

</body>
</html>
```

[- Seletores de pseudo-elementos (selecione e estilize uma parte de um elemento)](https://www.w3schools.com/css/css_pseudo_elements.asp)

```HTML
<!DOCTYPE html>
<html lang="pt-br">
<head>
<style>
p.pseudo::first-letter {
    color: green;
    font-size: xx-large;
}
</style>
</head>
<body>

<h1>Exemplo seletores de pseudo-elemento</h1>

<section id="contato">
    <p class="pseudo">Selecione o elemento pelo nome da tag, classe ou id</p>
    <p>Selecione elementos diferentes a depender da especificidade do seletor</p>
</section>

</body>
</html>
```

[- Seletores de atributo (selecione elementos com base em um atributo ou valor de atributo)](https://www.w3schools.com/css/css_attribute_selectors.asp)

```HTML
<!DOCTYPE html>
<html lang="pt-br">
<head>
<style>
[title~="titulo"] {
    color: green;
    font-size: xx-large;
}
</style>
</head>
<body>

<h1>Exemplo seletores de pseudo-atributo</h1>

<section id="contato">
    <p title="titulo">Selecione o elemento a partir de um atributo</p>
    <input >
</section>

</body>
</html>
```

[Exemplos de seletores](/exemplos/seletores.html)

**Especificidade**

Se houver duas ou mais regras CSS que apontam para o mesmo elemento, o seletor com o maior valor de especificidade "vencerá" e sua declaração de estilo será aplicada a esse elemento HTML.

Pense na especificidade como uma pontuação/classificação que determina qual declaração de estilo é aplicada a um elemento.

- Estilos embutidos - **Exemplo:** `<h1 style="color: pink;">`
- IDs - **Exemplo:** #navbar
- Classes, pseudoclasses, seletores de atributos - **Exemplo:** .test, :hover, [href]
- Elementos e pseudoelementos - **Exemplo:** h1, :before

[Leia mais sobre especificidade](https://www.w3schools.com/css/css_specificity.asp)

#### Classes e id

Classes e ids são atributos que podem ser inseridos em qualquer tag dentro da . Eles são atributos de nomeação, sendo class muito usada para referência em CSS e id para Javascript (apesar de que há outras boas práticas no mercado atualmente). Uma diferença entre os dois é que podem haver várias classes com o mesmo valor, ao passo que ids devem ser únicos.

### Transform

O CSS aceita transformações em 2D e 3D para gerar algumas animações através da propriedade transform

#### Métodos de transformações CSS 2D

Com a propriedade CSS transform você pode usar os seguintes métodos de transformação 2D:

[- translate()](https://www.w3schools.com/css/tryit.asp?filename=trycss3_transform_translate)

[- rotate()](https://www.w3schools.com/css/tryit.asp?filename=trycss3_transform_rotate)

[- scale()](https://www.w3schools.com/css/tryit.asp?filename=trycss3_transform_scale)

[- scaleX()](https://www.w3schools.com/css/tryit.asp?filename=trycss3_transform_scaleX)

[- scaleY()](https://www.w3schools.com/css/tryit.asp?filename=trycss3_transform_scaleY)

[- skew()](https://www.w3schools.com/css/tryit.asp?filename=trycss3_transform_skew)

[- skewX()](https://www.w3schools.com/css/tryit.asp?filename=trycss3_transform_skewx)

[- skewY()](https://www.w3schools.com/css/tryit.asp?filename=trycss3_transform_skewy)

[- matrix()](https://www.w3schools.com/css/tryit.asp?filename=trycss3_transform_matrix1)

#### Métodos de transformações CSS 3D

Com a propriedade CSS transform você pode usar os seguintes métodos de transformação 3D:

[- rotateX()](https://www.w3schools.com/css/tryit.asp?filename=trycss3_transform_rotateX)

[- rotateY()](https://www.w3schools.com/css/tryit.asp?filename=trycss3_transform_rotateY)

[- rotateZ()](https://www.w3schools.com/css/tryit.asp?filename=trycss3_transform_rotateZ)

**Animações feitas com CSS Puro**

https://webdesign.tutsplus.com/pt/articles/15-inspiring-examples-of-css-animation-on-codepen--cms-23937

https://webdesign.tutsplus.com/articles/15-inspiring-examples-of-css-animation-on-codepen--cms-23937

https://blog.hubspot.com/website/css-animation-examples

## Dicas

### Dev Tools

Dá um crtl + f12 e vamos embora! O Devtools é uma ferramenta do navegador que permite a inspeção do código. Com ele você consegue verificar o html e css de qualquer página. Você pode ver as aplicações do código, copiar (sim!, é possivel), mas também ter como inspiração para a sua página. Ali também você pode fazer alterações para verificar como fica a aplicação na sua página e depois aplicar no seu código.

### Documentação

A leitura da documentação é essencial para o aprendizado de HTML e CSS. A documentação te auxilia a tirar dúvidas, corrigir bugs/erros e trazer novos elementos no seu código.

[W3 Schools](https://www.w3schools.com/)

[Mozilla Developer](https://developer.mozilla.org/pt-BR/)

### Identação

⚠️ Identar o código é deixar ele organizado de uma maneira que facilite a sua leitura e de outros desenvolvedores que leiam os eu código. Para indentar, segure a linha de código e aperte tab.

### Reset CSS

Ele ajuda a resetar configurações inicias de elementos que vem como padrão pelo navegadores. Isso nos auxilia na personalização e definição de box model de alguns elementos. Usamos o `*` como seletor, pois ele seleciona todos os elementos de um HTML, exemplo:

```CSS
* {
    margin: 0;
    padding: 0;
    border: none;
}
```

### Metodologia BEM CSS

A sigla BEM significa block, element, modifier, que são os três pilares do método BEM. É uma metodologia de criação de nomes para classes, tornando esse processo mais prático, lógico, e rápido. Ele facilita o entendimento da hierarquia e ação do código, criando um padrão, exemplo:

O nome do bloco e o nome do elemento são separados por dois underlines (\_\_):

```HTML
<form class= "search-form">
    <input class="search-form__input">

    <button class="search-form__button">Pesquisar</button>
</form>
```

O modificador é separado do nome do bloco ou elemento por dois sublinhado (\--):

```HTML
<form class= "search-form">
    <input class="search-form__input--error">

    <button class="search-form__button">Pesquisar</button>
</form>
```

```CSS
.search-form__input--error {
    border: 1px solid red;
}
```

Saiba mais: [Metodologia BEM](https://desenvolvimentoparaweb.com/css/bem/)
