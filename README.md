## tag's HTML

As tags servem para marcar um conteúdo HTML, inserior conteúdo, imagens, vídeos e dar semantica, ou seja, permitir que AI de google e entre outras, identifiquem melhor seu contúdo na WEB. Além disso, servem para integração com o CSS e o JavaScript

> Exemplo de uma tag:

```
Abrimos <a> conteúdo: é o que vai aparecer para o usuário </a> e fechamos a tag
```

## Atributos de uma tag HTML

Os atributos dão informação extra ou funções para a tag

> Exemplo de um atributo na tag <a> seria o href=""

```
<a href="google.com">google</a>
```

## tag's mais comuns do HTML

```
p: Marca um parágrafo
<p>Conteúdo do parágrado</p>

h1,h2,h3,h4,h4,h6: Marca deiferentes tipos de títulos
<h1>Títulos</h1>

a: Marca um link
<a href='google.com'>Google</a>

body: Contém toda execusão do site
<body>
Vai todo o conteúdo que o usuário irá ver no site, ou seja, as tags devem ser construídas demtro do body
</body>

head: Conteém algumas configurações do site
<head>
Vai todo conteúdo configurável do site, o qual o usuário não irá ver. como exemplo o <title>para alterar o nome que aparesse na aba do site</title>
</head>
```

## VScode

#### Puglins para o VScode

Live Server

> Pode ser aplicado nos Puglins do VScode para não precisar ficar dando refresh no site. o mesmo emula um site. Após salvar alterações no código o mesmo automaticamnete muda os site.

#### Atalhos do VScode

CTRL + SHIFT + P

> Abre uma caixa de pesquisa para fazer consultas e encontrar algumas funcionalidades, como por exemplo: abrir arquivo de configuração do VScode, executar algum plugin, encontrar algum arquivo

CTRL + C na linha sem estar nada selecionado

> Copia todo a linha para o CTRL + V

CTRL + SHIF + Z

> Faz a funcionalidade inversa do CTRL + Z

ALT na linha mais setas direcionais cima ou baixo

> Movimenta a lina para o direcional que você clica

CTRL + D

> Seleciona as proximas palavras parecidas com uma palávra que já está selecionada, pocibilitando mudar tudo de uma vez

CTRL + / , `<!-- Comentário-->` ou //comentário

> Fazer Comentário

> CTRL + B
> Fecha explorador de arquivos

## Marcação para caminhos de arquivos

Arquivo index.html no diretório raiz /.

`/index.html`

Arquivo bicicletas.html no diretório /produtos localizado na raiz.

`/produtos/bicicletas.html`

Arquivo index.html no diretório atual ./.

`index.html ou ./index.html`

Arquivo index.html um diretório anterior ao atual ../.

`../index.html`

Arquivo index.html dois diretórios anteriores ao atual.

`../../index.html`

> Exemplos detalhados

```
<a href="/index.html">Home</a>

<a href="./bicicletas.html">Bicicletas</a>
<!--dessa forma, ele irá falar com o dretório atual que está carros e vai tentar encontrar bicletas, caso não encontre ele, irá dar erro -->

<a href="bicicletas.html">Bicicletas</a>
<!--dessa forma, ele irá falar com o dretório atual que está carros e vai tentar encontrar bicletas, caso não encontre ele, irá dar erro igual a anterios-->

<a href="/index.html">Bicicletas</a>
<!--dessa forma, ele irá falar com o dretório raiz onde está index e vai tentar encontrar index, caso não encontre ele, irá dar erro -->

<a href="../index.html">Bicicletas</a>
<!--dessa forma, ele irá falar com o dretório raiz onde está index e vai tentar encontrar index, caso não encontre ele, irá dar erro igual a anterior-->
```

## Box Model

Uma interface web é composta de diversas caixas que organizam o conteúdo. E com alguns atributos CSS definimos o tamanho dessas caixas

> Exemplo:

```
Content (conteúdo)
Define a largura inicial da caixa (salvo elementos de bloco).

Padding (preenchimento)
Separa o conteúdo das bordas da caixa. É a margem interna.

Border (borda)
Define bordas para a caixa.

Margin (margem)
Define a distância entre uma caixa e outra.

Width (largura)
A largura total da caixa, por padrão é o somatório do conteúdo + padding (left/right) + border (left/right).

Height (altura)
A largura total da caixa, por padrão é o somatório do conteúdo + padding (top/bottom) + border (top/bottom).
```

![Exemplo de Box Model](/imagens/box-model.png "Exemplo de Box Model.")

## Display

Define como a caixa irá se comportar

#### inline

> Respeita o fluxo da escrita sem iniciar uma nova linha, não é possível definir valores de width, height, margin (top/bottom) e etc. É o estilo padrão. Dessa forma os elementos ficam na linha um do lado do outro.

#### block

> Inicia uma nova linha e não permite que outros elementos sejam posicionados em sua linha. Aceita todas as propriedades do box model. Estilo inicial de elementos como h1, p, div e outros.

#### inline-block

> O elemento continua inline, mas passa a receber as propriedades do box model. Ou seja, pode ser atribuídos valores de tamanho das caixas

#### Outros elementos de display

> Para posicionamentos complexos, como o da imagem abaixo, utilizamos as propriedades display grid (CSS Grid Layout) e flex (Flexbox).

# Img

#### Max-width

> Com o atributo CSS max-width, voce define qual o tamanho máximo da image, de acordo com elemento pai que ela está. Então se ela está dentro de uma Div, ela vai ficar do tamanho da div, caso esteja max-width: 100%
