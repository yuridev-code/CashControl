# PRD Executivo — CashControl

| Campo                 | Valor                                        |
| --------------------- | -------------------------------------------- |
| **Produto**           | CashControl                                  |
| **Versão**            | v1.0                                         |
| **Autor / PO / Dev**  | Yuri                                         |
| **Data do documento** | 21/09/2026                                   |
| **Data-alvo do MVP**  | 19/01/2027                                   |
| **Status**            | Em definição / Pré-desenvolvimento           |
| **Categoria**         | Aplicação web de controle financeiro pessoal |

---

# 1. Capa do Documento

## CashControl — PRD Executivo v1.0

**Propósito do documento:** estabelecer uma especificação executiva e rastreável para orientar o desenvolvimento individual do MVP do CashControl.

**Escopo temporal:** MVP com entrega prevista para **19 de janeiro de 2027**.

**Modelo de execução:** Product Owner + Designer + Engenheiro, executados por Yuri.

**Princípio de escopo:** priorizar uma aplicação web funcional de planejamento e acompanhamento financeiro, sem movimentação de dinheiro real e sem integrações externas de dados financeiros no MVP.

---

# 2. Sumário Executivo

## Problema

Pessoas que recebem renda mensal frequentemente sabem quanto ganham, mas não possuem uma visão estruturada de **quanto podem gastar, quanto deveriam economizar e como seu comportamento financeiro evolui ao longo do tempo**.

Planilhas e controles manuais permitem registrar informações, mas podem gerar excesso de trabalho e dificultar comparações mensais.

## Solução

O CashControl centraliza o controle financeiro pessoal em uma aplicação web.

O usuário poderá:

1. cadastrar sua renda;
2. definir uma distribuição planejada;
3. registrar despesas, lazer, investimentos e economia;
4. acompanhar o resultado mensal;
5. comparar o mês atual com períodos anteriores;
6. visualizar sua evolução financeira.

A distribuição inicial terá como referência a metodologia **50/20/30**, mas será personalizável.

> **Informação pendente:** a correspondência exata entre a metodologia 50/20/30 e as quatro categorias do CashControl ainda precisa ser definida.

## Público

**Primário:** pessoas com renda mensal recorrente, incluindo assalariados, CLT e profissionais PJ com receita previsível.

**Secundário:** empresários e autônomos com renda fracionada.

## Diferencial

O diferencial central do MVP não será movimentar dinheiro, mas transformar a renda recebida em um **plano financeiro visual, registrável e comparável ao longo do tempo**.

## Status atual

O produto encontra-se em fase de definição. O principal objetivo desta versão do PRD é transformar a visão do produto em requisitos implementáveis e explicitar as decisões ainda pendentes.

### Decisão de escopo relevante

O contexto inicial listava **IA, 2FA e análise financeira via IA** dentro do MVP, mas também estabelecia explicitamente que esses recursos **não fazem parte do MVP de janeiro/2027**.

**Decisão v1.0:** prevalece a regra explícita de exclusão. IA, 2FA e integrações bancárias estão fora do MVP e permanecem no roadmap.

---

# 3. Visão Geral do Produto

## 3.1 Contexto

O CashControl será uma aplicação web B2C de planejamento financeiro pessoal.

O sistema não terá acesso a contas bancárias nem realizará pagamentos, transferências ou investimentos reais.

Toda informação financeira do MVP será informada manualmente pelo usuário.

## 3.2 Problema de Produto

O usuário precisa responder rapidamente perguntas como:

* Quanto recebi este mês?
* Quanto posso direcionar para cada categoria?
* Quanto já gastei?
* Quanto consegui economizar?
* Estou gastando mais ou menos que nos meses anteriores?
* Como meu comportamento financeiro está evoluindo?

O produto deve reduzir o esforço necessário para responder essas perguntas.

## 3.3 Proposta de Valor

> **"Transforme sua renda mensal em um plano claro, visual e comparável ao longo do tempo — sem precisar conectar sua conta bancária."**

## 3.4 Público-Alvo

| Público    | Características           | Necessidade principal                                  |
| ---------- | ------------------------- | ------------------------------------------------------ |
| Primário   | Renda mensal recorrente   | Planejar e controlar o mês                             |
| Secundário | Renda fracionada/variável | Consolidar entradas e acompanhar capacidade financeira |

## 3.5 Job to Be Done

> Quando recebo dinheiro durante o mês, quero saber quanto devo reservar, quanto posso gastar e como estou evoluindo em relação aos meses anteriores, para tomar decisões financeiras com maior clareza.

## 3.6 Princípios do Produto

| Princípio             | Aplicação                                                               |
| --------------------- | ----------------------------------------------------------------------- |
| Simplicidade          | Registrar informações deve exigir poucos passos                         |
| Transparência         | Valores calculados devem ser explicáveis                                |
| Comparabilidade       | O histórico deve permitir comparação entre períodos                     |
| Controle pelo usuário | Categorias e percentuais devem ser personalizáveis                      |
| Segurança             | Dados financeiros devem ser protegidos mesmo sem movimentação monetária |
| Escopo disciplinado   | Recursos não essenciais ao MVP devem permanecer fora do lançamento      |

