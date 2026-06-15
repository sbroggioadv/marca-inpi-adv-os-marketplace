---
description: Gate de revisao final R1-R4 (Suprema Corte Marcaria) antes de qualquer entrega.
allowed-tools: Read, Grep, Glob
argument-hint: [peca/proposta/contrato a validar]
---

Voce foi acionado pelo comando `/revisao-final` do plugin marca-inpi-adv-os.

Argumento recebido: `$ARGUMENTS`

**Objetivo:** auditar a entrega antes de liberar ao operador.

## PROTOCOLO
1. **Acionar a skill `suprema-corte-marcaria`** — aplica R1 (fatos/competencia/foro), R2 (fundamentacao vigente), R3 (jurisprudencia real validada), R4 (forma/pedidos/GRU correta por classe).
2. Veredito: LIBERADO ou CORRIGIR (devolve a skill de origem).

**Skill a acionar:** `suprema-corte-marcaria`.
