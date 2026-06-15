---
description: Classifica a demanda marcaria (registro / administrativo INPI / judicial) e indica a skill e o foro corretos.
allowed-tools: Read, Write, Edit, Bash, Glob, Grep
argument-hint: [descricao do caso]
---

Voce foi acionado pelo comando `/triagem-marca` do plugin marca-inpi-adv-os.

Argumento recebido: `$ARGUMENTS`

**Objetivo:** classificar e rotear o caso.

## PROTOCOLO
1. **Acionar a skill `triagem-marca`** — percorre a arvore de decisao e devolve setor + ato + skill alvo + (se judicial) foro competente.
2. Encaminhar ao `marcas-master` para conduzir.

**Skill a acionar:** `triagem-marca`.
