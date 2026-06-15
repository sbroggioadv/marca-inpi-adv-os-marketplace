---
description: Inicia o wizard de configuracao do plugin marca-inpi — cria a pasta marca-inpi/ com identidade, paleta do escritorio, honorarios-base por classe e modo de fluxo.
allowed-tools: Read, Write, Edit, Bash, Glob, Grep
argument-hint: [--update para reconfigurar]
---

Voce foi acionado pelo comando `/start-marca-inpi` do plugin marca-inpi-adv-os.

Argumento recebido: `$ARGUMENTS`

**Objetivo:** configurar o plugin de marcas ao perfil do escritorio.

## PROTOCOLO
1. **Acionar a skill `marca-inpi-onboarding`** imediatamente — ela conduz o wizard completo (com botoes via AskUserQuestion nas escolhas de lista fechada).
2. O wizard cria `<cwd>/marca-inpi/perfil.md` com identidade, paleta de cores, honorarios-base por classe e modo de fluxo.
3. Se ja existir `marca-inpi/perfil.md`, oferecer continuar / atualizar / recriar.
4. Se o argumento for `--update`, ir direto para o fluxo de atualizacao.

**Skill a acionar:** `marca-inpi-onboarding`.
