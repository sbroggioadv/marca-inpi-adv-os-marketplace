---
name: base-legal-marcaria
description: Biblioteca de fundamentação legal marcária (LPI + CUP + Madri + TRIPS). Recupera, sob demanda das demais skills, o dispositivo exato — artigo, parágrafo, inciso e tratado — para sustentar peça, parecer, oposição, recurso ou contrato. Use quando precisar localizar a base legal de um ponto marcário, ou disser "qual artigo da LPI", "base legal marcária", "fundamento legal da marca", "o que diz o art. 124", "dispositivo da CUP/Madri/TRIPS", "prioridade unionista", "alto renome lei", "proibições de registro", "prazo do recurso na LPI", "competência da nulidade na lei", "preciso do texto do artigo".
---

# BASE-LEGAL-MARCARIA — Recuperação de dispositivos

> Camada 1 (Fundação). Serve as demais skills: entrega o dispositivo certo, vigente e referenciado, sem reproduzir lei "de cabeça".

## Anexos obrigatorios (context/)
- `context/lpi-marcas-titulo-iii.md` — recorte das marcas (arts. 122–182). **Fonte primária para tudo de marca.**
- `context/lpi-9279-96.md` — Lei 9.279/96 integral (consultar quando o ponto sair do Título III: crimes art. 189-195, disposições gerais, processo administrativo).
- `context/tratados-cup-madri-trips.md` — CUP (Decreto 75.572/1975), Protocolo de Madri e TRIPS.

## Objetivo
Localizar e entregar o dispositivo legal/convencional exato — com texto e referência ao anexo — que sustenta o ponto jurídico requisitado, pronto para citação por outra skill.

## Quando ativar
- Outra skill precisa do fundamento legal de um ponto (proibição, prazo, competência, prioridade).
- O operador pede o texto/artigo de um dispositivo marcário.
- Há dúvida sobre qual artigo cobre a situação (ex.: colidência, caducidade, prorrogação).

## Metodologia
1. **Identificar** o tema jurídico do pedido (registrabilidade, proibição, prazo, competência, tratado).
2. **Localizar no anexo** o dispositivo (sempre abrir `context/lpi-marcas-titulo-iii.md` primeiro). Mapa de referência rápido:
   - **Registrabilidade / propriedade:** art. 122 (sinais registráveis); art. 123 (definições — produto/serviço, coletiva, certificação); art. 129 (sistema atributivo).
   - **Proibições:** art. 124 (todos os incisos — destaque XIX colidência/confusão).
   - **Proteções especiais:** art. 125 (alto renome); art. 126 (notoriamente conhecida — exceção à territorialidade).
   - **Prioridade:** art. 127 LPI + art. 4 da CUP (prioridade unionista) em `tratados-cup-madri-trips.md`.
   - **Vigência/prorrogação:** art. 133 (prorrogação decenal).
   - **Caducidade:** arts. 143–146 (desuso 5 anos; justo motivo; ônus do uso).
   - **Processo administrativo:** art. 158 (oposição); art. 159 (exigência); arts. 168–172 (PAN — nulidade administrativa).
   - **Ação de nulidade:** arts. 173–175 (art. 175 = Justiça Federal, INPI no feito).
   - **Crimes / concorrência desleal:** art. 195 (em `lpi-9279-96.md`).
   - **Tratados:** CUP (tratamento nacional art. 2, prioridade art. 4); Madri (registro internacional via INPI); TRIPS (padrões mínimos) — ver `tratados-cup-madri-trips.md`.
3. **Conferir vigência/redação** do dispositivo no anexo (não citar de memória; a redação atual está no `context/`).
4. **Montar o bloco de fundamentação:** transcrição do dispositivo + referência ("ver `context/lpi-marcas-titulo-iii.md`, art. 124, XIX") + 1 linha de aplicação ao caso.
5. **Sinalizar lacuna:** se o dispositivo não estiver no anexo ou houver dúvida de vigência, encaminhar ao `validador-marcario` antes de liberar.

## Entrega obrigatoria final
- Dispositivo(s) localizado(s) com texto + referência ao anexo de `context/`.
- Bloco de fundamentação pronto para ser inserido pela skill solicitante.
- Aviso de qualquer dispositivo não confirmado (remete ao `validador-marcario`).

## Guard
Nenhum artigo, parágrafo ou inciso entra em peça sem constar do anexo de `context/` e sem passar pelo `validador-marcario`. Na dúvida sobre vigência/redação, bloquear e checar ao vivo. A entrega final do caso fecha pela `suprema-corte-marcaria`.
