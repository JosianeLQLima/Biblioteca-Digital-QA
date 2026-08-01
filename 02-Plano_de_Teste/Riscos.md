# Análise de Riscos

**Projeto:** Biblioteca Digital QA
**Versão:** 1.0
**Data:** Agosto/2026
**Autor:** Josiane Lima

---

# 1. Objetivo

Este documento identifica os principais riscos que podem impactar o planejamento, a execução e a conclusão dos testes da aplicação **Biblioteca Digital**, bem como as estratégias para reduzir seus impactos.

---

# 2. Classificação dos Riscos

Os riscos serão classificados conforme:

## Probabilidade

| Nível | Descrição                      |
| ----- | ------------------------------ |
| Baixa | Pouca chance de ocorrer        |
| Média | Pode ocorrer durante o projeto |
| Alta  | Grande chance de ocorrer       |

---

## Impacto

| Nível | Descrição                                               |
| ----- | ------------------------------------------------------- |
| Baixo | Pouco impacto no projeto                                |
| Médio | Pode atrasar algumas atividades                         |
| Alto  | Pode comprometer o cronograma ou a qualidade do projeto |

---

# 3. Matriz de Riscos

| ID     | Risco                                              | Probabilidade | Impacto | Prioridade |
| ------ | -------------------------------------------------- | ------------- | ------- | ---------- |
| RSK001 | Alteração de requisitos durante o projeto          | Média         | Alto    | Alta       |
| RSK002 | Ambiente de testes indisponível                    | Média         | Alto    | Alta       |
| RSK003 | Dados de teste inconsistentes                      | Média         | Médio   | Média      |
| RSK004 | Correções de bugs atrasadas                        | Alta          | Alto    | Alta       |
| RSK005 | Casos de teste incompletos                         | Baixa         | Alto    | Média      |
| RSK006 | Defeitos críticos encontrados no final da execução | Média         | Alto    | Alta       |
| RSK007 | Falha de comunicação entre equipe                  | Baixa         | Médio   | Média      |
| RSK008 | Instabilidade da aplicação                         | Média         | Alto    | Alta       |
| RSK009 | Problemas de integração entre Front-end e API      | Média         | Alto    | Alta       |
| RSK010 | Banco de dados indisponível                        | Baixa         | Alto    | Média      |

---

# 4. Estratégias de Mitigação

## RSK001 – Alteração de Requisitos

**Mitigação**

* Revisar os requisitos periodicamente.
* Atualizar os casos de teste e a matriz de rastreabilidade sempre que houver mudanças.

---

## RSK002 – Ambiente de Testes Indisponível

**Mitigação**

* Manter ambiente alternativo de homologação.
* Validar a disponibilidade antes do início da execução.

---

## RSK003 – Dados de Teste Inconsistentes

**Mitigação**

* Preparar uma massa de testes padronizada.
* Validar os dados antes da execução.

---

## RSK004 – Correções Atrasadas

**Mitigação**

* Priorizar bugs críticos e bloqueadores.
* Realizar acompanhamento periódico do status das correções.

---

## RSK005 – Casos de Teste Incompletos

**Mitigação**

* Revisar todos os casos de teste antes da execução.
* Garantir cobertura dos requisitos funcionais e regras de negócio.

---

## RSK006 – Defeitos Críticos

**Mitigação**

* Executar testes exploratórios durante todo o ciclo.
* Realizar testes de regressão após cada correção.

---

## RSK007 – Comunicação Ineficiente

**Mitigação**

* Registrar todas as decisões.
* Atualizar continuamente a documentação do projeto.

---

## RSK008 – Instabilidade da Aplicação

**Mitigação**

* Validar o ambiente antes da execução.
* Registrar ocorrências e interromper a execução quando necessário.

---

## RSK009 – Problemas de Integração

**Mitigação**

* Validar endpoints utilizando Postman.
* Confirmar os dados gravados no banco utilizando consultas SQL.

---

## RSK010 – Indisponibilidade do Banco de Dados

**Mitigação**

* Verificar a conectividade antes da execução.
* Utilizar backup da base de dados quando necessário.

---

# 5. Plano de Contingência

Caso algum risco de alta prioridade ocorra durante o projeto, deverão ser adotadas as seguintes ações:

* Replanejar o cronograma das atividades.
* Comunicar imediatamente os envolvidos.
* Priorizar a correção dos defeitos críticos.
* Atualizar a documentação do projeto.
* Reexecutar os testes impactados.

---

# 6. Monitoramento dos Riscos

Os riscos deverão ser avaliados durante todo o ciclo de testes.

Em cada fase do projeto será verificado:

* surgimento de novos riscos;
* alteração da probabilidade;
* alteração do impacto;
* necessidade de novas ações de mitigação.

---

# 7. Critérios de Priorização

Os riscos serão tratados conforme a prioridade abaixo:

| Prioridade | Ação                                             |
| ---------- | ------------------------------------------------ |
| Alta       | Acompanhamento contínuo e mitigação imediata     |
| Média      | Monitoramento periódico e plano de ação definido |
| Baixa      | Monitoramento durante o projeto                  |

---

# 8. Riscos Relacionados aos Testes

| Área                 | Possível Risco                               |
| -------------------- | -------------------------------------------- |
| Login                | Falha de autenticação                        |
| Cadastro de Usuários | Dados duplicados                             |
| Cadastro de Livros   | ISBN duplicado                               |
| Pesquisa             | Resultados incorretos                        |
| Reserva              | Reserva duplicada                            |
| Empréstimo           | Estoque inconsistente                        |
| Devolução            | Livro permanecer indisponível após devolução |
| Histórico            | Informações incompletas                      |
| Dashboard            | Indicadores desatualizados                   |
| API                  | Respostas incorretas ou indisponibilidade    |
| Banco de Dados       | Dados inconsistentes após operações          |

---

# 9. Indicadores de Risco

Durante o projeto serão monitorados os seguintes indicadores:

* Quantidade de bugs críticos encontrados.
* Quantidade de bugs bloqueadores.
* Percentual de casos de teste executados.
* Percentual de casos aprovados.
* Tempo médio para correção de defeitos.
* Quantidade de retestes realizados.
* Cobertura dos requisitos.

---

# 10. Conclusão

A identificação e o acompanhamento dos riscos permitem reduzir impactos no cronograma e aumentar a qualidade da aplicação. Este documento deve ser revisado sempre que ocorrerem mudanças relevantes nos requisitos, no ambiente de testes ou na estratégia de execução, garantindo que o projeto Biblioteca Digital QA seja conduzido de forma organizada e com maior previsibilidade.
