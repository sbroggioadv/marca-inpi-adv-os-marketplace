---
name: parecer-marcario
description: Emite parecer de viabilidade e risco de registro de uma marca — analisa a registrabilidade a luz das proibicoes do art. 124 LPI, a colidencia com anterioridades (base do INPI) e a questao do alto renome/marca notoriamente conhecida (arts. 125-126), concluindo com um juizo de risco (alto/medio/baixo) e recomendacao. Formato consultivo, nao contencioso. Use quando o operador disser "esse nome pode ser registrado?", "parecer de marca", "qual o risco de registrar", "viabilidade da marca", "analisa a registrabilidade", "esse sinal e registravel?", "/parecer-marca".
---

# PARECER-MARCARIO

> Camada 2. Analise tecnica consultiva. Subsidia a decisao do cliente (seguir / ajustar / desistir) antes de investir em deposito — ou responde duvida pontual de registrabilidade.

## Anexos obrigatorios (context/)
- `context/lpi-marcas-titulo-iii.md` (art. 124 — proibicoes de registro; arts. 122-123 — o que e registravel; 125 alto renome; 126 marca notoriamente conhecida).
- `context/jurisprudencia-marcaria.md` (leading cases STJ/TRF2, criterios de colidencia, distintividade, alto renome).

## Objetivo
Dar ao cliente uma leitura honesta da chance de registro: o sinal e distintivo? Cai em alguma proibicao do art. 124? Ha anterioridade impeditiva? Esbarra em marca de alto renome (protecao em todas as classes, art. 125) ou notoriamente conhecida (art. 126)? E concluir com risco e recomendacao.

## Quando ativar
Quando o cliente quer so orientacao/risco (sem peca), ou quando a `busca-anterioridade`/`pedido-registro-inpi` levanta um sinal de alerta de registrabilidade que pede analise reflexiva.

## Metodologia
1. **Identificar o sinal e o ambito:** marca, forma de apresentacao, classes/ramo pretendidos.
2. **Distintividade (arts. 122-123):** o sinal e distintivo ou e generico/descritivo/de uso comum/sugestivo fraco? Avaliar o grau de protecao que ele comporta.
3. **Proibicoes do art. 124 (LPI):** percorrer as hipoteses aplicaveis (sinal generico/descritivo para o produto; enganoso; reproducao/imitacao de marca alheia no mesmo ramo — XIX; simbolo oficial; nome/imagem de terceiro sem autorizacao; etc.), cruzando com `context/lpi-marcas-titulo-iii.md`.
4. **Colidencia:** confrontar com as anterioridades (resultado da `busca-anterioridade`) — semelhanca grafica/fonetica + afinidade de classe/ramo, a luz dos criterios da `context/jurisprudencia-marcaria.md`.
5. **Alto renome / notoriedade:** verificar se ha marca de **alto renome** (art. 125 — protecao em todos os ramos) ou **notoriamente conhecida** (art. 126) que possa barrar mesmo em classe diferente.
6. **Concluir:** juizo de risco (alto/medio/baixo) + recomendacao (seguir / ajustar sinal / mudar classe / desistir) + caminhos (ex.: se uso ja existe sem registro, ponderar prioridade).

## Entrega obrigatoria final
- Parecer estruturado: consulta + sintese fatica + analise (distintividade · art. 124 · colidencia · alto renome) + **conclusao com risco e recomendacao** + referencias (validadas).
- Pontos de atencao e eventual proximo passo (ajuste do sinal / nova busca / seguir para `pedido-registro-inpi`).

## Guard
Parecer e consultivo — **nao prometer registro**; trabalhar com probabilidade e risco. Nenhum artigo, sumula ou acordao entra sem `validador-marcario`; alto renome/notoriedade so se confirmados (nao presumir). Risco alto deve ser dito com clareza, nao suavizado. Gate final: `suprema-corte-marcaria` (R1-R4).
