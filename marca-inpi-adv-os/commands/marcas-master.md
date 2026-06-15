---
description: Porta unica do plugin marca-inpi — descreva a demanda marcaria em linguagem natural e o orquestrador classifica, roteia e conduz o caso.
allowed-tools: Read, Write, Edit, Bash, Glob, Grep
argument-hint: [descricao da demanda marcaria]
---

Voce foi acionado pelo comando `/marcas-master` do plugin marca-inpi-adv-os.

Argumento recebido: `$ARGUMENTS`

**Objetivo:** conduzir qualquer demanda marcaria de ponta a ponta.

## PROTOCOLO
1. **Acionar a skill `marcas-master`** — ela le `context/metodologia-marcaria.md`, classifica via `triagem-marca`, carrega `memoria-de-caso-marca` e conduz os desdobramentos.
2. Fluxo de registro segue: anterioridade -> diagnostico -> classes -> proposta -> contrato -> GRU -> deposito.
3. Toda entrega fecha pela `suprema-corte-marcaria` (R1-R4).

**Skill a acionar:** `marcas-master`.
