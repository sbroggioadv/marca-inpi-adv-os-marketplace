---
name: manifestacao-oposicao
description: Redige a defesa do depositante quando o pedido de marca do cliente sofreu oposição de terceiro, com fundamento no art. 159 da LPI (manifestação à oposição). Use quando o operador disser "fui oposto no INPI", "minha marca recebeu oposição", "preciso responder a oposição", "manifestação à oposição", "defender meu pedido de marca", "terceiro opôs minha marca", ou descrever que o cliente é DEPOSITANTE e foi intimado da oposição apresentada por outrem. Rebate colidência, sustenta distintividade, convivência e diferença de ramo. Prazo de 60 dias da intimação (art. 158 § 1º). Sem GRU própria (a manifestação à oposição não tem retribuição de serviço autônoma).
---

# MANIFESTAÇÃO À OPOSIÇÃO (art. 159 LPI)

> Camada 3 — Contencioso administrativo INPI. Acionada pelo `marcas-master` quando o cliente é o **depositante** do pedido oposto e foi intimado para se defender da oposição de terceiro.

## Anexos obrigatórios (context/)
- `context/lpi-marcas-titulo-iii.md` — art. 158 § 1º (intimação do depositante, prazo 60 dias); art. 159 (exame após a manifestação); art. 124 (incs. para rebater a colidência); art. 158 § 2º (não conhecimento da oposição que não comprovar o depósito quando fundada em 124 XXIII / 126).
- `context/ncl-13-2026-classes.md` — para demonstrar diferença/afinidade de produtos e serviços entre os sinais.
- `context/jurisprudencia-marcaria.md` — convivência de marcas, princípio da especialidade, sob demanda.
- `context/custos-gru-inpi.md` — referência (a manifestação à oposição não exige GRU autônoma).

## Objetivo
Produzir defesa tempestiva e técnica que afaste a oposição e leve ao deferimento do pedido do cliente, demonstrando ausência de colidência, distintividade do sinal e/ou possibilidade de convivência.

## Quando ativar
- Cliente é depositante e foi intimado (art. 158 § 1º) da oposição de terceiro.
- Há tese de defesa: sinais distinguíveis, ramos diversos, especialidade, convivência pacífica, fragilidade do direito do opoente, ou falha na prova-condição do art. 158 § 2º.
- O prazo de 60 dias da intimação ainda está aberto.

## Metodologia
1. **Estado do caso** via `memoria-de-caso-marca`: pedido do cliente (nº, classe, sinal, data), oposição (opoente, fundamento alegado, marca anterior invocada), data da intimação.
2. **Tempestividade:** confirmar os **60 dias** da intimação (art. 158 § 1º).
3. **Mapear a oposição:** identificar exatamente os incisos do art. 124 (ou arts. 125/126) invocados pelo opoente — só se rebate o que foi alegado.
4. **Teses de defesa** (selecionar as cabíveis): inexistência de colidência (cotejo gráfico/fonético/ideológico); diferença de ramo/afinidade de produtos-serviços (`ncl-13-2026-classes.md`); suficiente forma distintiva; princípio da especialidade; convivência pacífica/coexistência; anterioridade ou uso do próprio cliente (art. 129 § 1º precedência, se houver); fragilidade do registro do opoente.
5. **Prova-condição do opoente:** se a oposição se funda em 124 XXIII ou 126, verificar se o opoente comprovou o depósito em 60 dias (art. 158 § 2º) — a falta enseja **não conhecimento** e deve ser arguida.
6. **Validação:** todo dispositivo/jurisprudência passa por `validador-marcario`.
7. Atualizar `memoria-de-caso-marca` (manifestação protocolada; próximo passo: exame pelo INPI, art. 159 — pode gerar exigência → `cumprimento-exigencia`).

## Entrega obrigatória final
- Peça de manifestação à oposição (qualificação, tempestividade, síntese da oposição, teses de defesa ponto a ponto, eventual não conhecimento por falha do § 2º, pedido de deferimento).
- Observação de que não há GRU autônoma para o ato.
- `memoria-de-caso-marca` atualizado + próximo passo (exame; possível exigência ou decisão).
- **Validação pela `suprema-corte-marcaria` (R1–R4) antes da entrega.**

## Guard
Nenhum dispositivo/súmula/acórdão entra na peça sem `validador-marcario`. Rebater apenas os fundamentos efetivamente arguidos pelo opoente. Conferir prazo de 60 dias (art. 158 § 1º). Entrega só após `suprema-corte-marcaria`. Na dúvida sobre vigência/existência, bloquear e checar ao vivo.
