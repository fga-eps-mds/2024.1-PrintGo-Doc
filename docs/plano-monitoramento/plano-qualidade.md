# Plano de Garantia de Qualidade

## Introdução

A qualidade de software é a gestão eficaz que visa criar um produto útil, proporcionando valor tanto para seus desenvolvedores quanto para seus usuários. Um software de alta qualidade é confiável, livre de erros, atende às necessidades dos usuários e melhora os processos de negócios. Este documento descreve as ferramentas e práticas utilizadas para assegurar a qualidade durante o desenvolvimento do projeto e define as métricas para avaliação da qualidade.

## Ferramentas

### SonarCloud

SonarCloud é utilizado para coletar e analisar métricas técnicas do código, ajudando a monitorar a qualidade. Métricas são capturadas a cada Pull Request (PR) e analisadas para avaliar a confiabilidade e manutenibilidade do código, orientando melhorias contínuas.

### Testes Unitários

Testes unitários são realizados para identificar e corrigir defeitos, não para provar a correção total do software. Esses testes automatizados verificam partes isoladas do código, garantindo a funcionalidade e robustez do sistema.

#### Jest

Jest é um framework de testes para JavaScript, utilizado tanto no frontend quanto em outros serviços do projeto. É conhecido por sua simplicidade e eficiência e é compatível com várias tecnologias, como Babel, TypeScript, Node, React e Angular.

## Verificação e Validação

A verificação confirma se o software realiza suas funções corretamente, enquanto a validação assegura que o produto atende às expectativas dos clientes. A equipe utiliza as seguintes técnicas:

**Validações com Stakeholders:** Reuniões semanais com Product Owners (POs) para validar o progresso e obter feedback.

**Análise Contínua do Código:** Uso do SonarCloud para análise estática, fornecendo métricas e identificando problemas no código-fonte.

**Testes Automatizados:** Realização de testes unitários e de integração durante o desenvolvimento e revisões de PRs para verificar cenários e lidar com erros inesperados.

**Revisão de Pull Requests:** Membros da equipe revisam PRs para garantir a qualidade e conformidade com as diretrizes do projeto antes da integração ao repositório principal.

## Métricas de Qualidade

As métricas ajudam a avaliar a eficiência dos processos e a qualidade do software. Elas devem ser claras, fáceis de calcular e baseadas em modelos de requisitos ou estrutura do software. As métricas definidas para este projeto incluem:

|**Métrica**|**Descrição**|
|-----------|-------------|
|Cobertura|Percentual de código coberto pelos testes|
|Duplicação|Percentual de código duplicado|
|Defeitos|Número de falhas identificadas|
|Code Smells|Indicadores de práticas inadequadas|
|Vulnerabilidades|Número de vulnerabilidades encontradas|
|Linhas|Número total de linhas de código|
|Pontos Críticos de Segurança|Avaliação de aspectos críticos de segurança|

Critérios mínimos para cada métrica:

|**Métrica**|**Critério**|
|-----------|------------|
|Cobertura|Pelo menos 80% de cobertura de testes|
|Duplicação|Até 3% de duplicação de código|
|Defeitos|Classificação "A"|
|Code Smells|Classificação "A"|
|Vulnerabilidades|Classificação "A"|
|Pontos Críticos de Segurança|Classificação "A"|

## Bibliografia

- PRESSMAN, Roger S.; MAXIM, Bruce R. *Engenharia de Software*. Grupo A, 2021. E-book. ISBN 9786558040118. Disponível em: <https://integrada.minhabiblioteca.com.br/#/books/9786558040118/>. Acesso em: 26 ago. 2024.

- DELAMARO, Marcio. *Introdução ao Teste de Software*. Grupo GEN, 2016. E-book. ISBN 9788595155732. Disponível em: <https://integrada.minhabiblioteca.com.br/#/books/9788595155732/>. Acesso em: 26 ago. 2024.