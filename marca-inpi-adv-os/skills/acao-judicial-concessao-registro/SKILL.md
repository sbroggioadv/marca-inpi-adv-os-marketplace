---
name: acao-judicial-concessao-registro
description: Redige ação judicial na JUSTIÇA FEDERAL para anular o ato do INPI que indeferiu o registro e determinar novo exame/reanálise do pedido (controle judicial do ato administrativo — STJ REsp 1.787.676). NÃO se pede "registre já" nem prazo ao INPI — o Judiciário controla o indeferimento indevido, mas não impõe prazo nem substitui o INPI (TRF2 MS 5084794-88.2023.4.02.5101). Use quando o operador disser "fui indeferido no INPI e quero forçar o registro", "o INPI negou minha marca injustamente", "ação pra obter o registro", "anular o indeferimento", "judicializar o indeferimento", "esgotei o recurso administrativo e perdi", "o INPI indeferiu sem razão", ou descrever um indeferimento que persistiu após o recurso administrativo e o cliente quer revertê-lo no Judiciário. Cobre o controle judicial do ato administrativo do INPI, com o INPI no polo (competência federal).
---

# AÇÃO JUDICIAL CONTRA O INDEFERIMENTO DO INPI (anular + novo exame)

> Camada 4 — Contencioso judicial. **Justiça Federal — INPI no polo.** Acionada pelo `marcas-master` quando o indeferimento persistiu após o recurso administrativo (`recurso-indeferimento-inpi`) e o cliente quer revertê-lo judicialmente.

## Anexos obrigatórios (context/)
- `context/lpi-marcas-titulo-iii.md` — art. 160 (decisão de deferimento/indeferimento); arts. 124/125/126 (fundamento do indeferimento a ser combatido); art. 175 (foro federal, INPI no feito) por analogia de competência ao controle do ato do INPI.
- `context/jurisprudencia-marcaria.md` — TEMA 5 (forçar/reanalisar registro — REsp 1.787.676: o STJ anula o ato do INPI e determina reanálise; TRF2 MS 5084794-88.2023.4.02.5101: NÃO cabe impor prazo ao INPI, mas o controle do indeferimento indevido subsiste); TEMA 3 (alto renome só prospectivo), sob demanda.

## Objetivo
Produzir ação que **anule o ato administrativo de indeferimento** e **determine que o INPI reanalise/conclua o exame** do pedido — sem pedir registro automático nem fixação de prazo, dentro dos limites do controle judicial reconhecido pelo STJ e pelo TRF2.

## Quando ativar
- O pedido de registro foi **indeferido** e o **recurso administrativo** já foi esgotado (ou é inviável) — o ato do INPI persiste.
- O cliente entende que o indeferimento foi **indevido** (ex.: indeferimento por colidência/alto renome incabível, exame equivocado).
- **Não** confundir com nulidade de registro de terceiro (`acao-nulidade-registro`) — aqui se ataca o **ato denegatório do próprio pedido do cliente**.

## Metodologia
1. **Estado do caso** via `memoria-de-caso-marca`: nº do pedido, marca, classe, fundamento do indeferimento, decisão do recurso administrativo.
2. **Foro — Justiça Federal, INPI no polo.** Endereçar à vara federal; o INPI é réu (controle de ato da autarquia federal).
3. **Pedido CORRETO (regra de ouro):** **anular o ato de indeferimento + determinar novo exame/reanálise** do pedido (STJ REsp 1.787.676). **NÃO redigir** pedido de "conceder/registrar já" nem de "decidir em X dias" — o Judiciário **não impõe prazo** nem substitui o INPI (TRF2 MS 5084794-88.2023.4.02.5101). Conferir os dois precedentes em `context/jurisprudencia-marcaria.md`.
4. **Mérito:** demonstrar o vício do indeferimento (ex.: alto renome só tem efeito prospectivo — não atinge pedido depositado antes do reconhecimento; ausência de colidência real; erro no exame). Validar a tese com jurisprudência real.
5. **Limites do controle judicial:** o Judiciário controla preterição na fila, irregularidade em exigências, demora em recursos e **indeferimento indevido** — mas não fixa prazo por "razoabilidade abstrata" (TRF2).
6. **Valor da causa**, provas. **Validação** por `validador-marcario`.
7. Atualizar `memoria-de-caso-marca` (ação proposta, pedido de anulação + reanálise).

## Entrega obrigatória final
- Peça redigida (endereçada à **Justiça Federal**, **INPI no polo**), com pedido de **anulação do indeferimento + novo exame** (nunca "registre já", nunca prazo), mérito combatendo o vício e valor da causa.
- `memoria-de-caso-marca` atualizado + próximo passo + prazo.
- **Validação pela `suprema-corte-marcaria` (R1–R4) antes da entrega.**

## Guard
Nenhum dispositivo/súmula/acórdão entra na peça sem `validador-marcario`. **Pedido correto (R4): anular o ato + determinar novo exame — NUNCA "registre já" nem prazo ao INPI** (STJ REsp 1.787.676 / TRF2 MS 5084794-88.2023.4.02.5101). **Foro (R1): Justiça Federal, INPI no polo.** Entrega só após `suprema-corte-marcaria`. Na dúvida sobre vigência/existência de precedente, bloquear e checar ao vivo.
