# Seção 4 - Introdução ao CSS

## Aula 1 - Maneiras de adicionar CSS

Temos algumas maneiras de adicionar css ao html:

Inline: quando os estilos são adicionados por um atributo;

Internal: quando o css é adicionado na tag head;

External: quando o css é adicionado através de um arquivo externo e depois importado no html.

Vamos sempre optar pelo external, quando houver opção, isso vai organizar melhor nosso projeto.

## Aula 2 - A anatomia do CSS

Com css aplicamos css (estilo) a um elemento

Primeiramente devemos selecionar o elemento, isso pode ser feito atrvés da tag

Depois precisamos colocar as propriedades e os valores

Se quisermos mudar a cor de algo, por exemplo, utilizamos: color: red;

Nome da propriedade, dois pontos, valor, ponto e vírgula.

## Aula 3 - Inline CSS

O CSS inline pode ser adicionado sem selecionar o elemento, pois é um atributo diretamente inserido no mesmo

O elemento já está selecionado!

O atributo 'style' nos permite escrever regras de css

Exemplo: style="color: red;"

### Aula 4 - Múltiplas regras

Nós podemos adicionar várias regras de css

Elas podem ser separadas por ponto e vírgula

Então é possível fazer uma união de estilos, dar uma aparência melhor ao elemento

## Aula 5 - Internal

O css interno é uma técnica melhor que o inline, vamos colocar todos os estilos na tag head

As regras precisam também estar entre a tag style

E através dessa maneira, é necessário selecionar o elemento alvo. Ex.:

p { <br/>
    color: red; <br/>
}

## Aula 6 - External

Para adicionar css com esta técnica, precisamos criar um arquivo .css

Geralmente eles ficam numa pasta chamada css

E nós o importamos através da tag 'link'

As regras que estão no arquivo são aplicadas em todo o html

## Aula 7 - Ordem do CSS

O CSS é carregado a partir de uma ordem

Se temos estilos misturados (inline, internal e external), qual será aplicado?

Todos eles, mas com a seguinte ordem: inline > internal = external > padrão do navegador

Esta regra funciona quando temos estilos diferentes em um mesmo elemento

Interno e externo tem a mesma prioridade, a última regra ganha a "corrida"


## Aula 8 - Múltiplos arquivos CSS

É possível ter mais de uma folha de estilo no nosso projeto

Precisamos apenas importar todas elas na tag head

Os arquivos importados por último tem maior prioridade

Esta é uma boa prática, pois possibilita a divisão do css por páginas, por exemplo (ou seções diferentes do html, etc)

## Desafio 1 de CSS

Primeiro desafio de css -> <a href="./desafio1/">Pasta do Desafio</a>

## Aula 9 - Comentários no CSS

Comentários no CSS são como os de HTML, usamos para descrever algo no código

Caso o código seja inspecionado, os comentários também serão exibidos

A sintaxe é: /* Algum comentário */

## Aula 10 - Classes e IDs

Classes e ids são atributos de tags do HTML, mas estão altamente relacionados ao CSS

Podemos especificar elementos específicos com eles

Ids são utilizados para elementos únicos

E classes servem para um ou mais elementos, geralmente usadas em conjuntos de elementos

## Aula 11 - Classes

As classes são inseridas através de um atributo de HTML

O valor do atributo é o nome da classe, e também uma escolha nossa

Por exemplo: temos um botão que aparece x vezes no nosso projeto, podemos colocar uma classe 'btn' nele

Ou seja, os padrões de estilo desses botões podem ser transmitidos através desta classe para os demais

O seletor fica: .nomeClasse (com um ponto na frente)

## Aula 12 - IDs

Os ids também são atributos do HTML

Podemos escrever qualquer coisa como valor, será o nome do id

Ids são únicos, ou seja, não repetiremos o mesmo nome na mesma página

O HTML não nos proíbe disso, mas é uma má prática e deve ser evitada

O seletor fica: #nomeID

## Aula 13 - A ordem dos seletores

Nós aprendemos sobre o seletor de id e de classe

E se a tag estiver com id e uma classe, o que acontece?

Como nas maneiras de adicionar CSS, temos também uma ordem

Então o id vai vencer todos os outros, utilize isso a seu favor

Regras que não entram em conflito serão aplicadas normalmente

## Aula 14 - As cores no CSS

Em CSS as cores são divididas em grupos, temos:

- Nomes de cor: como red ou blue, não são muito utilizadas

- RGB: configuramos as tonalidades de red, green e blue

- Hexadecimal: uma união de letras e números, que podem criar uma cor, a maneira mais utilizada

- HSL: hue, saturation e lightness, mudando estes valores temos uma cor

Nas próximas aulas abordaremos todos, detalhadamente

## Aula 15 - Nomes das cores

Nós utilizamos muito essa maneira até agora, mas em projetos reais não é muito empregada

