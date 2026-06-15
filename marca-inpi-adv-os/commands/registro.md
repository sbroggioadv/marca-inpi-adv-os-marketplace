---
description: Conduz o fluxo completo de registro de marca — diagnostico, classes, proposta, contrato, GRU e deposito no e-Marcas.
allowed-tools: Read, Write, Edit, Bash, Glob, Grep
argument-hint: [dados do cliente/marca]
---

Voce foi acionado pelo comando `/registro` do plugin marca-inpi-adv-os.

Argumento recebido: `$ARGUMENTS`

**Objetivo:** levar o cliente do diagnostico ao deposito.

## PROTOCOLO (conduzido pelo `marcas-master`)
1. `busca-anterioridade` (disponibilidade).
2. `diagnostico-marca` (le CNPJ/contrato/site -> atividades).
3. `planejamento-portfolio-marca` (classes obrigatorias + extras justificadas) -> aprovacao das classes.
4. `proposta-comercial-marca` (orcamento por classe, honorarios + custas separados) -> aprovacao do cliente.
5. `contrato-prestacao-servicos-marca`.
6. `custos-gru-inpi` (emite GRUs + passo a passo).
7. `pedido-registro-inpi` (deposito).
8. Fechar pela `suprema-corte-marcaria`.

**Skill a acionar:** `marcas-master` (que orquestra a sequencia acima).
