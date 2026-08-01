# Requisitos Não Funcionais

**Projeto:** Biblioteca Digital QA
**Versão:** 1.0
**Objetivo:** Definir os requisitos não funcionais da aplicação Biblioteca Digital, estabelecendo critérios de qualidade, desempenho, segurança, usabilidade e compatibilidade que servirão de base para os testes.

---

# 1. Objetivo

Os requisitos não funcionais definem como o sistema deve se comportar em relação à qualidade, desempenho, segurança, disponibilidade e experiência do usuário.

---

# 2. Desempenho

## RNF001 – Tempo de Resposta

O sistema deve responder às solicitações do usuário em até **2 segundos** para operações comuns, como login, pesquisa e consulta de livros.

---

## RNF002 – Pesquisa

A pesquisa de livros deve retornar os resultados em até **3 segundos**, mesmo com uma base de dados de até 100.000 registros.

---

## RNF003 – Cadastro

O cadastro de livros e usuários deve ser concluído em até **2 segundos** após o envio das informações.

---

## RNF004 – Concorrência

O sistema deve suportar, no mínimo, **100 usuários simultâneos** sem perda significativa de desempenho.

---

# 3. Disponibilidade

## RNF005 – Disponibilidade

A aplicação deverá permanecer disponível **99,5% do tempo**, exceto durante manutenções programadas.

---

## RNF006 – Recuperação

Em caso de falha do servidor, o sistema deverá ser restaurado em até **30 minutos**.

---

# 4. Segurança

## RNF007 – Comunicação Segura

Toda comunicação entre cliente e servidor deverá utilizar o protocolo **HTTPS**.

---

## RNF008 – Armazenamento de Senhas

As senhas dos usuários não poderão ser armazenadas em texto simples, devendo utilizar algoritmos de criptografia seguros.

---

## RNF009 – Sessão

A sessão do usuário deverá expirar automaticamente após **30 minutos de inatividade**.

---

## RNF010 – Controle de Acesso

Apenas usuários autenticados poderão acessar áreas restritas do sistema.

---

## RNF011 – Permissões

Administradores terão acesso às funcionalidades administrativas, enquanto usuários comuns terão acesso apenas às funcionalidades permitidas para seu perfil.

---

# 5. Usabilidade

## RNF012 – Interface

A interface deverá ser intuitiva, organizada e de fácil utilização.

---

## RNF013 – Mensagens

Todas as mensagens de erro deverão ser claras, objetivas e indicar ao usuário como corrigir o problema.

---

## RNF014 – Campos Obrigatórios

Os campos obrigatórios deverão ser identificados visualmente.

---

## RNF015 – Navegação

O usuário deverá conseguir acessar qualquer funcionalidade em, no máximo, três cliques a partir da página inicial.

---

# 6. Compatibilidade

## RNF016 – Navegadores

O sistema deverá funcionar corretamente nas versões mais recentes dos seguintes navegadores:

* Google Chrome
* Microsoft Edge
* Mozilla Firefox

---

## RNF017 – Responsividade

A interface deverá adaptar-se corretamente às seguintes resoluções:

* Desktop
* Notebook
* Tablet
* Smartphone

---

# 7. Confiabilidade

## RNF018 – Integridade dos Dados

Nenhuma operação deverá gerar inconsistências no banco de dados.

---

## RNF019 – Backup

O banco de dados deverá possuir rotina diária de backup.

---

## RNF020 – Recuperação de Dados

Os dados deverão ser restauráveis a partir do último backup disponível.

---

# 8. Manutenibilidade

## RNF021 – Código

O sistema deverá possuir código organizado e documentado para facilitar futuras manutenções.

---

## RNF022 – Logs

Todas as operações críticas deverão ser registradas em logs para auditoria e análise de falhas.

---

# 9. Escalabilidade

## RNF023 – Crescimento

A aplicação deverá suportar crescimento do número de usuários e livros sem necessidade de alterações significativas na arquitetura.

---

# 10. Acessibilidade

## RNF024 – Navegação por Teclado

Todas as funcionalidades deverão ser acessíveis utilizando apenas o teclado.

---

## RNF025 – Contraste

As cores da interface deverão apresentar contraste suficiente para facilitar a leitura.

---

## RNF026 – Textos Alternativos

Imagens e ícones deverão possuir descrições alternativas quando necessário.

---

# 11. Critérios de Aceitação

* O tempo de resposta deve atender aos limites definidos.
* A aplicação deve funcionar corretamente nos navegadores suportados.
* O acesso deve ocorrer exclusivamente por conexão segura (HTTPS).
* Usuários sem permissão não devem acessar funcionalidades restritas.
* O sistema deve manter a integridade dos dados mesmo em situações de erro.
* A interface deve ser responsiva e de fácil utilização.
* Todas as mensagens de erro devem ser compreensíveis para o usuário.
* Os registros críticos devem ser armazenados em logs para auditoria.

---

# 12. Resumo dos Requisitos Não Funcionais

| ID     | Requisito                            | Categoria        |
| ------ | ------------------------------------ | ---------------- |
| RNF001 | Tempo de resposta                    | Desempenho       |
| RNF002 | Pesquisa rápida                      | Desempenho       |
| RNF003 | Cadastro rápido                      | Desempenho       |
| RNF004 | Usuários simultâneos                 | Desempenho       |
| RNF005 | Disponibilidade                      | Disponibilidade  |
| RNF006 | Recuperação do sistema               | Disponibilidade  |
| RNF007 | HTTPS                                | Segurança        |
| RNF008 | Criptografia de senhas               | Segurança        |
| RNF009 | Expiração de sessão                  | Segurança        |
| RNF010 | Controle de acesso                   | Segurança        |
| RNF011 | Permissões por perfil                | Segurança        |
| RNF012 | Interface intuitiva                  | Usabilidade      |
| RNF013 | Mensagens claras                     | Usabilidade      |
| RNF014 | Identificação de campos obrigatórios | Usabilidade      |
| RNF015 | Navegação simplificada               | Usabilidade      |
| RNF016 | Compatibilidade com navegadores      | Compatibilidade  |
| RNF017 | Responsividade                       | Compatibilidade  |
| RNF018 | Integridade dos dados                | Confiabilidade   |
| RNF019 | Backup diário                        | Confiabilidade   |
| RNF020 | Recuperação de dados                 | Confiabilidade   |
| RNF021 | Código organizado                    | Manutenibilidade |
| RNF022 | Registro de logs                     | Manutenibilidade |
| RNF023 | Escalabilidade                       | Escalabilidade   |
| RNF024 | Navegação por teclado                | Acessibilidade   |
| RNF025 | Contraste adequado                   | Acessibilidade   |
| RNF026 | Textos alternativos                  | Acessibilidade   |
