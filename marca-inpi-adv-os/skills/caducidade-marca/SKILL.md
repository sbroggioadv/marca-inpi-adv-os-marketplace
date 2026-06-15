---
name: caducidade-marca
description: Conduz o pedido de caducidade de registro de marca por desuso, com fundamento nos arts. 143 a 146 da LPI — tanto para requerer a caducidade (cliente com legítimo interesse) quanto para defender o registro provando o uso (cliente titular intimado). Use quando o operador disser "caducidade de marca", "marca não está sendo usada", "quero derrubar uma marca por desuso", "pedido de caducidade", "fui intimado para provar uso da minha marca", "defender caducidade", "registro caduco", ou descrever marca registrada há mais de 5 anos sem uso comprovado no Brasil. O ônus de provar o uso é do TITULAR (art. 143 § 2º). Prazo do titular intimado — 60 dias. GRU 337 (caducidade). Cabe caducidade total ou parcial (art. 144).
---

# CADUCIDADE POR DESUSO (arts. 143-146 LPI)

> Camada 3 — Contencioso administrativo INPI. Acionada pelo `marcas-master` para extinguir (ou defender) registro de marca por desuso.

## Anexos obrigatórios (context/)
- `context/lpi-marcas-titulo-iii.md` — art. 142 III (caducidade como causa de extinção); art. 143 (requerimento por legítimo interesse, decorridos 5 anos da concessão; § 1º justificativa de desuso por razões legítimas; **§ 2º ônus do uso é do titular, intimado em 60 dias**); art. 144 (caducidade parcial); art. 145 (não conhecimento se uso comprovado em processo anterior < 5 anos); art. 146 (recurso).
- `context/jurisprudencia-marcaria.md` — **prova e ônus do uso** (uso efetivo × simbólico, caducidade parcial, justificativas legítimas) — anexo central nesta skill.
- `context/custos-gru-inpi.md` — GRU 337 (caducidade; confirmar valor na emissão).

## Objetivo
- **Atacante:** requerer a caducidade de registro que não vem sendo usado no Brasil, abrindo espaço para a marca do cliente.
- **Defensor:** comprovar o uso efetivo (ou justificar o desuso por razões legítimas) e preservar o registro do cliente.

## Quando ativar
- Marca de terceiro está registrada há mais de 5 anos e não há uso efetivo no Brasil — o cliente tem legítimo interesse em derrubá-la.
- O cliente é titular e foi **intimado** para comprovar o uso (art. 143 § 2º).

## Metodologia
1. **Estado do caso** via `memoria-de-caso-marca`: registro alvo (nº, classe, titular, data da concessão), legítimo interesse do cliente; ou, na defesa, data da intimação e elementos de uso disponíveis.
2. **Requisito temporal (atacante):** o requerimento só cabe se, **decorridos 5 anos da concessão**, na data do requerimento, o uso não foi iniciado ou foi interrompido por mais de 5 anos consecutivos (art. 143 I/II). Verificar também o art. 145 (não conhecimento se houve comprovação de uso em processo anterior < 5 anos).
3. **Ônus do uso — regra de ouro (art. 143 § 2º):** o **titular** é quem tem o ônus de provar o uso ou justificar o desuso, intimado em **60 dias**. O atacante demonstra apenas o legítimo interesse e a aparência de desuso.
4. **Defesa (titular):** reunir prova de **uso efetivo** no Brasil (notas fiscais, embalagens, publicidade, presença comercial), ou justificar o desuso por razões legítimas (art. 143 § 1º). Atenção à caducidade **parcial** (art. 144): o uso de parte dos produtos/serviços não salva o registro quanto aos demais não afins.
5. **Custas:** indicar **GRU 337** (no requerimento de caducidade).
6. **Validação:** todo dispositivo/jurisprudência (especialmente sobre prova do uso) passa por `validador-marcario`, cruzando com `jurisprudencia-marcaria.md`.
7. Atualizar `memoria-de-caso-marca` (caducidade requerida/respondida; próximo passo: decisão; recurso cabível art. 146).

## Entrega obrigatória final
- Peça de requerimento de caducidade **ou** de comprovação de uso/justificativa de desuso (qualificação, legítimo interesse, requisito temporal, ônus do titular, prova/justificativa, pedido).
- GRU 337 indicada (no requerimento).
- Análise de caducidade total × parcial (art. 144) quando o uso for de apenas parte dos produtos/serviços.
- `memoria-de-caso-marca` atualizado + próximo passo (decisão; recurso art. 146).
- **Validação pela `suprema-corte-marcaria` (R1–R4) antes da entrega.**

## Guard
Nenhum dispositivo/súmula/acórdão entra na peça sem `validador-marcario`. **O ônus do uso é do titular (art. 143 § 2º)** — não inverter. Conferir o requisito dos 5 anos (art. 143) e o art. 145. Entrega só após `suprema-corte-marcaria`. Na dúvida sobre vigência/valor de GRU/existência de precedente, bloquear e checar ao vivo.
