# Avaliação para Seleção - Desenvolvedor Sênior

## Objetivo

Criar um CRUD de cliente.

## Descrição

Antes de manipular os dados do cliente é necessário realizar a autenticação do usuário. Não se preocupe nesse momento em criar contas para o serviço.

Um usuário poderá se autenticar no sistema com duas contas diferentes:

| **Usuário** | **Senha** | **Observação** |
| --- | --- | --- |
| **admin** | 123456 | Esse usuário possui permissão total no sistema. |
| **comum** | 123456 | Esse usuário só tem permissão de visualização dos dados. |

Um registro de um cliente deverá ter os seguintes campos com suas respectivas regras:

| **Campo** | **Observação** |
| --- | --- |
| **Nome** | Mínimo de 3 caracteres; Máximo de 100 caracteres; Campo obrigatório; Permite apenas letras, espaços e números. |
| **CPF** | Sempre deve ser mostrado com máscara; Deve ser persistido na base sem máscara; É um campo obrigatório. |
| **Endereço** | Obrigatório preenchimento de CEP, logradouro, bairro, cidade e uf; Opcional complemento; Outros dados não devem ser preenchidos; Deve estar integrado com um serviço de consulta de CEP. Sugestão: https://viacep.com.br/; O usuário pode alterar os dados que vieram do serviço de consulta de CEP; O CEP deve ser mostrado com máscara; O CEP deve ser persistido sem máscara. |
| **Telefones** | Podem ser cadastrados múltiplos telefones; Pelo menos um telefone deve ser cadastrado; No cadastro de telefone, deve ser informado o tipo de telefone (residencial, comercial e celular) e o número; A máscara de telefone deve ser de acordo com o tipo de telefone (celular possui um digito a mais); O telefone deve ser mostrado com máscara; O telefone deve ser persistido sem máscara. |
| **E-mail** | Podem ser cadastrados múltiplos e-mails; Pelo menos um e-mail deve ser cadastrado; Deve ser um e-mail válido. |

## Restrições

- Todas as operações devem ser registradas no banco de dados contendo a data da operação e o usuário que realizou aquela operação;
- O sistema é web e você deve garantir que não haja problemas de concorrência na manipulação dos dados;
- O sistema deverá ser divido em dois projetos, um projeto para o front e outro para o serviço;
- O sistema deverá ser desenvolvido com as seguintes tecnologias:
  - Java 8;
  - Spring / Spring Boot;
  - Hibernate;
  - Maven;
  - Javascript ES6;
  - React.

Observação: você pode adicionar tecnologias a mais se achar necessário.

## Solução

### Código-fonte

O código-fonte se encontra nos seguintes caminhos:

| **Nome** | **Descrição** | **Endereco** |
| --- | --- | --- |
| **BD** | Referente ao banco de dados. | https://github.com/netinhoteixeira/avaliacao-selecao-desenvolvedor-senior-bd |
| **UI (React)** | Referente ao front-end em React. | https://github.com/netinhoteixeira/avaliacao-selecao-desenvolvedor-senior-ui-react |
| **UI (Angular)** | Referente ao front-end em Angular. | https://github.com/netinhoteixeira/avaliacao-selecao-desenvolvedor-senior-ui-angular |
| **API (Java)** | Referente ao back-end em Java. | https://github.com/netinhoteixeira/avaliacao-selecao-desenvolvedor-senior-api-java |

