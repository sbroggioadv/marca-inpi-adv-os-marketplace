Mode: production

# marca-inpi-adv-os

Plugin Claude Code **full-stack de Direito Marcário** (propriedade industrial — marcas), de uso **nacional** (Brasil). Cobre o ciclo completo do registro à defesa judicial, com a legislação e os procedimentos do INPI enraizados na base de conhecimento.

> Onboarding: rode **`/start-marca-inpi`**. Porta única: **`marcas-master`**.

## O que ele faz (4 setores)

1. **Consultivo / Registro + Comercial** — pesquisa de anterioridade, diagnóstico por CNPJ/contrato/site, classificação NCL, **proposta comercial e contrato por classe**, depósito no e-Marcas e emissão de GRU.
2. **Contencioso Administrativo INPI** — oposição, manifestação, cumprimento de exigência, recurso contra indeferimento, PAN (nulidade administrativa), caducidade, alto renome/notoriedade, Protocolo de Madri, ciclo de vida (prorrogação/cessão/licença).
3. **Contencioso Judicial** — abstenção de uso + liminar, concorrência desleal, nulidade de registro (Justiça Federal), ação para novo exame após indeferimento, contestação, recursos, liquidação de danos.
4. **Orquestração & QA** — `marcas-master` conduz o caso; `suprema-corte-marcaria` aplica 4 validações finais (R1–R4) antes de toda entrega.

## Fundação jurídica enraizada (`context/`)
LPI 9.279/96 · CUP (Paris) · Protocolo de Madri · TRIPS · NCL 13/2026 · Tabela de custos/GRU do INPI · Procedimento e-Marcas · Jurisprudência STJ/TRF2.

## Regra de ouro
**Cada classe NCL = 1 processo administrativo autônomo.** Honorários e custas são sempre calculados **por classe**.

## Comandos principais
`/start-marca-inpi` · `/marcas-master` · `/triagem-marca` · `/anterioridade` · `/registro` · `/proposta` · `/contrato` · `/oposicao` · `/recurso-inpi` · `/abstencao` · `/nulidade` · `/notificacao` · `/parecer-marcario` · `/revisao-final` · `/status-marca-inpi`
