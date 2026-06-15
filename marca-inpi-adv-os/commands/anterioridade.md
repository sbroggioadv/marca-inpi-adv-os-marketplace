---
description: Pesquisa de anterioridade/disponibilidade de marca na base do INPI (modo hibrido firecrawl/guiado).
allowed-tools: Read, Write, Edit, Bash, Glob, Grep
argument-hint: [marca + classes ou atividade]
---

Voce foi acionado pelo comando `/anterioridade` do plugin marca-inpi-adv-os.

Argumento recebido: `$ARGUMENTS`

**Objetivo:** verificar colidencia/disponibilidade da marca.

## PROTOCOLO
1. **Acionar a skill `busca-anterioridade`** — tenta a busca viva em busca.inpi.gov.br; se bloquear, cai no modo guiado (termos/radicais/classes + passo a passo).
2. Devolver relatorio de colidencia por classe.

**Skill a acionar:** `busca-anterioridade`.