---

# 4. Objetivos de Negócio e OKRs

## 4.1 Objetivos Estratégicos

### Objetivo 1 — Reduzir despesas do usuário

Aumentar a visibilidade sobre os gastos para favorecer decisões de consumo mais conscientes.

### Objetivo 2 — Aumentar a capacidade de economia

Permitir que o usuário identifique, acompanhe e compare quanto consegue reservar ao longo dos meses.

### Objetivo 3 — Melhorar o planejamento financeiro pessoal

Transformar renda e gastos históricos em informações comparáveis para apoiar planejamento futuro.

---

## 4.2 OKRs Provisórios

> **Nota:** as metas percentuais abaixo são **suposições iniciais** e devem ser calibradas após testes com usuários e definição do baseline.

### O1 — Aumentar a adoção do planejamento mensal

| Key Result | Indicador                                                                         |
| ---------- | --------------------------------------------------------------------------------- |
| KR1.1      | Aumentar a proporção de usuários ativos que cadastram renda e distribuição mensal |
| KR1.2      | Aumentar a proporção de usuários que registram pelo menos uma transação por mês   |
| KR1.3      | Aumentar a proporção de usuários que consultam histórico ou comparação mensal     |

### O2 — Melhorar o comportamento de economia

| Key Result | Indicador                                                                            |
| ---------- | ------------------------------------------------------------------------------------ |
| KR2.1      | Medir evolução da economia média por usuário entre meses comparáveis                 |
| KR2.2      | Medir evolução da proporção da renda destinada à economia                            |
| KR2.3      | Identificar usuários que mantêm registro financeiro por múltiplos meses consecutivos |

### O3 — Melhorar a qualidade do planejamento

| Key Result | Indicador                                                                  |
| ---------- | -------------------------------------------------------------------------- |
| KR3.1      | Medir percentual de usuários com distribuição definida para o mês          |
| KR3.2      | Medir percentual de meses com planejamento e consolidação completos        |
| KR3.3      | Medir taxa de conclusão do fluxo renda → distribuição → registro → análise |

---

## 4.3 North Star Metric

### Métrica proposta: Meses Financeiros Completos por Usuário Ativo

**Definição provisória:**

Quantidade média de meses em que um usuário ativo:

1. cadastrou renda;
2. possui distribuição planejada;
3. registrou movimentações financeiras;
4. possui consolidação mensal disponível.

**Fórmula conceitual:**

`MFC = quantidade de meses completos / usuários ativos no período`

### Justificativa

A métrica mede a criação de hábito e o uso efetivo do produto, evitando que o sucesso seja definido apenas por número de cadastros.

> **Validação pendente:** definir exatamente o que caracteriza um “mês completo”.

---

# 5. Escopo

## 5.1 Dentro do Escopo — MVP

| Item                                                     | Status                       |
| -------------------------------------------------------- | ---------------------------- |
| Cadastro de usuário                                      | MVP                          |
| Login                                                    | MVP                          |
| Recuperação de acesso                                    | MVP                          |
| Cadastro de renda                                        | MVP                          |
| Distribuição planejada da renda                          | MVP                          |
| Referência 50/20/30                                      | MVP                          |
| Personalização de distribuição                           | MVP                          |
| Categorias personalizáveis                               | MVP                          |
| Registro de despesas                                     | MVP                          |
| Registro de lazer                                        | MVP                          |
| Registro de investimentos                                | MVP                          |
| Registro de economia                                     | MVP                          |
| Histórico mensal                                         | MVP                          |
| Comparação com meses anteriores                          | MVP                          |
| Cálculo de economia                                      | MVP                          |
| Consolidação financeira mensal                           | MVP                          |
| Gráficos básicos                                         | Could, condicionado ao prazo |
| Análise financeira baseada em regras e dados registrados | MVP                          |
| IA generativa / chatbot                                  | Fora do MVP                  |
| 2FA                                                      | Fora do MVP                  |
| Integração bancária / Open Finance                       | Fora do MVP                  |

## 5.2 Fora do Escopo — Roadmap

| Item                                 | Roadmap |
| ------------------------------------ | ------- |
| Chatbot com IA                       | v2.0    |
| Análise financeira via IA            | v2.0    |
| Autenticação 2FA                     | v2.0    |
| Integrações bancárias / Open Finance | v2.0    |
| Aplicativos iOS / Android            | Futuro  |
| Movimentação de dinheiro real        | Futuro  |
| Automatizações avançadas             | Futuro  |

## 5.3 Premissas

