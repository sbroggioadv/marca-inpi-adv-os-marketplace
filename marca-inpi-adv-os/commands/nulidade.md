---
description: Anular registro de marca de terceiro — via administrativa (PAN no INPI) ou judicial (Justica Federal, INPI no polo).
allowed-tools: Read, Write, Edit, Bash, Glob, Grep
argument-hint: [registro alvo + via]
---

Voce foi acionado pelo comando `/nulidade` do plugin marca-inpi-adv-os.

Argumento recebido: `$ARGUMENTS`

**Objetivo:** derrubar um registro indevido de terceiro.

## PROTOCOLO
1. Escolher a via:
   - Administrativa (prazo art. 174, 5 anos) -> `nulidade-administrativa-pan` (GRU 336).
   - Judicial -> `acao-nulidade-registro` (**Justica Federal**, INPI no polo, arts. 173-175).
2. Fechar pela `suprema-corte-marcaria` (foro correto em R1).

**Skill a acionar:** `nulidade-administrativa-pan` OU `acao-nulidade-registro` conforme a via.
