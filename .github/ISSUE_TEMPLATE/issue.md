---
name: Issue
about: Template de issue
title: "[tipo] - Nome da issue"
labels: ''
assignees: ''

---

Para criar uma nova issue, um padrão deve ser seguido para dar o nome a issue:

[tipo] - Nome da issue

    [tipo] será o tipo da issue, podendo ser:
       - Feature - Para novas funcionalidades;
       - Bug - Para correção de bugs;
       - Docs - Para documentação.

    **Nome da issue é o nome da issue que será criada.**

Importante: O nome da issue deve descrever de forma clara e objetiva o que será feito e a descrição mais completa deverá ficar no corpo da issue.

### Descrição

Descreva de forma clara e concisa o problema ou a tarefa que a issue precisa abordar. Por exemplo:

"A funcionalidade de login com JWT tokens no Jitsi Meet não está autenticando corretamente os usuários, resultando em falhas ao tentar acessar as salas de reunião."

### Critérios de Aceitação

Liste os critérios que precisam ser atendidos para que a issue seja considerada resolvida. Por exemplo:

- [ ] Implementar a lógica de verificação de JWT tokens.
- [ ] Adicionar logs detalhados para falhas de autenticação.
- [ ] Atualizar a documentação do projeto.
- [ ] Criar e executar testes automatizados para os novos cenários.
- [ ] Validar a compatibilidade com todas as versões relevantes do Jitsi.
