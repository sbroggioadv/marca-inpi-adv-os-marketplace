---
name: recursos-judiciais-marcarios
description: "Redige recursos em lides marcárias — apelação (contra sentença), agravo de instrumento (contra interlocutória, ex. tutela de urgência) e embargos de declaração (omissão/contradição/obscuridade + prequestionamento). O tribunal segue o foro da causa — TJ se a causa correu na Justiça Estadual (abstenção/concorrência desleal); TRF se na Justiça Federal (nulidade de registro/ação contra indeferimento INPI). Use quando o operador disser \"vou recorrer da sentença de marca\", \"apelação marcária\", \"agravar a liminar de abstenção\", \"embargos de declaração no acórdão de marca\", \"perdi a ação de nulidade e quero recorrer\", \"recurso contra decisão do INPI no Judiciário\", ou descrever decisão judicial marcária adversa a recorrer. Cobre apelação (CPC 1.009-1.014), agravo (CPC 1.015-1.020) e embargos (CPC 1.022-1.026). Template: templates/recurso-judicial-marca.md."
---

# RECURSOS JUDICIAIS MARCÁRIOS

> Camada 4 — Contencioso judicial. Fase recursal. Acionada pelo `marcas-master` após decisão judicial marcária adversa. **O tribunal competente segue o foro da causa.**

## Anexos obrigatórios (context/)
- `context/lpi-marcas-titulo-iii.md` — dispositivos de mérito que sustentam a tese recursal (arts. 124/125/126; 129-132; 165-167; 173-175), conforme a lide.
- `context/lpi-9279-96.md` — arts. 209-210 (perdas e danos/abstenção), quando a lide envolver indenização (ficam na LPI integral, fora do recorte das marcas).
- `context/jurisprudencia-marcaria.md` — precedente aplicável à tese (TEMA 2 competência/Tema 950; TEMA 7 colidência/convivência; TEMA 4 danos; TEMA 5 controle do indeferimento), sob demanda e sempre validado.

## Objetivo
Produzir o recurso correto para a decisão impugnada, no tribunal certo, com admissibilidade aferida e tese de mérito ancorada na LPI e em jurisprudência real — preparando o prequestionamento quando houver horizonte de REsp/RE.

## Quando ativar
- Sentença marcária adversa → **apelação**.
- Interlocutória adversa (tutela de urgência deferida/indeferida, suspensão de efeitos do registro) → **agravo de instrumento**.
- Acórdão/sentença com omissão/contradição/obscuridade ou necessidade de prequestionar → **embargos de declaração**.

## Metodologia
1. **Estado do caso** via `memoria-de-caso-marca`: tipo de decisão, juízo/foro de origem, fundamentos da decisão, prazo.
2. **Tribunal correto (decorre do foro):** causa na **Justiça Estadual** (abstenção/concorrência desleal) → **TJ**; causa na **Justiça Federal** (nulidade/ação contra indeferimento INPI) → **TRF**. Confirmar o foro com base no pedido e no Tema 950 (`context/`).
3. **Recurso correto e admissibilidade:**
   - **Apelação** (CPC 1.009-1.014): tempestividade (15 dias úteis), preparo/porte, interposição ao juízo a quo + razões ao tribunal, efeito (regra suspensivo — CPC 1.012), honorários recursais.
   - **Agravo de instrumento** (CPC 1.015-1.020): cabimento (1.015, I — tutelas), peças obrigatórias (CPC 1.017), efeito suspensivo/tutela recursal (CPC 1.019, I), comunicação ao juízo de origem em 3 dias (CPC 1.018).
   - **Embargos de declaração** (CPC 1.022-1.026): apontar o vício específico (omissão/contradição/obscuridade/erro material), efeitos infringentes se for o caso, e **prequestionamento** explícito dos dispositivos (LPI/CPC).
4. **Tese de mérito:** error in judicando/in procedendo, combatendo cada fundamento (ex.: competência — Tema 950; ausência/presença de confusão — TEMA 7; danos — TEMA 4; controle do indeferimento sem fixar prazo — TEMA 5). Validar toda citação.
5. **Cálculo de preparo** (quando aplicável) e checklist de admissibilidade.
6. **Validação** por `validador-marcario`. Usar `templates/recurso-judicial-marca.md`.
7. Atualizar `memoria-de-caso-marca`.

## Entrega obrigatória final
- Recurso redigido (apelação / agravo / embargos), no **tribunal correto**, com admissibilidade aferida, tese de mérito, preparo (se aplicável) e — nos embargos com horizonte de REsp/RE — prequestionamento explícito.
- `memoria-de-caso-marca` atualizado + próximo passo + prazo.
- **Validação pela `suprema-corte-marcaria` (R1–R4) antes da entrega.**

## Guard
Nenhum dispositivo/súmula/acórdão entra na peça sem `validador-marcario`. **Tribunal correto (R1): segue o foro** — TJ (Estadual) ou TRF (Federal/INPI), conforme Tema 950. **Admissibilidade (R4):** conferir tempestividade, preparo/porte e peças obrigatórias do agravo (CPC 1.017) sob pena de não conhecimento. Entrega só após `suprema-corte-marcaria`. Na dúvida sobre vigência/existência, bloquear e checar ao vivo.
