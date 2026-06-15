---
description: Gera a proposta comercial de registro de marca (orcamento por classe, honorarios + custas separados, PDF na paleta do escritorio).
allowed-tools: Read, Write, Edit, Bash, Glob, Grep
argument-hint: [marca + classes definidas]
---

Voce foi acionado pelo comando `/proposta` do plugin marca-inpi-adv-os.

Argumento recebido: `$ARGUMENTS`

**Objetivo:** produzir a proposta/resumo do caso para o cliente.

## PROTOCOLO
1. **Acionar a skill `proposta-comercial-marca`** — le `marca-inpi/perfil.md` (paleta + honorarios), calcula por classe (cada classe = 1 processo), separa honorarios e custas GRU e gera o documento na identidade do escritorio.
2. Considerar desconto 50% (ME/EPP/MEI/PF) quando aplicavel.

**Skill a acionar:** `proposta-comercial-marca`.
