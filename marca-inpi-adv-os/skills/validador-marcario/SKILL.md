---
name: validador-marcario
description: Gate anti-alucinação do plugin de marcas. Antes de QUALQUER citação entrar em peça/parecer/proposta/contrato, valida a existência e a vigência de dispositivo legal (LPI/CUP/Madri/TRIPS), súmula, tese, classe NCL, código GRU e acórdão — cruzando com context/ e, na dúvida, exigindo checagem ao vivo (WebFetch real) ou BLOQUEANDO. Use sempre antes de citar, ou quando disser "valida essa citação", "esse artigo está vigente?", "esse acórdão existe?", "essa súmula vale?", "confere essa tese/Tema", "essa classe NCL existe?", "esse código de GRU está certo?", "antes de citar marcário".
---

# VALIDADOR-MARCARIO — Gate anti-alucinação

> Camada 1 (Fundação). Porta de verdade do plugin. Nenhuma citação marcária entra em entrega sem passar por aqui. Pode BLOQUEAR.

## Anexos obrigatorios (context/)
- `context/lpi-marcas-titulo-iii.md` — dispositivos das marcas (arts. 122–182), para conferir artigo/redação/vigência.
- `context/jurisprudencia-marcaria.md` — leading cases e súmulas/teses com link verificado, para conferir acórdão.

## Objetivo
Garantir que todo elemento citável — dispositivo legal, súmula, tese/Tema, classe NCL, código GRU, acórdão — exista, esteja vigente e corresponda ao que se quer afirmar, antes de a citação seguir para a peça.

## Quando ativar
- Sempre que outra skill estiver prestes a citar algo (lei, súmula, tese, classe, GRU, acórdão).
- Quando o operador pede para conferir uma citação ou duvida de vigência/existência.
- Como antecâmara obrigatória da `suprema-corte-marcaria`.

## Metodologia
1. **Inventariar as citações** do material (cada artigo/inciso, súmula, tese/Tema, classe NCL, código GRU, acórdão).
2. **Cruzar com `context/`:**
   - Dispositivo legal → `lpi-marcas-titulo-iii.md` (ou `lpi-9279-96.md` / `tratados-cup-madri-trips.md`): existe? a redação confere? está no Título III/lei vigente?
   - Acórdão/súmula/tese → `jurisprudencia-marcaria.md`: existe no corpus com órgão/número/relator/data e LINK?
   - Classe NCL → `ncl-13-2026-classes.md`: a classe existe (1–45) e o caput casa com a atividade?
   - Código GRU → `custos-gru-inpi.md` / `procedimento-emarcas.md`: o código corresponde ao ato (ex.: 389/394 depósito, 332 oposição, 3000 recurso contra indeferimento ≠ 333, 336 PAN).
3. **Pontos de atenção fixos (armadilhas):**
   - Recurso contra **indeferimento** = GRU **3000** (NÃO 333).
   - Nulidade de registro = **Justiça Federal**, INPI no feito (art. 175 LPI); abstenção/concorrência desleal entre particulares = **Justiça Estadual** (Tema 950).
   - **Súmula 142/STJ** = cancelada/superada pela 143 → bloquear.
   - Casos não confirmados no corpus (ex.: "Rainha") → não citar.
   - Valores de GRU mudam → conferir vigência na emissão.
4. **Na dúvida, checar ao vivo:** `WebFetch` na fonte oficial (planalto/LPI, portal STJ/TRF2, gov.br/inpi); só validar se a página abrir e confirmar. Sem confirmação → **BLOQUEAR** a citação.
5. **Acionar o guard global** `anti-alucinacao-juridica` em paralelo para jurisprudência.
6. **Emitir veredito por item:** ✅ VALIDADO (com referência), 🟡 REVISAR (corrigir e revalidar) ou 🔴 BLOQUEADO (não pode entrar).

## Entrega obrigatoria final
- Lista item a item com veredito (✅/🟡/🔴) + referência ao anexo ou URL que confirmou.
- Correções concretas dos itens 🟡.
- Bloqueio explícito dos itens 🔴 (com motivo) — esses NÃO seguem para a peça.

## Guard
Este é o próprio guard de citação do plugin: na ausência de confirmação em `context/` ou em fonte oficial ao vivo, a citação é BLOQUEADA. Validação aqui não dispensa o gate final da `suprema-corte-marcaria` (R3 jurisprudência real).
