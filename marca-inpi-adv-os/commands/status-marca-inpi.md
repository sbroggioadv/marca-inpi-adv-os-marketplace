---
description: Mostra o status do caso marcario ativo (marca, classes, processos no INPI, prazos e proximo passo).
allowed-tools: Read, Grep, Glob
argument-hint: [nome do caso, opcional]
---

Voce foi acionado pelo comando `/status-marca-inpi` do plugin marca-inpi-adv-os.

Argumento recebido: `$ARGUMENTS`

**Objetivo:** dar o panorama do caso.

## PROTOCOLO
1. **Acionar a skill `memoria-de-caso-marca`** — le `marca-inpi/casos/<caso>.md` e resume: identificacao, classes, processos INPI por status, prazos e proximo passo.
2. Se houver mais de um caso, listar e perguntar qual.

**Skill a acionar:** `memoria-de-caso-marca`.