1. O CashControl não movimenta dinheiro real.
2. Os dados financeiros do MVP são inseridos manualmente.
3. A distribuição possui uma configuração inicial baseada em 50/20/30.
4. O usuário pode personalizar as categorias e percentuais.
5. O histórico depende da qualidade dos dados inseridos.
6. A comparação histórica utilizará dados registrados no próprio CashControl.
7. O produto será exclusivamente web no MVP.
8. O projeto será desenvolvido individualmente por Yuri.
9. O MVP tem data-alvo de 19/01/2027.
10. IA, 2FA e integrações bancárias não fazem parte da entrega do MVP.

## 5.4 Restrições

| Restrição                    | Impacto                                                                     |
| ---------------------------- | --------------------------------------------------------------------------- |
| Desenvolvimento individual   | Capacidade limitada de execução simultânea                                  |
| Prazo até 19/01/2027         | Exige priorização rígida                                                    |
| Aplicação exclusivamente web | Não haverá aplicativo nativo no MVP                                         |
| Entrada manual dos dados     | Qualidade das análises depende do usuário                                   |
| Sem integração bancária      | Não haverá sincronização automática                                         |
| Sem IA no MVP                | Insights precisam ser determinísticos ou baseados em cálculos pré-definidos |

---

# 6. Stakeholders

## 6.1 Stakeholders

| Nome          | Papel                         | Interesse | Influência | Responsabilidade                                  |
| ------------- | ----------------------------- | --------- | ---------- | ------------------------------------------------- |
| Yuri          | Product Owner, Designer e Dev | Alta      | Alta       | Definir, projetar, implementar, testar e entregar |
| Usuário final | Consumidor                    | Alta      | Média      | Utilizar o produto, fornecer dados e feedback     |

> **Classificação de influência e interesse:** provisória.

## 6.2 Matriz Influência × Interesse

|                            | **Baixo Interesse** | **Alto Interesse**                                                      |
| -------------------------- | ------------------- | ----------------------------------------------------------------------- |
| **Alta Influência**        | —                   | **Yuri** — gerenciar diretamente                                        |
| **Baixa/Média Influência** | —                   | **Usuário final** — observar feedback, comportamento e problemas de uso |

### Estratégia

**Yuri:** centralizar decisões de produto, engenharia, UX e lançamento.

**Usuário final:** utilizar pesquisas, testes de usabilidade e métricas comportamentais para validar hipóteses.

---

# 7. Requisitos Funcionais

## 7.1 Cadastro e Autenticação

| ID     | Descrição                                                                   | Prioridade | Critério de Aceite                                                             |
| ------ | --------------------------------------------------------------------------- | ---------- | ------------------------------------------------------------------------------ |
| RF-001 | Permitir criação de conta com dados mínimos necessários                     | **Must**   | Usuário consegue criar conta válida e receber confirmação visual de sucesso    |
| RF-002 | Permitir login com credenciais cadastradas                                  | **Must**   | Credenciais válidas autenticam; inválidas retornam mensagem de erro            |
| RF-003 | Permitir encerramento de sessão                                             | **Must**   | Usuário pode sair da conta e não acessar páginas autenticadas após logout      |
| RF-004 | Permitir recuperação de acesso por e-mail                                   | **Must**   | Usuário consegue solicitar recuperação e redefinir senha mediante token válido |
| RF-005 | Impedir reutilização/aceitação de token de recuperação expirado ou inválido | **Must**   | Token inválido, expirado ou já utilizado é recusado                            |

## 7.2 Renda e Planejamento

| ID     | Descrição                                            | Prioridade | Critério de Aceite                                                                 |
| ------ | ---------------------------------------------------- | ---------- | ---------------------------------------------------------------------------------- |
| RF-006 | Permitir cadastrar renda                             | **Must**   | Usuário consegue informar valor, data/período e salvar a renda                     |
| RF-007 | Permitir editar ou excluir renda cadastrada          | **Must**   | Alterações refletem nos cálculos posteriores                                       |
| RF-008 | Gerar distribuição planejada da renda                | **Must**   | Sistema calcula valores por categoria a partir de percentuais configurados         |
| RF-009 | Disponibilizar referência baseada em 50/20/30        | **Must**   | Usuário consegue aplicar a configuração de referência                              |
| RF-010 | Permitir personalizar os percentuais da distribuição | **Must**   | Usuário consegue alterar percentuais respeitando as regras definidas               |
| RF-011 | Impedir distribuição percentual inconsistente        | **Must**   | Sistema bloqueia configuração que viole a regra definida para soma dos percentuais |

> **Informação pendente:** a regra exata de soma dos percentuais e o mapeamento 50/20/30 → quatro categorias precisam ser definidos antes da implementação final.

## 7.3 Categorias e Registros