Pois ela nos limita a apenas as cores com nomes existentes (e registrados no editor)

No mundo real precisamos de mais possibilidades, para não limitar os designers

O nome da cor consiste na utilização do nome real da cor como propriedade

## Aula 16 - Hexadecimal

HEX ou Hexadecimal é a abordagem mais utilizada

Basicamente temos que inserir 6 dígitos, precedidos de uma #

Os dois primeiros representam o tom de vermelho, depois de verde, e por fim, de azul

Os valores vão de 0 a 9 e A a F

0 é o mais escuro e F o mais claro

O valor de #000 é a cor preta e #FFF é o branco (3 dígitos pq como cada dupla é igual, não precisa digitar tudo e só os três já indicam o RGB em HEX)

### Aula 17 - Aprofundando sobre o HEX

Se um valor for repetido 6 vezes, podemos escrever a cor de uma forma mais simples

No caso de #FFFFFF podemos reescrever com #FFF

A mesma coisa vale para #112233, essa cor pode ser escrita como #123

## Aula 18 - RGB

RGB significa Red, Green e Blue (ou seja, vermelho, verde e azul)

Nós precisamos inserir a intensidade de cada um, com valores de 0 a 255 [no fim das contas, com números em hex também é de 0 a 255 (00 a FF)]

0 é o mais escuro e 255 o mais claro

Aplicamos RGB com a seguinte sintaxe: rgb(0-255, 0-255, 0-255)

O primeiro valor representa o vermelho, o segundo o verde e o terceiro azul

Para criar a cor verde, inserimos: rgb(0, 255, 0)

### Aula 19 - RGBa

Podemos criar cores também com o RGBA, o A vem de alpha

A alteração dele muda a opacidade da cor

Os valores possíveis são de 0 a 1 (assumindo os valores reais no meio termo)

Sendo 0 transparente e 1 totalmente visível

A sintaxe e quase a mesma: rgba(0-255, 0-255, 0-255, 0-1)

## Aula 20 - HSL

HSL é um acrônimo para hue, saturation e lightness (tonalidade, saturação e luminosidade)

Esta abordagem também não é muito utilizada, o ranking de uso é esse: HEX > RGB > HSL > nomes de cor

Podemos definir uma cor com hsl(0-360, 0-100%, 0-100%) [sim, até 360, hsl é baseado em círculo cromático e muito utilizado por designers para criar as variações de tonalidade a partir de uma cor base, e usar opostos no círculo para criar contraste agradável]

## Aula 21 - Background Color

Quase todo elemento tem um background, e podemos mudar a cor dele

Todas as regras que vimos sobre cores podem ser aplicadas em cores de background

A regra é: background-color: "cor"

As regras de cor de fundo e cor de fonte podem ser utilizadas juntas

## Aula 22 - Background Opacity

Podemos alterar a opacidade de uma cor de fundo com CSS

A regra é a 'opacity'

Os valores vão de 0 a 1

Sendo 1 totalmente visível e 0 remove a cor

Com esta regra mudamos também a opacidade do conteúdo dentro do elemento, veremos uma solução depois

## Aula 23 - RGBa para Background

Se você não quer aplicar a opacidade para os elementos internos, então deve aplicar RGBa em vez de opacity

Alterando o valor de alpha temos a opacidade aplicada apenas na cor de fundo

Então preservamos o conteúdo e alteramos o background

## Aula 24 - Background Image

Podemos inserir imagens no fundo dos elementos

A regra é: background-image: url("caminho/url")

Geralmente a imagem fica em outra pasta, então temos que voltar um diretório

Isso pode ser feito com o símbolo '..' (ex.: url("../pasta_imagens/imagem.png"))

## Aula 25 - Centralizando a imagem de bg

Às vezes a imagem é muito maior que o elemento que estamos inserindo

Então precisamos melhorar a visualização, centralizando a imagem

Isso pode ser feito com duas regras:

- background-position: center; e

- background-size: cover;

## Aula 26 - Box-Model

Box model é uma entidade que é criada em todo elemento do HTML

Ela consiste em quatro partes: altura e largura, padding, border e margin

Todas elas podem ser alteradas por CSS

Alguns elementos do HTML já vem com valor padrão nestas regras

Este conceito é muito importante, veremos em detalhes nas próximas aulas

### Aula 27 - Altura e Largura

A altura e a largura são o núcleo do box-model

Estas propriedades consistem no conteúdo do elemento

Podemos alterar as duas e mudar o tamanho do elemento na tela

Alguns dos elementos do HTML, os block elements, já vem com 100% de largura

Preenchendo a tela toda na horizontal

### Aula 28 - Padding

Padding é o espaço entre o conteúdo e a borda do elemento, também conhecido como espaçamento interno

Este recurso é utilizado para criar uma distância entre o conteúdo (texto) e a extremidade do elemento

