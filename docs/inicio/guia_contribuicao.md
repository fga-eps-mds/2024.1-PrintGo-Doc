# Guia de Contribuição

## Introdução

&emsp;&emsp;Este guia tem como objetivo orientar os membros da equipe de desenvolvimento sobre as práticas e políticas de contribuição ao projeto. Aqui estão descritas as regras de versionamento, criação de issues, branches e commits, além de outras informações relevantes para o desenvolvimento do projeto.

## 1. Política de branches

&emsp;&emsp;As branches base do projeto são a [main](#main) e a [develop](#develop). A partir delas, são criadas as branches de desenvolvimento e correção de bugs.

### Main

&emsp;&emsp;Esta é a ramificação principal do projeto, onde está a versão mais atualizada do código.
Ela é protegida contra commits diretos e aceita apenas mesclagens de ramificações do tipo [hotfix](#hotfix) e da [develop](#develop). Funciona como a ramificação central do projeto, sendo única e essencial para a integridade do código. A exceção é para o repositório de documentação, que tem permissão para fazer commits diretamente nesta ramificação.

### Develop

&emsp;&emsp;A branch develop é o centro do desenvolvimento do código, mantendo a versão mais atualizada em progresso e integrando novas funcionalidades finalizadas por meio de pull requests. Única no projeto, ela não está presente no repositório de documentação e é protegida contra commits diretos.
Derivada da main, serve como ponto zero do desenvolvimento, sincronizando-se constantemente com todas as branches do projeto.

### 1.1. Novas branches

Para criar novas branches um padrão deve ser seguido para dar o nome a branch:

    <tipo>/x-nome-da-issue

- `<tipo>` será o tipo da branch, podendo ser:
    - `feature` - Para novas funcionalidades;
    - `bugfix` - Para correção de bugs;
    - `hotfix` - Para correção de bugs em produção;
    - `docs` - Para documentação.
- `x` é o número da issue que a branch está relacionada;

Exemplo:

    docs/3-criar-guia-de-contribuicao

### 1.2. Tipos de branches

- #### Feature 

    Esta é a ramificação designada para o desenvolvimento de uma nova funcionalidade do produto. Deve ser criada a partir da ramificação develop. 
    Após a conclusão do desenvolvimento da funcionalidade, deve ser mesclada de volta à ramificação [develop](#develop) por meio de uma solicitação pull. Após a mesclagem bem-sucedida, a ramificação deve ser excluída.

- #### Docs

    Esta é uma ramificação exclusiva para o repositório de documentação, utilizada para criar e manter documentos na wiki. Deve ser derivada da ramificação [main](#main).
    Após a finalização da documentação, é necessário mesclar a ramificação de volta à [main](#main) por meio de uma solicitação pull. Após a mesclagem bem-sucedida, a ramificação deve ser excluída.

- #### Bugfix

    Esta é a ramificação dedicada à implementação de soluções para bugs e erros identificados na [develop](#develop). Deve ser criada a partir da [develop](#develop). 
    Após resolver o problema abordado pela ramificação, ela deve ser mesclada de volta à [develop](#develop) por meio de uma solicitação pull. Após a mesclagem bem-sucedida, a ramificação deve ser removida.

- #### Hotfix

    Esta é a ramificação designada para a implementação de soluções para bugs e erros emergentes encontrados no ambiente de produção, representado pela [main](#main). Deve ser criada a partir da ramificação [main](#main). Após resolver o ponto abordado pela ramificação, ela deve ser mesclada de volta à [main](#main).
    Além disso, quando um hotfix é mesclado à [main](#main), também é necessário realizar a mesclagem da [main](#main) com a [develop](#develop).

### 1.3. Repositório de documentação

&emsp;&emsp;O repositório de documentação é um repositório separado dos repositórios de código fonte, que contém a documentação do projeto. A política de branches para o repositório de documentação é a mesma dos outros repositórios, com exceção da branch [develop](#develop) que não existe.

## 2. Template de issues

Foram criadas os seguintes templates de issues:

**Em repositórios de código**:

- Bug Report (Issue para reportar um bug);
- Feature (Issue para uma nova feature relacionada a uma história de usuário);

**No repositório de documentação**:

- História de Usuário (Issue para descrever uma história de usuário)

## 3. Política de commits
O padrão de commits a ser seguido é o [Conventional Commits](https://www.conventionalcommits.org/en/v1.0.0/), além das seguintes regras:

1. A descrição de um commit deve ser escrita em Português;
2. Um commit deve referenciar a issue trabalhada;
3. Um commit deve representar uma unidade de trabalho. Ou seja, não se deve incluir num único commit trabalhos relacionados a issues diferentes;

O padrão de commit é o seguinte:

    <tipo>[<escopo>]: <descrição>

    <corpo> (opcional)

    <footer> 

> Apenas o boby é um campo opcional
Exemplo de commit:

    feature[login]: Adiciona botão de login

    Adiciona botão de login na tela inicial do sistema.

    Refs: #3

Outro exemplo fechando uma issue:

    bugfix[login]: Corrige erro de autenticação

    Corrige erro de autenticação que impedia o login de usuários.

    Closes: #4

**Para realizar um commit com múltiplos autores, consulte a [documentação](https://docs.github.com/en/pull-requests/committing-changes-to-your-project/creating-and-editing-commits/creating-a-commit-with-multiple-authors).**

## 4. Política de Pull Requests

&emsp;&emsp;Para a criação de um Pull Request (PR), deve ser seguido o template já criado nos repositórios:

      ## Qual o tipo do PR?

      - [ ] Refactor
      - [ ] Feature
      - [ ] Bug Fix
      - [ ] Otimização
      - [ ] Documentação

      ## Descrição

      ## Issues relacionadas

      - Related Issue #
      - closes #


      ## Testes adicionados ou atualizados?

      - [ ] Sim;
      - [ ] Não, porque: **Inclua aqui o motivo de não ter incluido testes**;
      - [ ] Preciso de ajuda para implementar os testes;

## Versionamento

|**Data**|**Descrição**|**Autor(es)**|
|:-:|---|---|
| 07/04/2024 | Criação do Guia de Contribuição | Daniel Vinicius |
| 08/04/2024 | Revisão do Guia de Contribuição | Matheus Brant |
| 08/04/2024 | Revisão do Guia de Contribuição | Lucas Braun |
