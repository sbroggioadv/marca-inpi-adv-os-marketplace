---
description: Recurso administrativo contra o indeferimento de pedido de registro de marca no INPI (GRU 3000).
allowed-tools: Read, Write, Edit, Bash, Glob, Grep
argument-hint: [processo indeferido + motivo]
---

Voce foi acionado pelo comando `/recurso-inpi` do plugin marca-inpi-adv-os.

Argumento recebido: `$ARGUMENTS`

**Objetivo:** reverter o indeferimento na via administrativa.

## PROTOCOLO
1. **Acionar a skill `recurso-indeferimento-inpi`** — prazo art. 212; **GRU 3000** (nao 333), por classe.
2. Se o recurso administrativo ja se esgotou, considerar a via judicial via `acao-judicial-concessao-registro`.
3. Fechar pela `suprema-corte-marcaria`.

**Skill a acionar:** `recurso-indeferimento-inpi`.