| ID     | Descrição                                                           | Prioridade | Critério de Aceite                                                             |
| ------ | ------------------------------------------------------------------- | ---------- | ------------------------------------------------------------------------------ |
| RF-012 | Permitir criar categoria personalizada                              | **Must**   | Usuário consegue criar categoria com nome válido                               |
| RF-013 | Permitir editar e excluir categorias conforme regras de integridade | **Should** | Categoria sem dependências pode ser alterada/removida; histórico não é perdido |
| RF-014 | Permitir registrar despesas                                         | **Must**   | Usuário consegue registrar valor, categoria, data e descrição mínima           |
| RF-015 | Permitir registrar lazer                                            | **Must**   | Registro pode ser associado à categoria de lazer                               |
| RF-016 | Permitir registrar investimentos                                    | **Must**   | Usuário consegue registrar valor e data de investimento                        |
| RF-017 | Permitir registrar economia                                         | **Must**   | Usuário consegue registrar valor destinado à economia                          |
| RF-018 | Permitir editar e excluir registros financeiros                     | **Must**   | Alteração ou exclusão atualiza corretamente os agregados                       |

## 7.4 Histórico e Análise

| ID     | Descrição                                               | Prioridade | Critério de Aceite                                                                 |
| ------ | ------------------------------------------------------- | ---------- | ---------------------------------------------------------------------------------- |
| RF-019 | Exibir resumo financeiro mensal                         | **Must**   | Sistema exibe renda, distribuição, registros e economia do período                 |
| RF-020 | Manter histórico mensal                                 | **Must**   | Usuário pode consultar meses anteriores sem sobrescrever dados históricos          |
| RF-021 | Comparar período atual com meses anteriores             | **Must**   | Sistema exibe diferença absoluta e/ou percentual conforme regra definida           |
| RF-022 | Calcular economia do período                            | **Must**   | Economia é calculada de forma consistente com a regra de negócio definida          |
| RF-023 | Exibir análise financeira baseada nos dados registrados | **Should** | Sistema apresenta indicadores derivados dos cálculos, sem IA                       |
| RF-024 | Exibir gráficos básicos                                 | **Could**  | Pelo menos os gráficos priorizados estão disponíveis sem comprometer a data do MVP |

## 7.5 Recursos Explicitamente Fora do MVP

| ID     | Descrição                            | Prioridade | Critério de Aceite                                |
| ------ | ------------------------------------ | ---------- | ------------------------------------------------- |
| RF-025 | Autenticação 2FA                     | **Won't**  | Não implementado no MVP; registrado no roadmap    |
| RF-026 | Chatbot com IA                       | **Won't**  | Não implementado no MVP; registrado no roadmap    |
| RF-027 | Análise financeira generativa via IA | **Won't**  | Não implementada no MVP; registrada no roadmap    |
| RF-028 | Integração bancária/Open Finance     | **Won't**  | Não implementada no MVP                           |
| RF-029 | Movimentação de dinheiro real        | **Won't**  | Não implementada em nenhuma funcionalidade do MVP |

---

# 8. Requisitos Não Funcionais

> Metas quantitativas abaixo são **suposições iniciais** e deverão ser recalibradas após implementação e testes.

| ID      | Categoria      | Descrição                                                                                     | Métrica                                                            |
| ------- | -------------- | --------------------------------------------------------------------------------------------- | ------------------------------------------------------------------ |
| RNF-001 | Segurança      | Senhas devem ser armazenadas usando algoritmo de hash apropriado, nunca em texto puro         | 100% das senhas persistidas com hash                               |
| RNF-002 | Segurança      | Dados de autenticação e recuperação devem utilizar tokens seguros e expiração                 | 100% dos fluxos de recuperação com token controlado                |
| RNF-003 | Segurança      | Aplicar validação de entrada no frontend e backend                                            | 100% dos endpoints críticos com validação no backend               |
| RNF-004 | Segurança      | Proteger sessões e endpoints autenticados contra acesso indevido                              | 0 acessos não autenticados permitidos a dados privados em testes   |
| RNF-005 | Segurança      | Aplicar controles alinhados às principais práticas do OWASP Top 10                            | Checklist de segurança concluído antes do lançamento               |
| RNF-006 | Segurança      | Dados trafegados entre cliente e servidor devem usar HTTPS em produção                        | 100% do tráfego produtivo via HTTPS                                |
| RNF-007 | Performance    | Operações comuns devem apresentar resposta adequada para uso web normal                       | **Suposição:** p95 ≤ 2s para operações padrão                      |
| RNF-008 | Performance    | Consultas do dashboard mensal devem evitar processamento desnecessário                        | **Suposição:** p95 ≤ 2s no carregamento do resumo                  |
| RNF-009 | Usabilidade    | O fluxo principal deve ser realizável sem treinamento externo                                 | Teste de usabilidade concluído com fluxo principal executável      |
| RNF-010 | Usabilidade    | Mensagens de erro devem indicar ação corretiva                                                | 100% dos fluxos críticos possuem feedback compreensível            |
| RNF-011 | Escalabilidade | Estrutura de dados deve separar usuários, categorias e registros financeiros                  | Modelo suporta crescimento sem duplicação estrutural desnecessária |
| RNF-012 | Escalabilidade | Agregações históricas não devem depender de lógica exclusiva do frontend                      | Cálculos críticos executados de forma consistente no backend       |
| RNF-013 | Confiabilidade | Operações financeiras devem ser transacionais quando houver múltiplas alterações relacionadas | Testes de falha não deixam estado parcialmente atualizado          |
| RNF-014 | Confiabilidade | Erros inesperados devem ser registrados para diagnóstico                                      | Logs disponíveis para falhas de aplicação em produção              |
| RNF-015 | Confiabilidade | Dados históricos não devem ser alterados por simples troca de período visualizado             | Teste de regressão confirma preservação histórica                  |

