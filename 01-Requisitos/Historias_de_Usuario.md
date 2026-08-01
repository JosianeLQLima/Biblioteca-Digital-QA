# Histórias de Usuário

**Projeto:** Biblioteca Digital QA
**Versão:** 1.0

---

# Objetivo

Este documento reúne as histórias de usuário da Biblioteca Digital, descrevendo as necessidades dos diferentes perfis do sistema. Cada história segue o formato:

> **Como** [perfil do usuário]
> **Quero** [funcionalidade]
> **Para** [benefício].

Também são apresentados os critérios de aceitação que servirão como base para a criação dos casos de teste.

---

# HU001 – Realizar Login

**Como** usuário cadastrado

**Quero** realizar login utilizando meu e-mail e senha

**Para** acessar as funcionalidades da Biblioteca Digital.

### Critérios de Aceitação

* O sistema deve solicitar e-mail e senha.
* Ambos os campos são obrigatórios.
* O login deve ser realizado apenas com credenciais válidas.
* Em caso de erro, o sistema deve apresentar uma mensagem informativa.
* Após autenticação, o usuário deve ser direcionado para a página inicial.

---

# HU002 – Recuperar Senha

**Como** usuário

**Quero** recuperar minha senha

**Para** voltar a acessar minha conta caso a esqueça.

### Critérios de Aceitação

* O usuário informa seu e-mail.
* O sistema envia um link de recuperação.
* O usuário consegue cadastrar uma nova senha.

---

# HU003 – Pesquisar Livros

**Como** usuário

**Quero** pesquisar livros

**Para** encontrar rapidamente um título de interesse.

### Critérios de Aceitação

* A pesquisa pode ser feita por título, autor, categoria ou ISBN.
* O sistema deve retornar apenas os resultados compatíveis com a pesquisa.
* Caso não existam resultados, uma mensagem deve ser apresentada.

---

# HU004 – Visualizar Detalhes do Livro

**Como** usuário

**Quero** visualizar as informações completas de um livro

**Para** decidir se desejo reservá-lo.

### Critérios de Aceitação

* Exibir título.
* Exibir autor.
* Exibir categoria.
* Exibir editora.
* Exibir descrição.
* Exibir disponibilidade.

---

# HU005 – Reservar Livro

**Como** usuário

**Quero** reservar um livro disponível

**Para** garantir meu empréstimo posteriormente.

### Critérios de Aceitação

* Apenas livros disponíveis podem ser reservados.
* O sistema deve registrar a reserva.
* Uma mensagem de sucesso deve ser apresentada.

---

# HU006 – Cancelar Reserva

**Como** usuário

**Quero** cancelar uma reserva

**Para** liberar o livro para outros usuários.

### Critérios de Aceitação

* O cancelamento deve ser permitido antes da retirada do livro.
* O sistema deve atualizar a disponibilidade do exemplar.

---

# HU007 – Consultar Histórico

**Como** usuário

**Quero** visualizar meu histórico

**Para** acompanhar empréstimos, devoluções e reservas realizadas.

### Critérios de Aceitação

* Exibir livros emprestados.
* Exibir reservas.
* Exibir devoluções.
* Exibir datas correspondentes.

---

# HU008 – Editar Perfil

**Como** usuário

**Quero** alterar minhas informações pessoais

**Para** manter meus dados atualizados.

### Critérios de Aceitação

* Permitir alteração do telefone.
* Permitir alteração da senha.
* Não permitir alteração do CPF.

---

# HU009 – Cadastrar Livro

**Como** administrador

**Quero** cadastrar novos livros

**Para** manter o acervo atualizado.

### Critérios de Aceitação

* Todos os campos obrigatórios devem ser preenchidos.
* O ISBN deve ser único.
* O sistema deve confirmar o cadastro.

---

# HU010 – Editar Livro

**Como** administrador

**Quero** editar informações dos livros

**Para** manter o cadastro atualizado.

### Critérios de Aceitação

* O sistema deve permitir alterar qualquer informação do livro.
* As alterações devem ser gravadas corretamente.

---

# HU011 – Excluir Livro

**Como** administrador

**Quero** excluir livros

**Para** remover registros desnecessários.

### Critérios de Aceitação

* Livros emprestados não podem ser excluídos.
* O sistema deve solicitar confirmação antes da exclusão.

---

# HU012 – Registrar Empréstimo

**Como** administrador

**Quero** registrar empréstimos

**Para** controlar a saída dos livros.

### Critérios de Aceitação

* Apenas livros disponíveis podem ser emprestados.
* O estoque deve ser atualizado automaticamente.
* A data prevista para devolução deve ser registrada.

---

# HU013 – Registrar Devolução

**Como** administrador

**Quero** registrar devoluções

**Para** disponibilizar novamente o livro para empréstimo.

### Critérios de Aceitação

* O sistema deve atualizar o estoque.
* O histórico do usuário deve ser atualizado.

---

# HU014 – Cadastrar Usuários

**Como** administrador

**Quero** cadastrar novos usuários

**Para** permitir acesso ao sistema.

### Critérios de Aceitação

* Nome, CPF, e-mail e senha são obrigatórios.
* O CPF deve ser único.
* O e-mail deve ser único.

---

# HU015 – Excluir Usuário

**Como** administrador

**Quero** excluir usuários

**Para** remover cadastros inativos.

### Critérios de Aceitação

* Usuários com empréstimos ativos não podem ser excluídos.
* O sistema deve solicitar confirmação antes da exclusão.

---

# HU016 – Visualizar Dashboard

**Como** administrador

**Quero** visualizar indicadores da biblioteca

**Para** acompanhar o funcionamento do sistema.

### Critérios de Aceitação

O dashboard deve apresentar:

* Quantidade de livros cadastrados.
* Quantidade de usuários.
* Empréstimos ativos.
* Reservas pendentes.
* Livros disponíveis.

---

# Resumo das Histórias de Usuário

| ID    | História             | Perfil        |
| ----- | -------------------- | ------------- |
| HU001 | Realizar Login       | Usuário       |
| HU002 | Recuperar Senha      | Usuário       |
| HU003 | Pesquisar Livros     | Usuário       |
| HU004 | Visualizar Livro     | Usuário       |
| HU005 | Reservar Livro       | Usuário       |
| HU006 | Cancelar Reserva     | Usuário       |
| HU007 | Consultar Histórico  | Usuário       |
| HU008 | Editar Perfil        | Usuário       |
| HU009 | Cadastrar Livro      | Administrador |
| HU010 | Editar Livro         | Administrador |
| HU011 | Excluir Livro        | Administrador |
| HU012 | Registrar Empréstimo | Administrador |
| HU013 | Registrar Devolução  | Administrador |
| HU014 | Cadastrar Usuários   | Administrador |
| HU015 | Excluir Usuário      | Administrador |
| HU016 | Visualizar Dashboard | Administrador |

---

# Observações

As histórias de usuário apresentadas neste documento servem como base para:

* elaboração dos casos de teste;
* criação dos checklists de validação;
* definição da matriz de rastreabilidade;
* documentação de bugs;
* planejamento e execução dos testes funcionais da Biblioteca Digital.
