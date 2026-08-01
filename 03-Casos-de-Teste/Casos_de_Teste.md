# Casos de Teste

## Projeto

**Biblioteca Digital QA**

---

## Visão Geral

Esta seção reúne todos os casos de teste elaborados para validar as funcionalidades da aplicação **Biblioteca Digital**.

Os casos de teste foram desenvolvidos com base nos requisitos funcionais, requisitos não funcionais, histórias de usuário e regras de negócio do projeto, seguindo as boas práticas de Garantia da Qualidade de Software (QA) e os princípios do ISTQB.

O objetivo é garantir que todas as funcionalidades críticas da aplicação sejam verificadas por meio de cenários positivos, negativos, validações de regras de negócio, testes de segurança e testes de interface.

---

## Objetivos

Os casos de teste têm como finalidade:

* Validar o funcionamento das funcionalidades da aplicação.
* Verificar o cumprimento dos requisitos definidos.
* Identificar possíveis defeitos antes da entrega do sistema.
* Garantir a integridade dos dados.
* Validar as regras de negócio.
* Assegurar uma boa experiência para o usuário.
* Apoiar a rastreabilidade entre requisitos e testes.

---

## Estrutura do Arquivo

O arquivo **`Casos_de_Teste.xlsx`** está organizado em abas, cada uma correspondente a um módulo da aplicação.

| Aba        | Funcionalidade                                  |
| ---------- | ----------------------------------------------- |
| Login      | Autenticação de usuários                        |
| Cadastro   | Cadastro e gerenciamento de usuários            |
| Livros     | Cadastro, edição, exclusão e pesquisa de livros |
| Reserva    | Reserva e cancelamento de livros                |
| Empréstimo | Registro e controle de empréstimos              |

---

## Estrutura dos Casos de Teste

Cada caso de teste contém as seguintes informações:

| Campo              | Descrição                                  |
| ------------------ | ------------------------------------------ |
| ID                 | Identificador único do caso de teste       |
| Caso de Teste      | Descrição da funcionalidade a ser validada |
| Prioridade         | Grau de importância da execução            |
| Pré-condição       | Condições necessárias antes da execução    |
| Passos             | Sequência de ações para execução do teste  |
| Dados de Teste     | Informações utilizadas durante a execução  |
| Resultado Esperado | Comportamento esperado do sistema          |
| Status             | Situação da execução do caso de teste      |

---

## Cobertura dos Testes

Os casos de teste contemplam:

* Testes Funcionais
* Testes Positivos
* Testes Negativos
* Classe de Equivalência
* Análise de Valores Limite
* Testes de Interface (UI)
* Testes de Regressão
* Testes Exploratórios
* Testes de Segurança (SQL Injection e XSS)
* Testes de Responsividade
* Testes de Desempenho
* Validação de Regras de Negócio

---

## Status dos Casos de Teste

Durante a execução, cada caso poderá assumir um dos seguintes status:

| Status        | Descrição                                               |
| ------------- | ------------------------------------------------------- |
| Não Executado | O teste ainda não foi realizado                         |
| Aprovado      | O resultado obtido corresponde ao esperado              |
| Reprovado     | Foi identificado um defeito durante a execução          |
| Bloqueado     | A execução não pôde ser concluída devido a impedimentos |

---

## Ferramentas Utilizadas

* Microsoft Excel
* GitHub
* PostgreSQL
* Postman
* Google Chrome
* Microsoft Edge
* Mozilla Firefox
* Visual Studio Code

---

## Documentos Relacionados

Os casos de teste foram elaborados com base nos seguintes documentos do projeto:

* Requisitos Funcionais
* Requisitos Não Funcionais
* Histórias de Usuário
* Regras de Negócio
* Plano de Testes
* Escopo
* Cronograma
* Análise de Riscos

---

## Organização do Repositório

```text
03-Casos-de-Teste/
│
├── README.md
└── Casos_de_Teste.xlsx
    ├── Login
    ├── Cadastro
    ├── Livros
    ├── Reserva
    └── Empréstimo
```

---

## Responsável

**QA Tester:** Josiane Lima

---

## Conclusão

Este conjunto de casos de teste foi elaborado para garantir uma cobertura abrangente das funcionalidades da Biblioteca Digital, proporcionando rastreabilidade entre os requisitos e a execução dos testes. A documentação demonstra a aplicação de boas práticas de QA e serve como evidência das atividades de planejamento e preparação para a validação do sistema.