## Privacidade e LGPD

Embora o produto não movimente dinheiro real, o sistema armazenará dados pessoais e informações financeiras fornecidas pelo usuário.

**Decisão de produto:** tratar privacidade e proteção de dados como requisito de engenharia desde o MVP.

**Ponto de validação:** requisitos jurídicos específicos, política de privacidade, base legal, retenção e procedimentos de exclusão devem ser validados antes do lançamento público.

---

# 9. Regras de Negócio

## RN-001 — Distribuição da renda

A distribuição deve ser calculada aplicando percentuais configurados pelo usuário sobre uma renda de referência.

**Fórmula:**

`valor da categoria = renda de referência × percentual da categoria`

## RN-002 — Soma dos percentuais

A soma dos percentuais deverá obedecer à regra definida pelo produto.

**Estado atual:** [Informação pendente].

Recomendação de produto para refinamento: adotar soma total de **100%** para evitar distribuição de valores acima ou abaixo da renda de referência.

## RN-003 — Metodologia 50/20/30

O sistema disponibilizará uma configuração baseada na metodologia 50/20/30.

**Informação pendente:** definir como os três blocos da metodologia serão relacionados às quatro categorias do CashControl:

* despesas;
* economia;
* lazer;
* investimentos.

A implementação não deve assumir essa correspondência sem decisão explícita.

## RN-004 — Personalização

O usuário poderá alterar os percentuais da distribuição para refletir sua realidade financeira.

A alteração do planejamento não deve, por si só, apagar registros históricos.

## RN-005 — Registro financeiro

Todo registro financeiro deverá estar associado, no mínimo, a:

* usuário;
* valor;
* data;
* categoria/tipo;
* identificação do período financeiro.

**Campos adicionais:** [Informação pendente].

## RN-006 — Histórico

Os dados de meses anteriores devem permanecer consultáveis mesmo após alteração da configuração atual.

Mudanças futuras no planejamento não devem reescrever automaticamente o planejamento histórico.

## RN-007 — Comparação histórica

A comparação deverá utilizar períodos equivalentes.

Exemplo:

`Setembro/2026 vs Agosto/2026`

ou

`Setembro/2026 vs Setembro/2025`

conforme período selecionado.

## RN-008 — Diferença absoluta

`diferença = valor atual - valor comparado`

## RN-009 — Diferença percentual

Quando o valor comparado for diferente de zero:

`variação % = ((valor atual - valor comparado) / valor comparado) × 100`

Quando o valor comparado for zero, o sistema deverá aplicar uma regra específica para evitar divisão por zero.

**Regra específica:** [Informação pendente].

## RN-010 — Economia

A definição de economia deverá ser explicitamente escolhida antes da implementação.

Possíveis abordagens:

`economia = renda - despesas totais`

ou

`economia = valor explicitamente reservado para economia`

ou combinação de ambas.

**Decisão necessária:** [Informação pendente].

## RN-011 — Categorização

Cada lançamento deverá pertencer a uma categoria ou tipo permitido.

O sistema não deverá permitir registros sem classificação quando a classificação for necessária para os cálculos.

## RN-012 — Dados inseridos incorretamente

O sistema deve validar valores, datas e campos obrigatórios, mas não será responsável por determinar se um valor financeiro informado manualmente pelo usuário é verdadeiro.

---

# 10. Fluxos Principais — User Journeys

## Fluxo 1 — Onboarding

**Objetivo:** levar um novo usuário até seu primeiro planejamento.

1. Usuário acessa o CashControl.
2. Seleciona cadastro.
3. Informa dados necessários.
4. Conta é criada.
5. Usuário acessa o sistema.
6. Sistema apresenta orientação inicial.
7. Usuário é direcionado para cadastro de renda.

**Resultado esperado:** usuário autenticado e pronto para iniciar o planejamento.

---

## Fluxo 2 — Cadastro de renda

1. Usuário acessa a área de renda.
2. Informa o valor recebido.
3. Informa o período/data necessários.
4. Sistema valida os dados.
5. Sistema salva a renda.
6. Sistema disponibiliza a distribuição planejada.

**Resultado esperado:** renda disponível para cálculo do planejamento.

---

## Fluxo 3 — Distribuição

1. Sistema apresenta a configuração de distribuição.
2. Usuário seleciona a referência 50/20/30 ou configuração personalizada.
3. Usuário ajusta categorias e percentuais, quando aplicável.
4. Sistema recalcula valores.
5. Sistema apresenta quanto corresponde a cada categoria.
6. Usuário confirma o planejamento.

