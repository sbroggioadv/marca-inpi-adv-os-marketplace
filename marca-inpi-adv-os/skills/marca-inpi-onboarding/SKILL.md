---
name: marca-inpi-onboarding
description: Wizard de configuracao do plugin marca-inpi ao perfil do escritorio. Conduz perguntas estruturadas para criar a pasta marca-inpi/ com identidade (nome, OAB, escritorio, cidade, e-mail), paleta de cores do escritorio (para a proposta em PDF), honorarios-base por classe e modo de fluxo. Use quando o operador disser "configurar marca-inpi", "instalar marca-inpi", "primeira vez", "/start-marca-inpi", "onboarding marca".
---

> **🖱️ Escolhas = botoes:** em campos de **lista fechada** (areas de atuacao, modo de fluxo, atualizar/recriar, sim/nao) use a ferramenta **AskUserQuestion** para mostrar **botoes clicaveis** (max. 4 por pergunta; se houver mais, divida em 2). **Texto livre** (nome, OAB, cidade, e-mail, cores hex, valores de honorarios) segue como pergunta digitada normal.

# MARCA-INPI ONBOARDING

> Tier 0. Wizard de configuracao inicial. Linguagem acolhedora e didatica. Configura o plugin ao perfil do escritorio e habilita a proposta comercial com a identidade visual do operador.

## Anexos obrigatorios (context/)
- `context/metodologia-marcaria.md` (para explicar o que o plugin faz).

## 0. Acionamento
Acionada por `/start-marca-inpi` ou quando o operador disser "configurar marca", "primeira vez", "onboarding marca". Cria/atualiza a pasta `marca-inpi/` no diretorio de trabalho com o perfil.

## 1. Regras do wizard
- Uma pergunta por vez. Acolhedor, sem jargao.
- Listas fechadas = **AskUserQuestion** (botoes). Texto livre = pergunta digitada.
- Ao fim, gravar `marca-inpi/perfil.md` e confirmar.

## 2. Blocos de pergunta
1. **Identidade (texto livre):** nome do advogado, OAB (numero/UF), nome do escritorio, cidade, e-mail de contato.
2. **Paleta do escritorio (texto livre):** cor primaria (hex), cor secundaria (hex), e se ja tem logo (caminho do arquivo). Usado pela `proposta-comercial-marca` para gerar o PDF na identidade do escritorio.
3. **Honorarios-base (texto livre):** valor de honorarios **por classe** para: (a) pesquisa de anterioridade, (b) deposito/pedido de registro, (c) acompanhamento. Lembrar: cada classe e um processo, entao o orcamento multiplica por classe.
4. **Areas de atuacao marcaria (botoes — AskUserQuestion):** Registro/consultivo · Contencioso administrativo INPI · Contencioso judicial · Tudo. (multi-selecao)
5. **Modo de fluxo (botoes):** Checkpoint (confirma a cada etapa) · Continuo (executa e mostra no fim).
6. **Enquadramento de descontos INPI (botoes):** Atende clientes ME/EPP/MEI/pessoa fisica com desconto 50%? Sim · Nao · As vezes. (orienta a `proposta-comercial-marca` a oferecer o calculo com desconto).

## 3. Gravacao
Criar `marca-inpi/perfil.md` com todos os campos. Se ja existir, perguntar (botoes) **Atualizar** ou **Recriar**.

## Entrega obrigatoria final
- `marca-inpi/perfil.md` criado/atualizado + resumo do perfil + sugestao do primeiro comando (`/triagem-marca` ou `/anterioridade`).

## Guard
Nao inventar dados do operador. Honorarios e paleta sao do escritorio — nunca preencher por conta propria.
