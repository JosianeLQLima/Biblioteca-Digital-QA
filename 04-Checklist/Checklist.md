# Checklist de Testes

## Projeto

**Biblioteca Digital QA**

---

## Visão Geral

Esta seção reúne os **checklists de teste** desenvolvidos para apoiar a execução rápida das principais funcionalidades da aplicação **Biblioteca Digital**.

Os checklists foram elaborados com base nos requisitos funcionais, requisitos não funcionais, histórias de usuário e regras de negócio do projeto, servindo como apoio para testes exploratórios, testes de regressão, smoke tests e validações rápidas antes de novas versões da aplicação.

Diferentemente dos casos de teste detalhados, os checklists apresentam uma lista objetiva de verificações que permitem confirmar se as funcionalidades continuam operando conforme o esperado.

---

## Objetivos

Os checklists têm como finalidade:

* Validar rapidamente as funcionalidades críticas do sistema.
* Confirmar o correto funcionamento das principais telas.
* Verificar a aplicação das regras de negócio.
* Auxiliar na execução de testes exploratórios.
* Apoiar testes de regressão e smoke tests.
* Identificar rapidamente comportamentos inesperados.
* Garantir consistência entre versões da aplicação.

---

## Estrutura do Arquivo

O arquivo **`Checklist.xlsx`** está organizado em abas, cada uma correspondente a um módulo da aplicação.

| Aba        | Funcionalidade                      |
| ---------- | ----------------------------------- |
| Login      | Autenticação de usuários            |
| Cadastro   | Cadastro de usuários                |
| Livros     | Gerenciamento de livros             |
| Reserva    | Reserva de livros                   |
| Empréstimo | Registro e devolução de empréstimos |

---

## Estrutura do Checklist

Cada checklist contém os seguintes campos:

| Campo               | Descrição                                                |
| ------------------- | -------------------------------------------------------- |
| ID                  | Identificador único do item                              |
| Item de Verificação | Funcionalidade ou comportamento a ser validado           |
| Prioridade          | Grau de importância do item                              |
| Status              | Situação da execução                                     |
| Observações         | Campo destinado ao registro de evidências ou comentários |

---

## Cobertura dos Checklists

Os itens contemplam verificações relacionadas a:

* Interface do usuário (UI)
* Navegação entre telas
* Campos obrigatórios
* Validações de entrada
* Regras de negócio
* Controle de acesso e permissões
* Persistência dos dados
* Atualização do banco de dados
* Mensagens de sucesso e erro
* Segurança (SQL Injection e XSS)
* Responsividade
* Compatibilidade entre navegadores
* Desempenho das funcionalidades

---

## Status dos Itens

Durante a execução, cada item poderá assumir um dos seguintes status:

| Status        | Descrição                               |
| ------------- | --------------------------------------- |
| Não Executado | O item ainda não foi validado           |
| Aprovado      | O comportamento corresponde ao esperado |
| Reprovado     | Foi identificado um defeito             |
| Bloqueado     | A validação não pôde ser concluída      |

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

Os checklists foram elaborados com base na documentação do projeto:

* Requisitos Funcionais
* Requisitos Não Funcionais
* Histórias de Usuário
* Regras de Negócio
* Plano de Testes
* Casos de Teste
* Matriz de Rastreabilidade

---

## Organização do Repositório

```text
04-Checklist/
└── Checklist.xlsx
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

Este conjunto de checklists foi desenvolvido para fornecer uma forma prática e eficiente de validar as principais funcionalidades da Biblioteca Digital. Sua utilização reduz o tempo de execução dos testes, facilita a identificação de regressões e complementa os casos de teste detalhados, contribuindo para uma estratégia de Garantia da Qualidade (QA) mais completa e organizada.