**Resultado esperado:** orçamento planejado para o período.

---

## Fluxo 4 — Registro financeiro

1. Usuário seleciona tipo/categoria.
2. Informa valor.
3. Informa data.
4. Adiciona descrição, quando disponível.
5. Salva o registro.
6. Sistema atualiza os indicadores do período.

**Resultado esperado:** transação incorporada ao resumo mensal.

---

## Fluxo 5 — Análise mensal

1. Usuário acessa o dashboard.
2. Sistema apresenta renda do período.
3. Sistema apresenta planejamento.
4. Sistema apresenta gastos e demais registros.
5. Sistema calcula economia.
6. Sistema apresenta histórico.
7. Usuário seleciona outro período para comparação.

**Resultado esperado:** usuário consegue entender sua posição financeira no período sem precisar calcular manualmente.

---

## Fluxo 6 — Recuperação de acesso

1. Usuário informa que esqueceu a senha.
2. Informa o e-mail cadastrado.
3. Sistema envia instrução de recuperação.
4. Usuário acessa link/token.
5. Define nova senha.
6. Sistema invalida o token utilizado.
7. Usuário realiza novo login.

---

# 11. Métricas de Sucesso

## 11.1 KPIs de Produto

| KPI                             | Definição                                                 | Como medir                  |
| ------------------------------- | --------------------------------------------------------- | --------------------------- |
| Usuários ativos mensais         | Usuários que utilizam o produto no mês                    | Eventos de autenticação/uso |
| Taxa de conclusão do onboarding | Usuários que completam cadastro → renda → planejamento    | Funil                       |
| Taxa de registro financeiro     | Usuários que registram pelo menos uma movimentação no mês | Eventos de registro         |
| Meses financeiros completos     | Meses que cumprem critérios de consolidação               | Banco de dados              |
| Retenção mensal                 | Usuários que retornam em meses subsequentes               | Identificador de usuário    |
| Uso de comparação               | Usuários que consultam histórico/comparações              | Eventos de navegação        |

## 11.2 KPIs de Negócio

| KPI                   | Definição                                                    | Como medir           |
| --------------------- | ------------------------------------------------------------ | -------------------- |
| Economia mensal       | Valor reservado/economizado no período conforme regra RN-010 | Dados financeiros    |
| Evolução da economia  | Diferença entre economia de períodos                         | Comparação histórica |
| Despesas mensais      | Total de despesas por período                                | Dados financeiros    |
| Variação das despesas | Evolução dos gastos entre períodos                           | Comparação histórica |
| Lazer mensal          | Total destinado a lazer                                      | Dados financeiros    |
| Investimentos mensais | Total registrado como investimento                           | Dados financeiros    |

## 11.3 Indicadores de Qualidade

| Métrica                            | Objetivo                 |
| ---------------------------------- | ------------------------ |
| Erros de cálculo reportados        | Minimizar                |
| Falhas de recuperação de conta     | Minimizar                |
| Taxa de abandono do cadastro       | Identificar gargalos     |
| Tempo de carregamento do dashboard | Manter dentro do RNF-007 |
| Erros de aplicação                 | Monitorar estabilidade   |

> **Importante:** redução de despesas ou aumento de economia são métricas de resultado observáveis, mas não devem ser atribuídos exclusivamente ao CashControl sem uma estratégia de validação causal.

---

# 12. Riscos e Mitigações

| Risco                                                 | Probabilidade | Impacto     | Mitigação                                                                       | Responsável |
| ----------------------------------------------------- | ------------- | ----------- | ------------------------------------------------------------------------------- | ----------- |
| Erros nos cálculos de distribuição                    | Média         | Alto        | Testes unitários, casos-limite e validação manual                               | Yuri        |
| Erros na comparação histórica                         | Média         | Alto        | Regras explícitas, testes com períodos zero/negativo e regressão                | Yuri        |
| Falhas de autenticação/recuperação                    | Média         | Alto        | Tokens seguros, expiração, rate limiting e testes de fluxo                      | Yuri        |
| Crescimento do escopo                                 | Alta          | Alto        | MoSCoW, backlog separado e congelamento do MVP próximo ao desenvolvimento final | Yuri        |
| Complexidade de categorias ilimitadas                 | Média         | Médio       | Definir limites/regras para criação, edição e exclusão                          | Yuri        |
| Dados financeiros incorretos inseridos pelo usuário   | Alta          | Médio       | Validação de campos, confirmação e edição de lançamentos                        | Yuri        |
| Usabilidade inadequada                                | Média         | Alto        | Testes com usuários e priorização do fluxo principal                            | Yuri        |
| Dependência de serviço de e-mail                      | Média         | Médio       | Escolher fornecedor com documentação e fallback operacional                     | Yuri        |
| Vazamento ou exposição de dados financeiros           | Baixa/Média   | Alto        | Controles de acesso, HTTPS, hash de senha, validação de entrada e logs          | Yuri        |
| Sobrecarga por desenvolvimento individual             | Alta          | Alto        | Limite de WIP, priorização rígida e adiamento explícito de Could items          | Yuri        |
| Gráficos comprometerem o prazo                        | Média         | Baixo/Médio | Tratar gráficos como Could e implementar somente após o núcleo funcional        | Yuri        |
| Requisito de distribuição 50/20/30 permanecer ambíguo | Alta          | Alto        | Resolver mapeamento antes da implementação das regras de cálculo                | Yuri        |

