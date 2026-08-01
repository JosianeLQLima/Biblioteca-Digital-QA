# Escopo dos Testes

**Projeto:** Biblioteca Digital QA
**Versão:** 1.0
**Data:** Agosto/2026
**Autor:** Josiane Lima

---

# 1. Objetivo

Este documento define o escopo dos testes da aplicação **Biblioteca Digital**, especificando as funcionalidades que serão validadas durante o ciclo de testes, bem como os itens que não fazem parte deste projeto.

---

# 2. Objetivo dos Testes

O objetivo é verificar se a aplicação atende aos requisitos funcionais, não funcionais e às regras de negócio, assegurando a qualidade e o correto funcionamento das funcionalidades implementadas.

---

# 3. Funcionalidades no Escopo

As seguintes funcionalidades serão contempladas pelos testes.

## 3.1 Autenticação

* Login com credenciais válidas.
* Login com credenciais inválidas.
* Logout.
* Recuperação de senha.
* Validação de campos obrigatórios.
* Mensagens de erro.

---

## 3.2 Cadastro de Usuários

* Cadastro de novo usuário.
* Validação dos campos obrigatórios.
* Validação de CPF único.
* Validação de e-mail único.
* Alteração de dados.
* Exclusão de usuários conforme regras de negócio.

---

## 3.3 Gerenciamento de Livros

* Cadastro de livros.
* Alteração de livros.
* Exclusão de livros.
* Validação do ISBN.
* Atualização do estoque.
* Consulta de disponibilidade.

---

## 3.4 Pesquisa de Livros

* Pesquisa por título.
* Pesquisa por autor.
* Pesquisa por categoria.
* Pesquisa por ISBN.
* Pesquisa parcial.
* Pesquisa sem diferenciação entre letras maiúsculas e minúsculas.

---

## 3.5 Reserva de Livros

* Reserva de livros disponíveis.
* Bloqueio de livros indisponíveis.
* Cancelamento de reservas.
* Limite máximo de reservas por usuário.
* Atualização automática da disponibilidade.

---

## 3.6 Empréstimos

* Registro de empréstimos.
* Atualização do estoque.
* Controle de livros emprestados.
* Bloqueio de empréstimos duplicados.

---

## 3.7 Devoluções

* Registro de devoluções.
* Atualização do estoque.
* Atualização do histórico.
* Disponibilização do livro para novos empréstimos.

---

## 3.8 Histórico

* Consulta de empréstimos.
* Consulta de devoluções.
* Consulta de reservas.
* Exibição das datas das operações.

---

## 3.9 Dashboard Administrativo

* Quantidade de livros.
* Quantidade de usuários.
* Empréstimos ativos.
* Reservas pendentes.
* Livros disponíveis.

---

# 4. Tipos de Teste

Serão executados os seguintes tipos de teste:

* Testes Funcionais.
* Testes de Interface (UI).
* Testes de Validação.
* Testes de Integração.
* Testes de Regressão.
* Testes Exploratórios.

---

# 5. Ambientes de Teste

Os testes serão executados no seguinte ambiente:

* Sistema Operacional: Windows 11
* Navegadores: Google Chrome, Microsoft Edge e Mozilla Firefox
* Banco de Dados: PostgreSQL
* API REST
* Ferramentas: Postman, DevTools, GitHub, VS Code e Draw.io

---

# 6. Itens Fora do Escopo

As seguintes atividades não fazem parte deste projeto:

* Testes de carga.
* Testes de estresse.
* Testes de desempenho em produção.
* Testes de segurança avançados (Pentest).
* Testes de invasão.
* Testes de acessibilidade utilizando leitores de tela.
* Integrações com sistemas externos.
* Aplicativos móveis.
* Integração com serviços de pagamento.

---

# 7. Premissas

Para que os testes possam ser executados, considera-se que:

* Os requisitos estejam aprovados.
* O ambiente de testes esteja disponível.
* O banco de dados esteja configurado.
* Os usuários de teste estejam cadastrados.
* A aplicação esteja estável para execução dos testes.

---

# 8. Restrições

* O projeto contempla apenas a versão web da Biblioteca Digital.
* Os testes serão executados em ambiente de homologação.
* O sistema utilizará dados fictícios para validação.
* Não serão realizados testes em ambiente de produção.

---

# 9. Critérios de Sucesso

Os testes serão considerados concluídos quando:

* Todos os casos de teste planejados forem executados.
* Todos os requisitos funcionais forem validados.
* Não existirem defeitos críticos ou bloqueadores em aberto.
* As evidências dos testes estiverem registradas.
* Os relatórios de bugs estiverem documentados.

---

# 10. Resumo do Escopo

| Área                          | Incluído |
| ----------------------------- | -------- |
| Login e Logout                | ✔        |
| Recuperação de Senha          | ✔        |
| Cadastro de Usuários          | ✔        |
| Cadastro de Livros            | ✔        |
| Pesquisa de Livros            | ✔        |
| Reserva de Livros             | ✔        |
| Empréstimos                   | ✔        |
| Devoluções                    | ✔        |
| Histórico                     | ✔        |
| Dashboard                     | ✔        |
| Testes Funcionais             | ✔        |
| Testes de Interface           | ✔        |
| Testes de Integração          | ✔        |
| Testes de Regressão           | ✔        |
| Testes Exploratórios          | ✔        |
| Testes de Carga               | ✘        |
| Testes de Estresse            | ✘        |
| Testes de Segurança (Pentest) | ✘        |
| Aplicativo Mobile             | ✘        |
| Integrações Externas          | ✘        |

---

# 11. Conclusão

Este documento define claramente os limites do processo de testes da Biblioteca Digital, garantindo que todas as funcionalidades críticas sejam validadas e que o projeto possua um escopo bem definido para o planejamento, execução e documentação dos testes.
