# Regras de Negócio

**Projeto:** Biblioteca Digital QA
**Versão:** 1.0

---

# Objetivo

Este documento descreve as regras de negócio da Biblioteca Digital. Essas regras definem como o sistema deve se comportar diante das operações realizadas pelos usuários e administradores, servindo como base para o desenvolvimento e para a elaboração dos casos de teste.

---

# Perfis de Usuário

## RN001 – Usuário

O usuário poderá:

* realizar login;
* pesquisar livros;
* visualizar detalhes dos livros;
* reservar livros disponíveis;
* cancelar reservas;
* consultar histórico de empréstimos;
* alterar sua senha e telefone.

O usuário **não poderá**:

* cadastrar livros;
* editar livros;
* excluir livros;
* cadastrar usuários;
* excluir usuários;
* registrar empréstimos;
* registrar devoluções.

---

## RN002 – Administrador

O administrador possui acesso completo ao sistema.

Pode:

* cadastrar livros;
* editar livros;
* excluir livros;
* cadastrar usuários;
* excluir usuários;
* registrar empréstimos;
* registrar devoluções;
* visualizar relatórios;
* acessar o dashboard administrativo.

---

# Autenticação

## RN003

Somente usuários cadastrados poderão acessar o sistema.

---

## RN004

O login deverá ser realizado utilizando e-mail e senha válidos.

---

## RN005

Após três tentativas consecutivas de login com senha incorreta, a conta deverá ser bloqueada por 15 minutos.

---

# Cadastro de Livros

## RN006

O ISBN deverá ser único.

Não poderá existir dois livros com o mesmo ISBN.

---

## RN007

Os seguintes campos são obrigatórios:

* ISBN
* Título
* Autor
* Categoria
* Quantidade

---

## RN008

A quantidade de exemplares deverá ser maior que zero.

---

## RN009

Somente administradores poderão cadastrar livros.

---

## RN010

Livros emprestados não poderão ser excluídos.

---

# Pesquisa de Livros

## RN011

A pesquisa deverá aceitar:

* título;
* autor;
* categoria;
* ISBN.

---

## RN012

A pesquisa deverá ignorar diferenças entre letras maiúsculas e minúsculas.

Exemplo:

"harry"

deve localizar

"Harry Potter".

---

# Reserva de Livros

## RN013

Somente livros disponíveis poderão ser reservados.

---

## RN014

Cada usuário poderá possuir no máximo **3 reservas ativas**.

---

## RN015

O mesmo usuário não poderá reservar o mesmo livro mais de uma vez simultaneamente.

---

## RN016

Ao cancelar uma reserva, o livro deverá voltar automaticamente para a lista de disponíveis.

---

# Empréstimos

## RN017

Somente administradores poderão registrar empréstimos.

---

## RN018

Um livro reservado deverá ficar indisponível para novos empréstimos até o cancelamento da reserva ou sua efetivação.

---

## RN019

Cada empréstimo deverá possuir:

* data do empréstimo;
* data prevista para devolução;
* usuário responsável;
* livro emprestado.

---

## RN020

Um livro emprestado não poderá ser emprestado novamente até sua devolução.

---

# Devoluções

## RN021

Após a devolução, o sistema deverá atualizar automaticamente a disponibilidade do livro.

---

## RN022

O histórico do usuário deverá registrar todas as devoluções realizadas.

---

# Usuários

## RN023

O CPF deverá ser único.

---

## RN024

O e-mail deverá ser único.

---

## RN025

Usuários com empréstimos ativos não poderão ser excluídos.

---

## RN026

O CPF não poderá ser alterado após o cadastro.

---

# Histórico

## RN027

O histórico deverá manter todos os registros de:

* empréstimos;
* devoluções;
* reservas;
* cancelamentos.

Os registros não poderão ser excluídos.

---

# Dashboard

## RN028

O dashboard administrativo deverá apresentar informações atualizadas em tempo real.

---

# Segurança

## RN029

Somente usuários autenticados poderão acessar páginas internas.

---

## RN030

Usuários sem permissão deverão receber mensagem de acesso negado ao tentar acessar funcionalidades restritas.

---

# Validações Gerais

## RN031

Todos os campos obrigatórios deverão ser validados antes da gravação.

---

## RN032

O sistema não deverá permitir registros duplicados quando existir restrição de unicidade.

---

## RN033

Mensagens de erro deverão ser exibidas sempre que ocorrer uma operação inválida.

---

# Fluxo Geral das Operações

```text
Login
   ↓
Página Inicial
   ↓
Pesquisar Livro
   ↓
Selecionar Livro
   ↓
Reservar Livro
   ↓
Registrar Empréstimo (Administrador)
   ↓
Registrar Devolução
   ↓
Atualizar Histórico
   ↓
Logout
```

---

# Resumo das Regras de Negócio

| ID    | Regra                                              | Categoria  |
| ----- | -------------------------------------------------- | ---------- |
| RN001 | Permissões do usuário                              | Perfil     |
| RN002 | Permissões do administrador                        | Perfil     |
| RN003 | Apenas usuários cadastrados acessam o sistema      | Login      |
| RN004 | Login por e-mail e senha                           | Login      |
| RN005 | Bloqueio após três tentativas inválidas            | Segurança  |
| RN006 | ISBN único                                         | Livros     |
| RN007 | Campos obrigatórios do livro                       | Livros     |
| RN008 | Quantidade maior que zero                          | Livros     |
| RN009 | Apenas administrador cadastra livros               | Livros     |
| RN010 | Livros emprestados não podem ser excluídos         | Livros     |
| RN011 | Pesquisa por título, autor, categoria e ISBN       | Pesquisa   |
| RN012 | Pesquisa sem diferenciar maiúsculas e minúsculas   | Pesquisa   |
| RN013 | Apenas livros disponíveis podem ser reservados     | Reserva    |
| RN014 | Máximo de três reservas por usuário                | Reserva    |
| RN015 | Não permitir reserva duplicada                     | Reserva    |
| RN016 | Cancelamento libera o livro                        | Reserva    |
| RN017 | Apenas administrador registra empréstimos          | Empréstimo |
| RN018 | Livro reservado fica indisponível                  | Empréstimo |
| RN019 | Empréstimo deve registrar datas e usuário          | Empréstimo |
| RN020 | Livro emprestado não pode ser emprestado novamente | Empréstimo |
| RN021 | Devolução atualiza disponibilidade                 | Devolução  |
| RN022 | Histórico registra devoluções                      | Devolução  |
| RN023 | CPF único                                          | Usuários   |
| RN024 | E-mail único                                       | Usuários   |
| RN025 | Usuário com empréstimo ativo não pode ser excluído | Usuários   |
| RN026 | CPF não pode ser alterado                          | Usuários   |
| RN027 | Histórico permanente                               | Histórico  |
| RN028 | Dashboard atualizado em tempo real                 | Dashboard  |
| RN029 | Acesso restrito a usuários autenticados            | Segurança  |
| RN030 | Controle de permissões                             | Segurança  |
| RN031 | Validação de campos obrigatórios                   | Geral      |
| RN032 | Não permitir registros duplicados                  | Geral      |
| RN033 | Exibir mensagens de erro em operações inválidas    | Geral      |

