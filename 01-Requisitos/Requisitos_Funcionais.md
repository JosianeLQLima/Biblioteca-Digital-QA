# Documento de Requisitos Funcionais

# Biblioteca Digital

**Versão:** 1.0
**Projeto:** Biblioteca Digital QA
**Autor:** Josiane Lima
**Objetivo:** Definir os requisitos funcionais da aplicação Biblioteca Digital que servirão de base para planejamento, execução e documentação dos testes.

---

# 1. Objetivo do Sistema

A Biblioteca Digital é um sistema web destinado ao gerenciamento de livros, usuários e empréstimos. O sistema permite que usuários pesquisem livros, realizem reservas e acompanhem seus empréstimos, enquanto administradores gerenciam o acervo.

---

# 2. Perfis de Usuário

## Administrador

Possui acesso completo ao sistema.

Pode:

* realizar login
* cadastrar livros
* editar livros
* excluir livros
* cadastrar usuários
* aprovar empréstimos
* visualizar relatórios

---

## Usuário

Pode:

* realizar login
* pesquisar livros
* reservar livros
* cancelar reservas
* visualizar histórico
* editar seu perfil

---

# 3. Funcionalidades

## RF001 – Login

O sistema deve permitir que usuários autenticados realizem login utilizando e-mail e senha.

### Regras

* e-mail obrigatório
* senha obrigatória
* senha mascarada
* botão Entrar
* botão Esqueci minha senha
* lembrar usuário (opcional)

### Resultado esperado

Usuário autenticado é direcionado para a página inicial.

---

## RF002 – Logout

O usuário poderá encerrar sua sessão.

Resultado esperado:

Retornar para a tela de login.

---

## RF003 – Recuperação de Senha

O sistema deverá permitir recuperação da senha.

Fluxo:

* informar e-mail
* receber link
* cadastrar nova senha

---

## RF004 – Cadastro de Livros

Administrador poderá cadastrar livros.

Campos

* ISBN
* Título
* Autor
* Categoria
* Editora
* Ano
* Quantidade
* Descrição
* Imagem

Campos obrigatórios

* ISBN
* Título
* Autor
* Categoria
* Quantidade

---

## RF005 – Alteração de Livro

Administrador poderá editar qualquer informação do livro.

---

## RF006 – Exclusão de Livro

Administrador poderá excluir livros.

Regra:

Não poderá excluir livros emprestados.

---

## RF007 – Consulta de Livros

Usuário poderá pesquisar livros.

Filtros

* título
* autor
* categoria
* ISBN

---

## RF008 – Visualizar Livro

Ao selecionar um livro deverão ser exibidos:

* capa
* autor
* descrição
* disponibilidade
* categoria
* editora
* quantidade disponível

---

## RF009 – Reserva

Usuário poderá reservar um livro disponível.

Resultado esperado

Reserva criada com sucesso.

---

## RF010 – Cancelamento da Reserva

Usuário poderá cancelar reserva antes da retirada.

---

## RF011 – Empréstimo

Administrador registra empréstimo.

Campos

* usuário
* livro
* data
* devolução prevista

---

## RF012 – Devolução

Administrador registra devolução.

Resultado esperado

Livro retorna ao estoque.

---

## RF013 – Histórico

Usuário visualiza:

* livros emprestados
* reservas
* devoluções

---

## RF014 – Cadastro de Usuários

Administrador poderá cadastrar usuários.

Campos

* Nome
* Sobrenome
* CPF
* E-mail
* Telefone
* Senha

---

## RF015 – Alteração de Perfil

Usuário poderá editar

* telefone
* senha

Não poderá alterar CPF.

---

## RF016 – Exclusão de Usuário

Administrador poderá excluir usuários.

Restrição

Usuário com empréstimo ativo não pode ser excluído.

---

## RF017 – Dashboard

Administrador visualiza

* livros cadastrados
* empréstimos ativos
* reservas
* usuários cadastrados

---

## RF018 – Pesquisa

Sistema deverá permitir pesquisa parcial.

Exemplo

Pesquisar

"har"

Resultado

Harry Potter

---

## RF019 – Paginação

Listagem deve possuir paginação.

20 registros por página.

---

## RF020 – Ordenação

Livros poderão ser ordenados por

* título
* autor
* categoria
* data

---

# 4. Mensagens do Sistema

Login inválido

"E-mail ou senha inválidos."

Cadastro realizado

"Cadastro realizado com sucesso."

Livro reservado

"Reserva realizada com sucesso."

Livro devolvido

"Livro devolvido com sucesso."

Campos obrigatórios

"Campo obrigatório."

Erro inesperado

"Ocorreu um erro. Tente novamente."

---

# 5. Fluxo Principal

Login

↓

Página Inicial

↓

Pesquisar Livro

↓

Visualizar Livro

↓

Reservar

↓

Empréstimo

↓

Devolução

↓

Histórico

↓

Logout

---

# 6. Critérios de Aceitação

* Todos os campos obrigatórios devem ser validados.
* Nenhum cadastro poderá conter dados inválidos.
* Mensagens de erro devem ser exibidas ao usuário.
* Apenas administradores podem gerenciar livros.
* Apenas usuários autenticados acessam funcionalidades protegidas.
* O sistema deve atualizar disponibilidade após empréstimos e devoluções.

---

# 7. Dependências

* Banco de dados
* API REST
* Serviço de autenticação
* Navegador compatível

---

# 8. Prioridade dos Requisitos

| ID    | Requisito            | Prioridade |
| ----- | -------------------- | ---------- |
| RF001 | Login                | Alta       |
| RF002 | Logout               | Média      |
| RF003 | Recuperação de senha | Média      |
| RF004 | Cadastro de livros   | Alta       |
| RF005 | Editar livro         | Alta       |
| RF006 | Excluir livro        | Alta       |
| RF007 | Pesquisa             | Alta       |
| RF008 | Visualizar livro     | Alta       |
| RF009 | Reserva              | Alta       |
| RF010 | Cancelar reserva     | Média      |
| RF011 | Empréstimo           | Alta       |
| RF012 | Devolução            | Alta       |
| RF013 | Histórico            | Média      |
| RF014 | Cadastro de usuários | Alta       |
| RF015 | Editar perfil        | Média      |
| RF016 | Excluir usuário      | Alta       |
| RF017 | Dashboard            | Baixa      |
| RF018 | Pesquisa parcial     | Média      |
| RF019 | Paginação            | Baixa      |
| RF020 | Ordenação            | Baixa      |
