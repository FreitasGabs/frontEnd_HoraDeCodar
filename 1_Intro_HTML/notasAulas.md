# Seção 3 - Introdução ao HTML 

## Aula 1 - A anatomia das tags

O Elemento principal do HTML é a tag;

Toda tag tem um nome e um propósito;

Precisamos envolver uma tag com sinais de menor e maior: \<tag>

E no meio colocar um conteúdo (a depender da tag) e adicionar tag de fechamento (também a depender da tag): \<tag>Conteúdo\</tag>

## Aula 2 - A estrutura base do HTML

Todos os projetos de HTML tem uma estrutura base, ou seja, precisamos criar algumas tags:

DOCTYPE: Esta tag declara a versão do HTML;

html: Esta tag envolve todo o código de HTML;

head: Nesta colocamos todas as configurações de um site, como a importação de CSS e o título da página (meta tags);

body: É onde todos os elementos visíveis estão.

## Aula 3 - Títulos

Os títulos são conhecidos como headings;

Utilizamos principalmente para separar seções;

O nome da tag é h*, onde * pode ser um valor de 1 a 6;

O maior título é o h1, e também é o mais importante, colocamos apenas um por página (questões de otimização de busca e indexação do conteúdo);

A importância deve estar conectada com o propósito da nossa página, esse assunto faz parte do HTML semântico. (ou seja, não se apegar somente ao tamanho do título, pois pode ser alterado com estilo, o foco é a importância semântica)

## Aula 4 - Parágrafos

Utilizamos os parágrafos para inserir textos maiores;

A tag é \<p>

Cada parágrafo começa uma nova linha, e este comportamento acontece com todas as tags de bloco;

Temos várias tags de bloco, os títulos fazem parte desse grupo.

## Aula 5 - Tags sem conteúdo

Nós temos em HTML tags sem conteúdo;
 
Elas possuem recursos geralmente, como quebrar linha;

Para este fim podemos utilizar a tag \<br/>

Para uma linha horizontal temos \<hr/>

(essas duas tags são do html anterior ao 5, e caíram em desuso, se utilizando do estilo para realizar essas ações)

Elas também introduzem o conceito de "self closing tags", onde a tag não possui uma outra tag de fechamento.

## Aula 6 - Comentários no HTML

Comentários são utilizados para descrever como algo funciona no nosso código;

Ou explicar a outros programadores o que fizemos;

Os comentários não são exibidos na página;

Mas qualquer inspeção de código terá acesso aos comentários.

## Aula 7 - Atributos

Atributos podem ser utilizados para adicionar funcionalidades às tags;

A tag 'a' é responsável por nos direcionar a uma nova página ou site;

Mas aonde vamos adicionar o endereço/URL?

Colocamos no atributo chamado 'href';

Um exemplo: \<a href="https://google.com">Google\</a>

Neste exemplo, ao clicar no link, o usuário é redirecionado ao Google.

### Aula 8 - Abrir link em nova aba

Com um atributo podemos fazer o link abrir em uma nova aba;

Isso é utilizado frequentemente para redirecionar a outro site;

Por exemplo: temos um link que leva a um e-commerce que não é nosso, não temos aquele domínio (então faz sentido abrir em outro lugar);

Então usamos o atributo 'target' com o valor '_blank'.

## Aula 9 - Imagens

Nós podemos inserir imagens no nosso site, com a tag 'img';

O caminho relativo até a imagem é inserido no atributo 'src';

Normalmente colocamos a imagem numa pasta chamada img ou assets, para fins de organização;

Nota: a imagem é uma self closing tag