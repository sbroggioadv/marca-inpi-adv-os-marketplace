---
name: acao-abstencao-uso-marca
description: "Redige ação de abstenção de uso de marca com pedido de tutela de urgência/liminar, para o titular de registro vigente no INPI fazer cessar o uso indevido por terceiro. FORO — JUSTIÇA ESTADUAL (vara cível/empresarial), pois não se discute nulidade de registro alheio (STJ Tema 950). Use quando o operador disser \"querem usar minha marca\", \"alguém está usando minha marca igual\", \"ação de abstenção\", \"fazer parar o uso da minha marca\", \"concorrente copiou minha marca registrada\", \"pedir liminar pra tirar a marca do ar\", \"abstenção de uso com multa diária\", ou descrever um titular de marca registrada que quer obrigar terceiro a parar de usar o sinal. Cobre arts. 129-132 (direitos do titular) e 209-210 (abstenção + perdas e danos) da LPI, astreinte (CPC 537) e tutela de urgência (CPC 300). Template: templates/acao-abstencao.md."
---

# AÇÃO DE ABSTENÇÃO DE USO DE MARCA (+ tutela de urgência)

> Camada 4 — Contencioso judicial. **Justiça Estadual.** Acionada pelo `marcas-master` quando o cliente é titular de registro vigente e quer fazer cessar o uso indevido por terceiro, sem discutir nulidade.

## Anexos obrigatórios (context/)
- `context/lpi-marcas-titulo-iii.md` — arts. 129-131 (aquisição e proteção do direito, uso exclusivo); art. 132 (limites do direito do titular — o que NÃO pode impedir).
- `context/lpi-9279-96.md` — arts. 209 e 210 (abstenção + perdas e danos, critérios de lucros cessantes) — estão na LPI integral, fora do recorte das marcas.
- `context/jurisprudencia-marcaria.md` — TEMA 1 (abstenção + tutela), TEMA 2 (competência — Tema 950), TEMA 7 (colidência/risco de confusão), sob demanda.

## Objetivo
Produzir ação de abstenção tempestiva e bem instruída, com pedido liminar de cessação do uso sob multa diária, que faça parar a violação e assegure as perdas e danos.

## Quando ativar
- Cliente é **titular de registro vigente no INPI** (ou depositante com direito de precedência — art. 129 § 1º) e identificou terceiro usando sinal idêntico/semelhante para produto/serviço idêntico ou afim.
- O pedido é de **cessação do uso** por violação do registro, **sem** discutir a nulidade de registro alheio.
- **Se** a discussão envolver nulidade de registro do terceiro → não é esta skill: vai para `acao-nulidade-registro` (Justiça Federal).

## Metodologia
1. **Estado do caso** via `memoria-de-caso-marca`: registro do cliente (nº, classe NCL, data, vigência), uso indevido do réu (sinal, produto/serviço, canais, provas).
2. **Foro — Justiça Estadual.** Confirmar que o pedido é de abstenção por violação (sem nulidade). Fundamentar a competência estadual no STJ Tema 950 (`context/jurisprudencia-marcaria.md`).
3. **Direito do titular:** sustentar o uso exclusivo (arts. 129-131) e a violação (art. 124, XIX, conferido em `context/`). Verificar os limites do art. 132 (esgotamento, peças/acessórios, citação) para antecipar defesa.
4. **Colidência:** comparar sinais (gráfico/fonético/ideológico) e afinidade de produtos/serviços; risco de confusão basta (jurisprudência — validar).
5. **Tutela de urgência (CPC 300):** probabilidade do direito (registro vigente) + perigo de dano (confusão/desvio de clientela); pedir cessação imediata sob **astreinte** (CPC 537).
6. **Perdas e danos:** pedir abstenção + indenização (art. 209); danos materiais apurados em liquidação pelo critério mais favorável (art. 210 — remeter a `liquidacao-danos-marcarios`); danos morais conforme jurisprudência (validar).
7. **Valor da causa** e provas (documental/pericial/testemunhal).
8. **Validação:** todo dispositivo/jurisprudência passa por `validador-marcario`. Usar `templates/acao-abstencao.md`.
9. Atualizar `memoria-de-caso-marca` (ação proposta, pedido liminar, próximo passo).

## Entrega obrigatória final
- Peça de abstenção redigida (endereçada à **Justiça Estadual**), com tutela de urgência e pedido de astreinte, perdas e danos e valor da causa.
- Fundamentação da competência estadual (Tema 950).
- `memoria-de-caso-marca` atualizado + próximo passo + prazo.
- **Validação pela `suprema-corte-marcaria` (R1–R4) antes da entrega.**

## Guard
Nenhum dispositivo/súmula/acórdão entra na peça sem `validador-marcario`. **Foro correto (R1): Justiça Estadual** — se o pedido virar discussão de nulidade, parar e redirecionar para `acao-nulidade-registro` (Justiça Federal). Entrega só após `suprema-corte-marcaria`. Na dúvida sobre vigência de dispositivo ou existência de precedente, bloquear e checar ao vivo.
