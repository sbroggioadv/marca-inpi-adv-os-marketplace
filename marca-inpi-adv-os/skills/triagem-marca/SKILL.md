---
name: triagem-marca
description: Classifica a demanda marcaria e roteia para a skill certa. Identifica o setor (consultivo/registro, contencioso administrativo INPI, contencioso judicial), o tipo de ato e, quando judicial, o foro competente. Use quando o operador descrever uma situacao de marca e nao souber qual caminho seguir, ou disser "triagem de marca", "qual o caminho", "que peca eu uso", "/triagem-marca".
---

# TRIAGEM-MARCA

> Tier 0. Porta de classificacao. Chamada pelo `marcas-master` no inicio de todo caso.

## Anexos obrigatorios (context/)
- `context/metodologia-marcaria.md` (mapa de skills + competencia).
- `context/lpi-marcas-titulo-iii.md` (para enquadrar o ato).

## Objetivo
Em poucas perguntas, dizer ao operador: setor, ato, skill alvo e (se judicial) foro.

## Arvore de decisao
1. **O cliente quer PROTEGER/REGISTRAR uma marca?**
   - Ainda nao depositou → `busca-anterioridade` + `diagnostico-marca` + fluxo comercial.
   - Marca coletiva/de certificacao → `marca-coletiva-certificacao`.
   - Indicacao geografica → `indicacao-geografica`.
2. **Ha um PROCESSO no INPI em andamento?**
   - Publicado para oposicao, quer opor marca de terceiro → `oposicao-registro`.
   - Cliente foi oposto, precisa defender → `manifestacao-oposicao`.
   - Recebeu exigencia do examinador → `cumprimento-exigencia`.
   - Pedido foi INDEFERIDO → `recurso-indeferimento-inpi` (GRU 3000).
   - Quer derrubar registro de terceiro na via administrativa → `nulidade-administrativa-pan`.
   - Marca de terceiro sem uso → `caducidade-marca`.
   - Alto renome / notoriedade → `marca-alto-renome-e-notoria`.
   - Registro internacional → `marca-internacional-madri`.
   - Prorrogacao/cessao/licenca → `ciclo-vida-marca`.
3. **Ha conflito que vai/esta no JUDICIARIO?**
   - Terceiro usando a marca do cliente → `acao-abstencao-uso-marca` (+ liminar) — **Justica Estadual**.
   - Concorrencia desleal → `acao-concorrencia-desleal` — **Justica Estadual**.
   - Anular registro de terceiro → `acao-nulidade-registro` — **Justica Federal (INPI no polo)**.
   - INPI indeferiu e ja esgotou recurso → `acao-judicial-concessao-registro` — **Justica Federal**.
   - Cliente foi acionado → `contestacao-marcaria`.
   - Recurso de sentenca/decisao → `recursos-judiciais-marcarios`.
4. **So precisa de orientacao/risco?** → `parecer-marcario`. **Notificar extrajudicialmente?** → `notificacao-extrajudicial-marcaria`.

## Entrega obrigatoria final
- Setor + ato + skill alvo + (se judicial) foro competente, em 3-5 linhas, e o handoff para o `marcas-master`.

## Guard
Na duvida de competencia, consultar `context/jurisprudencia-marcaria.md` (Tema 950). Nao redigir peca aqui — so classificar e rotear.