---

# 13. Dependências

## 13.1 Técnicas

| Dependência                    | Necessidade                      | Prioridade |
| ------------------------------ | -------------------------------- | ---------- |
| Banco de dados                 | Usuários e registros financeiros | Must       |
| Backend                        | Autenticação, regras e cálculos  | Must       |
| Frontend web                   | Interface do produto             | Must       |
| Serviço de autenticação        | Cadastro, login e sessão         | Must       |
| Serviço de e-mail transacional | Recuperação de acesso            | Must       |
| Hospedagem                     | Publicação da aplicação          | Must       |
| Biblioteca de gráficos         | Visualizações                    | Could      |
| Serviço de IA                  | Recursos de IA                   | Futuro     |

## 13.2 Dependências de Produto

* Definição do modelo de distribuição.
* Definição de economia.
* Definição do fechamento/consolidação mensal.
* Definição de comportamento de categorias.
* Definição dos campos obrigatórios de cada registro.
* Definição dos períodos de comparação.

## 13.3 Dependências Externas

* Provedor de e-mail transacional.
* Provedor de hospedagem.
* Banco de dados hospedado, caso separado da infraestrutura principal.
* Eventuais serviços de monitoramento/logs.

**Open Finance, APIs bancárias e provedores de IA não são dependências do MVP.**

---

# 14. Premissas

1. O produto é exclusivamente de planejamento e controle financeiro.
2. Nenhum valor será movimentado pelo CashControl.
3. Não haverá integração bancária no MVP.
4. O usuário será a fonte dos dados financeiros.
5. Renda poderá ser registrada manualmente.
6. O planejamento será calculado sobre uma renda de referência.
7. Percentuais de distribuição poderão ser personalizados.
8. O histórico será preservado mesmo após alterações futuras.
9. Os cálculos serão determinísticos no MVP.
10. IA e 2FA serão tratados como roadmap.
11. O lançamento é previsto para 19/01/2027.
12. Yuri é responsável por produto, design, desenvolvimento e testes.
13. Gráficos são opcionais e dependem da capacidade disponível no prazo.

---

# 15. Roadmap de Alto Nível

| Fase               | Escopo                                                                                                                             | Objetivo                                                                        |
| ------------------ | ---------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------- |
| **MVP — Jan/2027** | Cadastro, login, recuperação, renda, distribuição, categorias, registros, histórico, comparação, economia e análise determinística | Validar o núcleo do produto                                                     |
| **v1.1**           | [A definir]                                                                                                                        | Corrigir problemas do MVP, melhorar UX e adicionar melhorias de maior evidência |
| **v2.0**           | IA, 2FA, integrações bancárias/Open Finance                                                                                        | Expandir automação, segurança e aquisição automática de dados                   |
| Futuro             | Mobile e automatizações avançadas                                                                                                  | Expandir canais e automação                                                     |

## Priorização sugerida para pós-MVP

A ordem abaixo não representa julgamento de valor final; é uma proposta de backlog para refinamento:

**v1.1:** estabilização → UX → métricas → melhorias de usabilidade.

**v2.0:** 2FA → IA → integrações bancárias, sujeitas à definição técnica, jurídica e de produto.

---

# 16. Perguntas em Aberto

As questões abaixo impedem ou podem impactar significativamente a implementação.

### P0 — Bloqueadoras

1. **Como exatamente a metodologia 50/20/30 será mapeada para as quatro categorias do CashControl?**
2. **Como a renda será tratada quando houver múltiplas entradas no mesmo mês?**
3. **O que exatamente significa “economia” no produto: renda menos despesas, valor reservado pelo usuário, ou uma combinação?**
4. **Como será definido o fechamento de um mês e quais dados pertencem a cada período?**

### P1 — Importantes

5. **Quais regras de edição/exclusão devem ser aplicadas a categorias e registros que já possuem histórico?**
6. **Quais campos serão obrigatórios em cada registro financeiro?**
7. **Qual comportamento o sistema terá para renda variável, renda fracionada e múltiplas fontes de renda?**
8. **Qual será a experiência mínima de onboarding para levar o usuário ao primeiro planejamento sem etapas desnecessárias?**

### P2 — Engenharia

9. **Qual stack será utilizada no frontend, backend, banco de dados e hospedagem?**
10. **Qual estratégia mínima de testes será adotada antes do lançamento: unitário, integração, E2E ou combinação?**

### P3 — Pós-MVP

11. **Qual critério determinará a entrada de 2FA, IA e integração bancária no roadmap pós-MVP?**

---