#### Aula 29 - Padding Individual

Podemos adicionar o padding aos lados individuais de um elemento

A regra é: padding-*

Onde * pode ser: top, left, right ou bottom

Assim teremos valores customizados em cada um dos lados do elemento

#### Aula 30 - Shorthand Padding

As propriedades de shorthand nos permitem adicionar padding a todas as direções com apenas uma regra

Apenas precisamos utilizar a regra padding e configurar top, right, bottom e left, nessa ordem

Exemplo: padding: 10px 5px 12px 20px

Esta regra de shorthand pode ser aplicada para outras propriedades, como margin

#### Aula 31- Padding e Width

A padding é adicionada a largura do elemento, e isso pode ser um problema

Por exemplo: se precisamos seguir um layout perfeitamente

Um elemento com 200px de width e 25px de padding tem um tamanho total de 250px na horizontal (25 de um lado + 25 de outro)

Podemos diminuir a largura do elemento, mas isso dificulta o cálculo também

Isso pode ser resolvido com a regra 'box-sizing' com o valor 'border-box', isso faz o elemento respeitar a width

### Aula 32 - Borda

A borda é o elemento central, fica entre padding e margin

Padding é o espaçamento interno, e margin externo

Geralmente esta regra é utilizada com propósito decorativo

A regra de border é definida em algumas partes: tamanho, aspecto e cor da borda

#### Aula 33 - Lados individuais da borda

Podemos adicionar borda aos lados específicos de um elemento também

Podemos utilizar: border-*

Onde * pode ser top, right, bottom e left

Isso é utilizado frequentemente, especialmente com a border-bottom e left

#### Aula 34 - Bordas Arredondadas

Com a propriedade 'border-radius' podemos arredondar os cantos de um elemento

Podemos aplicá-la assim: border-radius: 5px

Isso faz com que os cantos sejam arredondados em 5px (também podemos arredondar cima-baixo/esquerda-direita, ou os quatro cantos individualmente na mesma chamada)

Importante: podemos arredondar elementos que não tem a regra de borda aplicada

### Aula 35 - Margem

a propriedade de 'margin' é responsável pelo espaçamento externo do elemento

Podemos aplicar o recurso como aplicamos padding

Ou seja: lados individuais e também o shorthand

### Aula 36 - Elementos do box-model juntos

Em alguns elementos vamos utilizar todos os recursos do box-model

Ou seja, vamos definir:

- o tamanho (width e height)

- um espaçamento interno (padding)

- decorar o elemento com bordas (border)

- afastar o elemento de outros elementos (margin)

## Aula 37 - Alinhamento de texto

Nossos textos podem ser alinhados em várias direções

Por padrão ele é alinhado a esquerda

Porém com a regra 'text-align' configuramos center (centro) ou right (direita), para alterar o valor default

Usamos muito o valor de center

## Aula 38 - Text Decoration

Com a decoration podemos adicionar efeitos ao texto

É possível colocar um underline ou até mesmo uma linha que corta o texto

Esta regra é utilizada em casos específicos

A tag 'a' tem um underline por padrão, podemos remover isso com a regra de 'text-decoration' e o valor de 'none'

## Aula 39 - Transformação de Texto

Com a regra 'text-transform' podemos alterar como o texto é exibido

É possível alterar para 'uppercase' ou 'lowercase' (maiúsculas ou minúsculas)

Não há muitos valores para esta regra

Cuidado: O CSS deve ser aplicado quando queremos o texto em uppercase, NUNCA escreva o texto em caps lock no HTML

## Aula 40 - Espaçamento entre letras

Com a regra 'letter-spacing' podemos alterar o espaçamento entre letras de um texto

Isso é interessante em situações que o layout pede essa mudança

A regra é aplicada da seguinte forma: 'letter-spacing: 5px;'

## Aula 41 - Fontes

Com CSS podemos alterar o tipo da fonte, com 'font-family'

As regras disponíveis são: 'Serif', 'Sans-serif', 'Monospace', 'Cursive' e 'Fantasy'

Todos os navegadores tem várias fontes que podemos utilizar

E ainda podemos adicionar fontes externas, como por exemplo do Google Fonts

## Aula 42 - Estilos de fontes

Nós podemos utilizar a propriedade font-style para mudar o aspecto das letras

Os valores são: 'normal', 'italic' e 'oblique'

Normal é o valor padrão, e os outros são as variantes

Oblique é como o tipo itálico, com pequenas diferenças

## Aula 43 - Font weight

A propriedade 'font-weight' pode deixar nossa fonte de texto mais fina ou mais grossa

Os valores vão de 100 a 900, sendo 100 o mais fino

Algumas palavras também funcionam como valores, exemplo: 'bold(600)'

Existem fontes que não tem todas as variações, devemos ter cuidado com isso (e no caso do Google Fonts, já avisa qual o range de cada fonte)