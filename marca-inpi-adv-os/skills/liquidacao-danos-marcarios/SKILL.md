---
name: liquidacao-danos-marcarios
description: Apura as perdas e danos marcários na fase de liquidação (arts. 208 a 210 da LPI), pelo critério MAIS FAVORÁVEL ao prejudicado — (i) benefícios que o titular teria auferido, (ii) benefícios auferidos pelo infrator, ou (iii) remuneração razoável de licença — somados aos lucros cessantes. Trabalha com dano material presumido e dano moral in re ipsa reconhecidos pelo STJ. Use quando o operador disser "liquidar os danos da marca", "quanto vou receber pelo uso indevido", "calcular perdas e danos marcários", "liquidação de sentença de marca", "apurar lucros cessantes da marca", "qual o critério de indenização do art. 210", "danos da concorrência desleal", ou descrever uma condenação/acordo de marca que precisa quantificar a reparação. Cobre arts. 208-210 (critérios), dano in re ipsa, Súmula 143/STJ (prescrição 5 anos).
---

# LIQUIDAÇÃO DE DANOS MARCÁRIOS (arts. 208-210 LPI)

> Camada 4 — Contencioso judicial. Fase de liquidação/apuração. Acionada pelo `marcas-master` quando há condenação ou acordo a quantificar (perdas e danos por uso indevido de marca ou concorrência desleal).

## Anexos obrigatórios (context/)
- `context/lpi-9279-96.md` — art. 207 (independência das ações cíveis); art. 208 (indenização determinada pelos benefícios que o prejudicado teria auferido se a violação não tivesse ocorrido); art. 209 (perdas e danos + abstenção); art. 210 (os **três critérios** de apuração dos lucros cessantes — adotar o **mais favorável ao prejudicado**). *(arts. 207-210 estão na LPI integral; o recorte das marcas termina no art. 182.)*
- `context/jurisprudencia-marcaria.md` — TEMA 4 (dano material presumido + dano moral in re ipsa — REsp 1.327.773 Cotemig; quantum em REsp 1.826.832); Súmula 143/STJ (prescrição 5 anos das perdas e danos).

## Objetivo
Quantificar a reparação pelo critério **mais favorável ao prejudicado**, separando dano emergente, lucros cessantes e dano moral, com memória de cálculo defensável.

## Quando ativar
- Há sentença/acórdão/acordo reconhecendo a violação e remetendo a apuração à liquidação.
- O cliente precisa **arbitrar/calcular** a indenização (autor) ou **impugnar** o valor pleiteado (réu).

## Metodologia
1. **Estado do caso** via `memoria-de-caso-marca`: o que a sentença reconheceu, período da violação, dados financeiros disponíveis (do titular e/ou do infrator).
2. **Critério mais favorável (art. 210):** apurar pelos **três** e adotar o maior:
   - (i) os **benefícios que o prejudicado teria auferido** se não houvesse a violação;
   - (ii) os **benefícios auferidos pelo infrator** (disgorgement) com o uso indevido;
   - (iii) a **remuneração que o infrator pagaria** por licença autorizada (royalty razoável).
   Conferir o texto do art. 210 em `context/` — o critério é o **mais favorável ao prejudicado**.
3. **Dano emergente + lucros cessantes (arts. 208-209):** somar prejuízos efetivos e o que se deixou de ganhar (desvio de clientela, diluição).
4. **Dano material presumido / dano moral in re ipsa:** o STJ reconhece o dano material presumido pela própria violação e o dano moral in re ipsa — sustentar com TEMA 4 (validar antes de citar; o quantum do dano moral é arbitrado pelo juízo, não somado por fórmula).
5. **Prescrição (Súmula 143/STJ):** atenção ao limite de 5 anos das perdas e danos — confirmar vigência da súmula antes de citar.
6. **Memória de cálculo:** planilha por período, com fonte de cada dado, correção monetária e juros conforme o título; indicar premissas e necessidade de **perícia contábil** quando os dados forem do infrator.
7. **Validação** por `validador-marcario`.
8. Atualizar `memoria-de-caso-marca`.

## Entrega obrigatória final
- Apuração das perdas e danos com os **três critérios do art. 210** calculados e o **mais favorável** adotado, dano emergente + lucros cessantes, e fundamentação do dano moral in re ipsa.
- Memória de cálculo com fontes, correção e juros + indicação de perícia se necessária.
- Alerta de prescrição (Súmula 143/STJ).
- `memoria-de-caso-marca` atualizado + próximo passo.
- **Validação pela `suprema-corte-marcaria` (R1–R4) antes da entrega.**

## Guard
Nenhum dispositivo/súmula/acórdão entra no cálculo sem `validador-marcario` — dano in re ipsa só com precedente real (TEMA 4); Súmula 143/STJ só após confirmar vigência. **Critério (R4): art. 210 = o mais favorável ao prejudicado entre os três** — não escolher o menor por padrão; o dano moral é arbitrado, não somado por fórmula. Entrega só após `suprema-corte-marcaria`. Na dúvida sobre dado financeiro ou vigência, bloquear e checar ao vivo (perícia contábil quando necessário).
