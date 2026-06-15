---
name: suprema-corte-marcaria
description: Gate de qualidade final do plugin marca-inpi. Aplica 4 validacoes (R1 fatos/competencia, R2 fundamentacao legal vigente, R3 jurisprudencia real verificada, R4 forma/pedidos/custas) antes de qualquer entrega ao operador. Use SEMPRE antes de entregar peca, proposta, contrato ou parecer; acionada pelo marcas-master ao fechar qualquer ato. Tambem quando o operador disser "revisao final", "valida antes de entregar", "/revisao-final".
---

# SUPREMA-CORTE-MARCARIA — Gate R1-R4

> Tier 0. Auditoria final obrigatoria. Nenhuma entrega sai sem passar por aqui.

## Anexos obrigatorios (context/)
- `context/lpi-marcas-titulo-iii.md`, `context/jurisprudencia-marcaria.md`, `context/custos-gru-inpi.md`, `context/metodologia-marcaria.md`.

## As 4 validacoes
**R1 — Fatos e competencia.** Os fatos batem com o caso (`memoria-de-caso-marca`)? O setor esta certo? Se judicial, o **foro** esta correto (nulidade = Justica Federal/INPI; abstencao/concorrencia desleal = Justica Estadual)? A classe NCL esta correta?

**R2 — Fundamentacao legal vigente.** Cada dispositivo citado existe e esta vigente (cruzar com `context/lpi-marcas-titulo-iii.md` e tratados)? Os artigos correspondem ao instituto (ex.: 158 oposicao, 168-172 PAN, 173-175 acao de nulidade, 143 caducidade, 125 alto renome)?

**R3 — Jurisprudencia real.** Todo acordao/sumula/tese citado passou pelo `validador-marcario` (existe, com fonte real)? Nenhuma citacao inventada. Em caso de duvida, remover ou checar ao vivo.

**R4 — Forma, pedidos e custas.** A peca tem enderecamento, partes, pedidos claros (liminar quando cabivel) e valor da causa? Para atos no INPI: a **GRU correta** (codigo certo: 389/394 deposito, 3000 recurso de indeferimento, 332 oposicao, 336 PAN, 374/375 prorrogacao) e o calculo **por classe**? Honorarios e custas separados e explicados?

## Metodologia
1. Rodar R1 -> R2 -> R3 -> R4 em ordem.
2. Marcar cada item como OK / CORRIGIR.
3. Se houver CORRIGIR, devolver a skill de origem com as correcoes; nao entregar.
4. So liberar a entrega quando R1-R4 = OK.

## Entrega obrigatoria final
- Veredito (LIBERADO / CORRIGIR) + lista do que foi checado + correcoes aplicadas.

## Guard
Este gate nao "passa pano": na duvida em R3 (jurisprudencia), o default e remover/checar, nunca presumir. Custas erradas (codigo ou nao multiplicar por classe) = reprova em R4.
