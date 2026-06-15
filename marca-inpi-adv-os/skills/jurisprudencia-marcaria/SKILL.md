---
name: jurisprudencia-marcaria
description: Busca viva e verificada de jurisprudência marcária (STJ, TRF2) para sustentar peça, parecer, oposição ou recurso. Prioriza os leading cases já curados em context/, e quando precisa de algo novo busca ao vivo (WebSearch/WebFetch; Firecrawl/Perplexity como fallback) sempre exigindo link de fonte real. Use quando precisar de precedente marcário, ou disser "jurisprudência de marca", "leading case marcário", "tem acórdão do STJ sobre", "precedente de abstenção/nulidade/caducidade/alto renome", "Tema 950", "como o STJ decide colidência", "busca jurisprudência marcária", "preciso citar acórdão de marca".
---

# JURISPRUDENCIA-MARCARIA — Precedente verificado

> Camada 1 (Fundação). Entrega precedente marcário REAL — primeiro do corpus curado, depois ao vivo — sempre com link de fonte. Zero acórdão inventado.

## Anexos obrigatorios (context/)
- `context/jurisprudencia-marcaria.md` — leading cases STJ/TRF2 + súmulas/teses, todos com link verificado. **Fonte primária — consultar antes de buscar ao vivo.**

## Objetivo
Fornecer o(s) precedente(s) pertinente(s) ao ponto controvertido, com órgão, número, relator, data, tese-síntese e URL de fonte real, prontos para citação.

## Quando ativar
- Uma peça/parecer/recurso precisa de jurisprudência marcária.
- O operador cita um Tema/REsp e quer confirmar/usar.
- Há tese controvertida (colidência, convivência, alto renome, caducidade, danos) a sustentar.

## Metodologia
1. **Identificar o tema** jurídico (abstenção de uso, nulidade/competência, alto renome, concorrência desleal/danos, controle judicial do INPI, caducidade, colidência/convivência).
2. **Buscar primeiro no corpus** `context/jurisprudencia-marcaria.md` — já mapeia por tema, com leading cases verificados. Mapa rápido:
   - **Abstenção + tutela:** REsp 1.826.832/MG; REsp 1.393.123/SP; AgInt no AREsp 1.629.976/SP.
   - **Nulidade / competência:** REsp 1.527.232 — Tema 950 (só Justiça Federal, com INPI; trade dress → Estadual).
   - **Alto renome:** REsp 1.336.164/SP (Bombril); REsp 1.893.426 (Naturaço — efeito prospectivo).
   - **Concorrência desleal / danos:** REsp 1.327.773/MG (dano material presumido; moral in re ipsa).
   - **Controle judicial do INPI:** REsp 1.787.676 (Perdigão — anula e manda reanalisar); MS 5084794-88.2023.4.02.5101/TRF2 (não cabe impor prazo).
   - **Caducidade:** REsp 1.236.218/RJ (ônus do uso ao titular); REsp 1.377.159 (justo motivo); EREsp 964.780/SP (efeitos ex nunc).
   - **Colidência/convivência:** REsp 2.120.527 (D'Linea — possibilidade de confusão basta); REsp 1.707.881/RS (marca x nome empresarial).
   - **Súmulas/teses:** Súm. 143/STJ (prescrição 5 anos perdas e danos); Jurisprudência em Teses Ed. 24 (Propriedade Industrial).
3. **Se faltar precedente** ou for preciso atualizar, **buscar ao vivo:** `WebSearch` + `WebFetch` no portal STJ/TRF2 ou fontes-espelho (Conjur, Migalhas, WIPO Lex, Trilhante); **Firecrawl/Perplexity como fallback**. Exigir SEMPRE um link que abra e confirme o caso.
4. **Verificar a existência real:** abrir a fonte e conferir número/relator/data/tese. Sem link que confirme → marcar como "NÃO ENCONTRADO" e NÃO citar (regra do próprio corpus). Atenção a casos não confirmados (ex.: "Rainha"; Súmula 142/STJ cancelada).
5. **Montar o bloco de citação:** caso · órgão/turma · número · relator · data · tese-síntese · URL.

## Entrega obrigatoria final
- Tabela de precedentes pertinentes com fonte (URL) para cada um.
- 1–3 leading cases comentados aplicados ao caso.
- Aviso sobre qualquer precedente não confirmado (excluído) ou que exija nova checagem.

## Guard
Toda citação passa pelo `validador-marcario` (cruza com `context/` + exige fetch real na dúvida) e pelo guard global `anti-alucinacao-juridica`. Nenhum acórdão/súmula/tese entra sem link de fonte que abra e confirme. A entrega do caso fecha pela `suprema-corte-marcaria`.
