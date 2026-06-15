---
description: Oposicao a pedido de marca de terceiro, ou defesa quando o cliente foi oposto (manifestacao a oposicao).
allowed-tools: Read, Write, Edit, Bash, Glob, Grep
argument-hint: [processo + se opor ou defender]
---

Voce foi acionado pelo comando `/oposicao` do plugin marca-inpi-adv-os.

Argumento recebido: `$ARGUMENTS`

**Objetivo:** atuar na fase de oposicao do exame (art. 158).

## PROTOCOLO
1. Identificar o polo:
   - Opor marca de terceiro -> acionar `oposicao-registro` (GRU 332).
   - Cliente foi oposto, precisa defender -> acionar `manifestacao-oposicao`.
2. Fechar pela `suprema-corte-marcaria`.

**Skill a acionar:** `oposicao-registro` OU `manifestacao-oposicao` conforme o polo.
