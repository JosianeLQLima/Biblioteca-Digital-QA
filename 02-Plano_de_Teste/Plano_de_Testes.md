# Plano de Testes

**Projeto:** Biblioteca Digital QA
**Versão:** 1.0
**Data:** Julho/2026
**Autor:** Josiane Lima

---

# 1. Objetivo

Este Plano de Testes tem como objetivo definir a estratégia, o escopo, os recursos e os critérios para validar a qualidade da aplicação **Biblioteca Digital**, garantindo que suas funcionalidades atendam aos requisitos funcionais e não funcionais especificados.

---

# 2. Escopo

Serão testadas as principais funcionalidades da aplicação web:

* Autenticação (Login e Logout)
* Recuperação de Senha
* Cadastro de Usuários
* Gerenciamento de Livros
* Pesquisa de Livros
* Reserva de Livros
* Empréstimos
* Devoluções
* Histórico de Empréstimos
* Dashboard Administrativo

---

# 3. Objetivos dos Testes

Os testes têm como objetivo:

* Validar todas as funcionalidades do sistema.
* Garantir que as regras de negócio sejam respeitadas.
* Verificar o comportamento da aplicação diante de entradas válidas e inválidas.
* Confirmar que os requisitos funcionais e não funcionais foram implementados corretamente.
* Identificar defeitos antes da disponibilização do sistema.

---

# 4. Tipos de Teste

Serão executados os seguintes tipos de teste:

## Testes Funcionais

* Login
* Cadastro
* Pesquisa
* Reserva
* Empréstimo
* Devolução
* Histórico

---

## Testes de Interface (UI)

* Layout
* Navegação
* Responsividade
* Mensagens
* Campos obrigatórios

---

## Testes de Validação

* Campos obrigatórios
* Tamanho mínimo
* Tamanho máximo
* Caracteres permitidos
* Mensagens de erro

---

## Testes de Integração

* Comunicação entre Front-end e API
* Atualização do banco de dados
* Fluxo completo de empréstimos

---

## Testes de Regressão

Após correções de bugs, serão reexecutados os testes impactados para garantir que funcionalidades existentes continuem operando corretamente.

---

# 5. Itens a Serem Testados

| Funcionalidade       | Status |
| -------------------- | ------ |
| Login                | ✔      |
| Logout               | ✔      |
| Recuperação de Senha | ✔      |
| Cadastro de Usuários | ✔      |
| Cadastro de Livros   | ✔      |
| Pesquisa             | ✔      |
| Reserva              | ✔      |
| Empréstimos          | ✔      |
| Devoluções           | ✔      |
| Histórico            | ✔      |
| Dashboard            | ✔      |

---

# 6. Itens Fora do Escopo

Não fazem parte deste ciclo de testes:

* Testes de carga.
* Testes de estresse.
* Testes de invasão (Pentest).
* Integrações com sistemas externos.

---

# 7. Ambiente de Testes

## Sistema Operacional

* Windows 11

## Navegadores

* Google Chrome
* Microsoft Edge
* Mozilla Firefox

## Banco de Dados

* PostgreSQL

## API

* REST API

## Ferramentas

* Postman
* DevTools
* GitHub
* Draw.io
* Excel
* VS Code

---

# 8. Critérios de Entrada

Os testes poderão ser iniciados quando:

* Os requisitos estiverem aprovados.
* O ambiente de testes estiver disponível.
* A aplicação estiver implantada.
* Os dados de teste estiverem preparados.

---

# 9. Critérios de Saída

Os testes serão considerados concluídos quando:

* Todos os casos de teste forem executados.
* Todos os defeitos críticos forem corrigidos.
* Não existirem defeitos bloqueadores.
* O relatório final de testes estiver concluído.

---

# 10. Critérios de Aprovação

O sistema será considerado aprovado quando:

* 100% dos casos de teste críticos forem aprovados.
* Não existirem defeitos críticos ou bloqueadores em aberto.
* Os requisitos funcionais forem atendidos.
* As regras de negócio forem respeitadas.

---

# 11. Estratégia de Testes

A estratégia adotada será composta pelas seguintes etapas:

1. Análise dos requisitos.
2. Planejamento dos testes.
3. Elaboração dos casos de teste.
4. Revisão dos casos de teste.
5. Preparação do ambiente.
6. Execução dos testes.
7. Registro das evidências.
8. Registro de defeitos.
9. Reexecução dos testes após correções (reteste).
10. Testes de regressão.
11. Emissão do relatório final.

---

# 12. Papéis e Responsabilidades

| Papel         | Responsabilidade                          |
| ------------- | ----------------------------------------- |
| QA Tester     | Planejar, executar e documentar os testes |
| Desenvolvedor | Corrigir defeitos identificados           |
| Product Owner | Validar requisitos e regras de negócio    |

---

# 13. Riscos

| Risco                   | Impacto | Mitigação                                  |
| ----------------------- | ------- | ------------------------------------------ |
| Alteração de requisitos | Alto    | Revisar casos de teste                     |
| Ambiente indisponível   | Alto    | Planejar ambiente alternativo              |
| Dados inconsistentes    | Médio   | Preparar massa de testes antes da execução |
| Correções atrasadas     | Alto    | Priorizar defeitos críticos                |

---

# 14. Entregáveis

Ao final deste projeto serão entregues:

* Documento de Requisitos
* Plano de Testes
* Casos de Teste
* Checklist de Testes
* Relatórios de Bugs
* Evidências dos Testes
* Coleção Postman
* Scripts SQL
* Matriz de Rastreabilidade
* Apresentação Final

---

# 15. Cronograma

| Etapa                      | Status       |
| -------------------------- | ------------ |
| Levantamento de Requisitos | ✔            |
| Planejamento               | ✔            |
| Casos de Teste             | Em andamento |
| Execução                   | Pendente     |
| Registro de Bugs           | Pendente     |
| Retestes                   | Pendente     |
| Relatório Final            | Pendente     |

---

# 16. Métricas de Qualidade

Serão acompanhadas as seguintes métricas:

* Quantidade de casos de teste planejados.
* Quantidade de casos executados.
* Percentual de aprovação.
* Quantidade de bugs encontrados.
* Quantidade de bugs corrigidos.
* Distribuição de bugs por severidade.
* Cobertura de requisitos.

---

# 17. Aprovação

Este Plano de Testes servirá como referência para todas as atividades de garantia da qualidade da Biblioteca Digital, orientando a elaboração dos casos de teste, execução, registro de defeitos e validação final do sistema.

