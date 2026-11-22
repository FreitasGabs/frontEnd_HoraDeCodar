# Seção 6 - Formulários

- Formulários tem o papel de receber dados do usuário, e enviar para um servidor;

- Podemos validar o dados;

- As tags mais utilizadas são: `<form>`, `<input>`, `<label>`;

- A tag `<form>` cria o formulário e o delimita;

- `<label>` define os inputs, e tem a função de melhorar a acessibilidade do formulário;

- E o `<input>` é o campo onde o usuário irá inserir os dados, e tem diversos tipos, como: `<number>`, `<text>`, `<email>`, `<password>`, `<submit>`, entre outros;

## Aula 1 - Criando nosso formulário

- Para criar um formulário vamos precisar da tag `<form>`, que encapsula todos os elementos do formulário;

- Dentro dela temos labels e inputs, mas podemos ter outras tags, como divs, fieldset, entre outras;

- A tag de input tem o atributo `type`, que define o tipo do campo, e o `name`, que é o nome do campo, e é importante para a identificação dos dados enviados;

- Um input do tipo `text` recebe dados de texto, por exemplo.

## Aula 2 - Atributos da tag form

- A tag `<form>` tem alguns atributos geralmente, que são:

  - `action`: o arquivo/página que os dados serão enviados;

  - `method`: GET ou POST, receber dados ou enviar dados;

- Não os exploraremos em detalhes nesse curso, pois são mais relacionados ao backend, mas é importante conhecer a existência deles.

### Aula 3 - Atributo name

- Utilizamos o atributo `name` para configurar os nossos inputs;

- O valor é ligado ao propósito do input, a sua categoria;

  - Exemplo: Um input que recebe a idade de um usuário, pode ter o name `idade`, ou `age`, ou algo relacionado a isso;

- O name é importante para a identificação dos dados enviados, e para a manipulação desses dados, seja no frontend ou no backend;

## Aula 4 - Atibuto da label

- A tag `<label>` tem o atributo `for`, que é utilizado para associar a label a um input específico;

- O valor deve ser o mesmo do `name` do atributo correspondente;

- A label é importante para a acessibilidade, pois permite que o usuário clique na label para focar no input correspondente, além de melhorar a experiência do usuário;

- É normalmente utilizada para propósitos semânticos e melhorar o ranking no Google.

## Aula 5 - Enviando os dados de formulário

- Podemos enviar os dados do form para um servidor através de um botão de submit, que é um input do tipo `submit`;

- Quando o usuário clica nesse botão, os dados do formulário são enviados para o servidor, e podemos manipular esses dados no backend;

- Os dados são enviados de acordo com o método definido no atributo `method` da tag `<form>`, que pode ser GET ou POST;

- Os dados serão enviados via requesição HTTP;

- Aqui é onde precisamos de um backend (não será visto nesse curso que é somente front) para receber esses dados, e processá-los, seja salvando em um banco de dados, ou realizando alguma ação com eles.

