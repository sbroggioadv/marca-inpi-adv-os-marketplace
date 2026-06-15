---
description: Gera o contrato de prestacao de servicos de registro de marca (pesquisa + deposito + acompanhamento, por classe).
allowed-tools: Read, Write, Edit, Bash, Glob, Grep
argument-hint: [marca + classes + valores aprovados]
---

Voce foi acionado pelo comando `/contrato` do plugin marca-inpi-adv-os.

Argumento recebido: `$ARGUMENTS`

**Objetivo:** formalizar o contrato apos a proposta aprovada.

## PROTOCOLO
1. **Acionar a skill `contrato-prestacao-servicos-marca`** — escopo pesquisa + deposito + acompanhamento; preve valores adicionais em manifestacao/exigencia/indeferimento; dimensiona por numero de classes.
2. Usar o template `templates/contrato-registro-marca.md`.

**Skill a acionar:** `contrato-prestacao-servicos-marca`.
