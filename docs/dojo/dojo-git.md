# Dojo de GIT/Github

## O que é GIT?

O Git é um sistema de controle de versão distribuído amplamente utilizado, projetado para gerenciar o desenvolvimento de software e rastrear mudanças no código-fonte ao longo do tempo. 
Ele oferece uma maneira eficiente e flexível de colaborar em projetos de software, facilitando o trabalho em equipe e o gerenciamento de código-fonte em diferentes ambientes de desenvolvimento.

## O que é Github?

O GitHub é uma plataforma de hospedagem de código-fonte e colaboração para projetos de software que utilizam o Git como sistema de controle de versão. 
Ele oferece uma variedade de recursos e ferramentas para desenvolvedores, equipes e organizações gerenciarem e colaborarem em projetos de software de forma eficiente.

## Proposta de Dojo

- Criar uma branch com o nome "dojo/dojo-docs"
- Criar uma issue
- Adicionar um arquivo com o nome "dojo-docs.md"
- Commitar a criação do documento apontando para a issue
- Alterar o arquivo
- Commitar as alterações do documento apontando para a issue
- Enviar as alterações para o repositório remoto
- Fazer um pull request para a branch master
- Adicionar revisores e comentários no pull request
- Aceitar o pull request
- Atualizar o repositório local com as alterações do repositório remoto realizado na master

## Configurar git na sua máquina

1. Configurar o nome do usuário:
```bash
git config --global user.name "Seu Nome"
```

2. Configurar o email do usuário:
```bash
git config --global user.email "Seu Email"
```
## Principais comandos

1. Clona um repositório: pega o repositório remoto e copia para a máquina local
```bash
git clone <url>
```

2. Adiciona um arquivo para ser commitado: 
```bash
git add <arquivo>
```

3. Commita as alterações: adiciona um comentário para o commit (precisa ser feito o push para enviar as alterações para o repositório remoto)
```bash
git commit -m "Mensagem do commit"
```

4. Envia as alterações para o repositório remoto:
```bash
git push
```

**Obs: faça o pull antes de enviar as alterações para o repositório remoto**

5. Atualiza o repositório local com as alterações do repositório remoto:
```bash
git pull
```

6. Pega todas as branches do repositório remoto: atualiza a lista de branches do repositório local
```bash
git fetch
```

7. Verifica o status do repositório: mostra os arquivos que foram alterados, adicionados ou removidos
```bash
git status
```

8. Troca de branch: muda de branch local
```bash
git checkout <branch>
```

# Como commmitar aponando para uma issue

- Isso ira apostar o commit para a issue #1

```bash
git commit -m "Mensagem do commit" -m "#1"
```

# Como commitar fechando uma issue

- Isso ira fechar a issue #1

```bash
git commit -m "Mensagem do commit" -m "Closes #1"
```


## Marcus Escobar

- Git é uma tecnologia foda, meu mano Linus Torvalds estava inspirado!!
- Não tive nenhuma dificuldade com o Dojo ,achei excelente. Daniel explica muito bem!!

## Caio Lamego

- Esse texto faz parte da tarefa do Dojo. 
- O Dojo foi ótimo

## Cairo Florenço

- Tava cometendo um erro bobo. ;-;

## Ana Júlia

- Aprendi que pra ver as branches remotas tem que colocar "-a" depois do git branch 👍

## Gustavo Feitosa 

- O Dojo tirou todas as dúvidas q eu tinha.
- Me ajudou a compreender como funcionam as etapas de commit e push.