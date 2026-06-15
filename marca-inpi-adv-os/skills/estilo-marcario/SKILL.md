---
name: estilo-marcario
description: Define o estilo juridico das pecas e documentos marcarios do plugin — peticoes ao INPI, recursos, acoes judiciais, notificacoes, pareceres, propostas e contratos. Use sempre que outra skill for redigir um texto marcario, para garantir tom, estrutura e terminologia corretos. Acionada internamente pelas skills de redacao.
---

# ESTILO-MARCARIO

> Tier 0. Camada de estilo. Consultada pelas skills de redacao antes de entregar a peca.

## Anexos obrigatorios (context/)
- `context/metodologia-marcaria.md` (terminologia e regras de ouro).

## Terminologia correta (nao confundir)
- **Deposito** = ato de apresentar o pedido de registro (nao "protocolo de marca").
- **Pedido de registro** (em exame) ≠ **registro** (concedido, com certificado).
- **Titular** (do registro) ≠ **depositante** (do pedido em exame).
- **Oposicao** (administrativa, durante o exame) ≠ **nulidade** (apos a concessao) ≠ **caducidade** (por desuso).
- **Classe NCL** = recorte de produtos/servicos; cada classe e um **processo administrativo** proprio.
- **Anterioridade** = marca anterior colidente; **especialidade** = protecao limitada ao ramo (salvo alto renome).

## Estrutura padrao por tipo
- **Peticao administrativa (INPI):** enderecamento ao INPI + nº do processo + classe + fundamento (LPI + ato normativo) + pedido + GRU.
- **Peca judicial:** enderecamento ao juizo competente (atencao ao foro) + partes + fatos + fundamentacao (LPI + jurisprudencia validada) + pedidos (com liminar quando cabivel) + valor da causa.
- **Notificacao extrajudicial:** identificacao + direito do titular + conduta exigida + prazo + consequencia.
- **Parecer:** consulta + sintese fatica + analise (registrabilidade/risco) + conclusao objetiva.

## Tom
Tecnico, objetivo, assertivo. Sem promessa de resultado (Codigo de Etica OAB). Linguagem do cliente quando for material de apresentacao (proposta).

## Guard
Toda citacao legal/jurisprudencial passa por `validador-marcario`. Antes de entregar, `suprema-corte-marcaria` (R4 cuida da forma).
