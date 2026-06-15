---
name: cumprimento-exigencia
description: Responde a exigência formulada pelo examinador do INPI durante o exame do pedido de marca — exigência formal (art. 157, prazo de 5 dias) ou exigência de mérito durante o exame (art. 159, prazo de 60 dias). Use quando o operador disser "recebi uma exigência do INPI", "o examinador pediu correção", "exigência de mérito na minha marca", "cumprir exigência", "responder exigência do e-Marcas", "o INPI exigiu especificação", "exigência formal de marca", ou descrever que o pedido foi sobrestado aguardando providência do depositante. Cobre correção de especificação NCL, etiqueta/imagem, qualificação, procuração, e resposta argumentativa a exigência de exame. GRU 338 (cumprimento de exigência de exame formal). Risco de arquivamento se não respondida (art. 159 § 1º).
---

# CUMPRIMENTO DE EXIGÊNCIA (arts. 157 e 159 LPI)

> Camada 3 — Contencioso administrativo INPI. Acionada pelo `marcas-master` quando o INPI formula exigência e o pedido fica sobrestado aguardando a providência do depositante.

## Anexos obrigatórios (context/)
- `context/lpi-marcas-titulo-iii.md` — art. 157 (exigência no exame formal preliminar, prazo 5 dias, sob pena de inexistência); art. 159 (exigências no exame, prazo 60 dias; § 1º arquivamento definitivo se não respondida; § 2º prosseguimento se respondida ou contestada).
- `context/procedimento-emarcas.md` — passo a passo do peticionamento no e-Marcas e emissão de GRU de cumprimento de exigência.
- `context/ncl-13-2026-classes.md` — para reespecificar produtos/serviços conforme a NCL quando a exigência for de especificação.
- `context/custos-gru-inpi.md` — GRU 338 (cumprimento de exigência de exame formal; confirmar valor na emissão).

## Objetivo
Sanear o pedido dentro do prazo, cumprindo a exigência (correção) ou contestando-a tecnicamente, evitando o arquivamento e levando o processo ao prosseguimento do exame.

## Quando ativar
- O INPI publicou exigência (formal — art. 157, ou de exame — art. 159) e o pedido aguarda resposta.
- Há necessidade de corrigir especificação NCL, etiqueta/imagem, qualificação, procuração, ou de rebater entendimento do examinador.

## Metodologia
1. **Estado do caso** via `memoria-de-caso-marca`: pedido (nº, classe, sinal), texto da exigência, base legal invocada pelo examinador, data da publicação.
2. **Identificar o tipo e o prazo:**
   - **Formal (art. 157):** prazo de **5 dias**, sob pena de o pedido ser considerado **inexistente**.
   - **De exame (art. 159):** prazo de **60 dias**; não respondida → **arquivamento definitivo** (§ 1º); respondida ou contestada → prosseguimento (§ 2º).
3. **Diagnosticar o objeto:** especificação de produtos/serviços (reespecificar pela NCL — `ncl-13-2026-classes.md`), etiqueta/imagem, qualificação do depositante, procuração/representação, ou questão de mérito (distintividade, colidência apontada de ofício).
4. **Estratégia de resposta:** cumprir (corrigir o que for procedente) e/ou contestar (sustentar a regularidade do pedido com fundamento legal). Lembrar que, mesmo "não cumprida", se contestada, o exame prossegue (art. 159 § 2º).
5. **Operacional:** orientar o peticionamento no e-Marcas e a **GRU 338** quando aplicável, conforme `procedimento-emarcas.md`.
6. **Validação:** todo dispositivo/jurisprudência passa por `validador-marcario`.
7. Atualizar `memoria-de-caso-marca` (exigência respondida; próximo passo: prosseguimento do exame / decisão).

## Entrega obrigatória final
- Peça/petição de cumprimento ou de contestação da exigência (identificação do pedido, transcrição da exigência, resposta item a item, especificação corrigida se for o caso, fundamento legal).
- Tipo e prazo da exigência destacados (5 dias formal × 60 dias exame) + alerta de arquivamento/inexistência.
- GRU 338 indicada quando aplicável + nota do peticionamento e-Marcas.
- `memoria-de-caso-marca` atualizado + próximo passo.
- **Validação pela `suprema-corte-marcaria` (R1–R4) antes da entrega.**

## Guard
Nenhum dispositivo/súmula/acórdão entra na peça sem `validador-marcario`. Conferir o prazo correto (5 dias art. 157 × 60 dias art. 159) — confundir é fatal. Especificação só pela NCL vigente. Entrega só após `suprema-corte-marcaria`. Na dúvida sobre vigência/valor de GRU, bloquear e checar ao vivo.