# 17. Histórico de Versões

| Versão | Data       | Autor | Mudanças                                                                                                                             |
| ------ | ---------- | ----- | ------------------------------------------------------------------------------------------------------------------------------------ |
| v1.0   | 21/09/2026 | Yuri  | Primeira consolidação do PRD Executivo; definição de escopo, requisitos, regras de negócio, métricas, riscos, dependências e roadmap |

---

# 18. Perguntas para Refinamento do Prompt

As respostas abaixo devem ser usadas na próxima versão do PRD e também para tornar este prompt mais preciso para futuras iterações.

## 1 — Regra de distribuição — P0

**Qual é a distribuição exata desejada para as quatro categorias?**

Escolha ou descreva sua própria regra:

* Despesas = 50%, Lazer = 30%, Economia = 20%, Investimentos = separado
* Despesas = 50%, Economia = 20%, Lazer = 20%, Investimentos = 10%
* Outra distribuição
* 50/20/30 deve existir apenas como template inicial e o usuário define as quatro categorias
* Outra lógica

**Essa resposta define diretamente RN-003, RF-008 a RF-011 e o cálculo central do produto.**

---

## 2 — Renda e entradas fracionadas — P0

**Como o CashControl deve tratar renda?**

* Uma única renda mensal
* Várias entradas no mesmo mês
* Múltiplas fontes de renda
* Renda variável mês a mês
* Combinação das anteriores

E: o planejamento deve ser recalculado automaticamente quando uma nova entrada for adicionada?

---

## 3 — Economia e consolidação — P0

**Qual fórmula representa “economia” para você?**

* `Renda - despesas`
* Valor explicitamente reservado para economia
* `Renda - todas as saídas`
* Economia planejada vs. economia realizada
* Outra

Depois disso, precisamos definir: **um mês pode ser considerado concluído mesmo sem todos os campos registrados?**

---

## 4 — Segurança e privacidade — P1

**Qual nível de segurança você deseja no MVP?**

Por exemplo:

* senha + sessão + recuperação por e-mail;
* senha + recuperação + rate limiting;
* incluir confirmação de e-mail;
* incluir política de expiração de sessão;
* outros requisitos.

**2FA permanece fora do MVP independentemente dessa escolha?**

---

## 5 — Escopo real do MVP — P1

**Quais funcionalidades são obrigatórias para a entrega de 19/01/2027?**

Classifique cada item como **Must / Should / Could / Won't**:

* gráficos;
* categorias personalizadas;
* múltiplas rendas;
* investimentos;
* lazer;
* comparação histórica;
* análise financeira;
* edição/exclusão de histórico.

Essa resposta será usada para congelar o backlog do MVP.

---

## 6 — UX e fluxo principal — P1

**Qual experiência você quer priorizar no primeiro uso?**

* Usuário termina o onboarding com um plano mensal pronto;
* Usuário primeiro cadastra renda e depois decide a distribuição;
* Dashboard já aparece vazio e orienta o preenchimento;
* Outro fluxo.

**Quantos passos máximos você considera aceitáveis para cadastrar a primeira renda?**

---

## 7 — Modelo de dados — P1

**Como você imagina as principais entidades?**

Uma primeira proposta é:

`User → Income → Budget/Distribution → Category → Transaction → MonthlySummary`

Você deseja essa estrutura, uma estrutura mais simples ou outra modelagem?

---

## 8 — Stack e deploy — P1

**Qual stack pretende utilizar?**

Informe, mesmo que provisoriamente:

* Frontend;
* Backend;
* Banco de dados;
* Autenticação;
* Hospedagem;
* Serviço de e-mail.

Essa resposta permitirá converter os RNFs em requisitos técnicos mais concretos.

---

## 9 — Testes e validação — P2

**Qual nível de testes você pretende entregar no MVP?**

* Unitários;
* Integração;
* E2E;
* Testes manuais;
* Todos os anteriores em níveis diferentes.

**Quais partes você considera obrigatórias para cobertura automatizada?**

Recomendação inicial de priorização técnica: cálculos financeiros, autenticação e regras de histórico.

---

## 10 — Roadmap e formato da documentação — P2

**Após o MVP, qual recurso você pretende explorar primeiro: 2FA, IA ou integração bancária?**

E qual formato de documentação você deseja manter?

* PRD executivo;
* PRD + especificação técnica;
* PRD + documentação de API;
* PRD + documentação técnica completa;
* documentação resumida para manutenção.

---

# Decisão de Refinamento v1.0

A principal decisão pendente antes do início da implementação é a definição das **regras matemáticas do produto**, especialmente:

`renda → distribuição → registros → economia → consolidação → comparação`

Enquanto essas regras não estiverem fechadas, a implementação da interface pode avançar, mas o núcleo de cálculo não deve ser considerado definitivo.

**Próximo marco recomendado:** congelar as regras RN-001 a RN-012 e, em seguida, transformar RF-001 a RF-024 em backlog técnico com tarefas de frontend, backend, banco e testes.
