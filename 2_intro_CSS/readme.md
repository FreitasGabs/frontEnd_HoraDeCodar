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
