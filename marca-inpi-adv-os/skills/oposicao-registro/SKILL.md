---
name: oposicao-registro
description: Redige oposição administrativa a pedido de registro de marca de terceiro, com fundamento no art. 158 da LPI. Use quando o operador disser "quero opor uma marca", "apareceu uma marca igual à minha na RPI", "oposição ao INPI", "impedir registro de terceiro", "marca de concorrente foi publicada", "oposição a pedido de marca", ou descrever que o cliente é titular/depositante anterior e quer impugnar pedido de marca conflitante publicado para oposição. Cobre os fundamentos do art. 124 (XIX colidência, V nome empresarial, VI descritivo, XXIII má-fé), art. 125 (alto renome) e art. 126/6º bis CUP (notoriamente conhecida). GRU 332 (oposição) ou 3022 (oposição restrita art. 124 XIX). Prazo de 60 dias da publicação.
---

# OPOSIÇÃO A PEDIDO DE REGISTRO (art. 158 LPI)

> Camada 3 — Contencioso administrativo INPI. Acionada pelo `marcas-master` quando o cliente é titular/depositante anterior e quer impedir o registro de marca de terceiro publicada para oposição.

## Anexos obrigatórios (context/)
- `context/lpi-marcas-titulo-iii.md` — art. 158 (oposição, prazo 60 dias); art. 124 (incs. V, VI, XIX, XXIII); art. 125 (alto renome); art. 126 (notoriamente conhecida); art. 158 § 2º (prova do depósito em 60 dias se fundada em 124 XXIII ou 126).
- `context/custos-gru-inpi.md` — GRU 332 (oposição R$ 520 por classe) · GRU 3022 (oposição restrita art. 124 XIX R$ 360).
- `context/jurisprudencia-marcaria.md` — colidência, afinidade de produtos/serviços, teoria da distância, sob demanda.
- `context/ncl-13-2026-classes.md` — para aferir afinidade/identidade de classe entre a marca oposta e a anterioridade do cliente.

## Objetivo
Produzir oposição tempestiva, fundamentada e com prova suficiente, que impeça o deferimento de pedido de marca de terceiro conflitante com direito anterior do cliente.

## Quando ativar
- Cliente é titular de registro/pedido anterior e identificou marca de terceiro publicada para oposição na RPI.
- Há colidência (art. 124 XIX), uso indevido de nome empresarial/título (art. 124 V), apropriação de termo descritivo do cliente, má-fé (art. 124 XXIII) ou ofensa a alto renome/notoriedade (arts. 125, 126).
- O prazo de 60 dias da publicação ainda está aberto.

## Metodologia
1. **Estado do caso** via `memoria-de-caso-marca`: marca anterior do cliente (nº processo/registro, classe, data), marca oposta (nº pedido, classe, depositante, data da publicação na RPI).
2. **Tempestividade:** confirmar que está dentro dos **60 dias** da publicação para oposição (art. 158). Fora do prazo → não cabe oposição; avaliar PAN (`nulidade-administrativa-pan`) se já registrado.
3. **Fundamento:** escolher o(s) inciso(s) aplicável(is) — XIX (reprodução/imitação de marca registrada, mesmo ramo/afim), V (nome empresarial/título), VI (sinal genérico/descritivo apropriado indevidamente), XXIII (má-fé), e/ou arts. 125/126. Conferir cada dispositivo em `context/`.
4. **Análise de colidência:** comparar sinais (gráfico, fonético, ideológico) e afinidade de produtos/serviços (mesma classe ou afins — usar `context/ncl-13-2026-classes.md`); aplicar teoria da distância e princípio da especialidade.
5. **Prova-condição (art. 158 § 2º):** se a oposição se fundar no art. 124 XXIII ou no art. 126, **comprovar o depósito do pedido de registro da marca no Brasil em até 60 dias após a interposição**, sob pena de não conhecimento.
6. **Custas:** indicar **GRU 332** (oposição) por classe; **GRU 3022** se restrita ao art. 124 XIX. Uma GRU por classe (`metodologia-marcaria.md`).
7. **Validação:** todo dispositivo/jurisprudência citado passa por `validador-marcario`.
8. Atualizar `memoria-de-caso-marca` (oposição protocolada, prazo da manifestação do depositante — art. 158 § 1º).

## Entrega obrigatória final
- Peça de oposição redigida (qualificação, tempestividade, direito anterior, fundamentos por inciso, análise de colidência, prova-condição se 124 XXIII/126, pedido de não concessão).
- GRU indicada (332 ou 3022) por classe.
- Alerta de prova-condição do art. 158 § 2º quando aplicável.
- `memoria-de-caso-marca` atualizado + próximo passo (aguardar manifestação do depositante).
- **Validação pela `suprema-corte-marcaria` (R1–R4) antes da entrega.**

## Guard
Nenhum dispositivo/súmula/acórdão entra na peça sem `validador-marcario`. Custas por classe. Confere prazo de 60 dias da publicação (art. 158) e a prova-condição do § 2º. Entrega só após `suprema-corte-marcaria`. Na dúvida sobre vigência/valor de GRU/existência de precedente, bloquear e checar ao vivo.
