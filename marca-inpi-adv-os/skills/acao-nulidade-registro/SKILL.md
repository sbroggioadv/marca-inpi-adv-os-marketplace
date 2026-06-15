---
name: acao-nulidade-registro
description: "Redige ação de nulidade de registro de marca de terceiro (arts. 173 a 175 da LPI). FORO — JUSTIÇA FEDERAL, com o INPI obrigatoriamente no polo (litisconsórcio/intervenção — art. 175); prazo prescricional de 5 anos da concessão (art. 174). Use quando o operador disser \"anular registro de marca de terceiro\", \"ação de nulidade\", \"o INPI concedeu marca igual à minha\", \"quero derrubar o registro do concorrente\", \"nulidade de registro na Justiça Federal\", \"registro indevido de terceiro\", ou descrever que um terceiro obteve registro em desacordo com a LPI (colidência, má-fé, nome empresarial) e o cliente quer desconstituí-lo judicialmente. Cobre arts. 165-167 (nulidade total/parcial, efeito desde o depósito) e 173-175 (ação, prescrição, foro federal, INPI no polo). Template: templates/acao-nulidade.md."
---

# AÇÃO DE NULIDADE DE REGISTRO DE MARCA (arts. 173-175 LPI)

> Camada 4 — Contencioso judicial. **Justiça Federal — INPI no polo.** Acionada pelo `marcas-master` quando o cliente quer desconstituir judicialmente registro de marca concedido pelo INPI a terceiro.

## Anexos obrigatórios (context/)
- `context/lpi-marcas-titulo-iii.md` — art. 165 (nulidade do registro em desacordo com a Lei; total ou parcial); art. 167 (efeito desde o depósito); art. 173 (legitimidade + tutela liminar de suspensão); art. 174 (prescrição em 5 anos da concessão); art. 175 (foro da Justiça Federal + INPI intervém quando não autor + prazo de resposta de 60 dias). Causas de nulidade no art. 124 (incisos) e arts. 125/126.
- `context/jurisprudencia-marcaria.md` — TEMA 2 (competência da Justiça Federal, Tema 950 / REsp 1.527.232, INPI no polo); TEMA 7 (colidência/risco de confusão); TEMA 3 (alto renome), sob demanda.

## Objetivo
Produzir ação de nulidade tempestiva, no foro federal correto, com o INPI no polo e com pedido de suspensão liminar dos efeitos do registro quando cabível.

## Quando ativar
- Terceiro obteve **registro concedido pelo INPI** em desacordo com a LPI (colidência art. 124 XIX, nome empresarial art. 124 V, má-fé art. 124 XXIII, ofensa a alto renome/notoriedade arts. 125/126, etc.).
- O cliente quer **desconstituir o registro** (não apenas opor-se na esfera administrativa — se ainda há prazo de oposição/PAN, considerar Camada 3).
- **Se** o objetivo for fazer o terceiro parar de usar sem discutir nulidade → é `acao-abstencao-uso-marca` (Justiça Estadual).

## Metodologia
1. **Estado do caso** via `memoria-de-caso-marca`: registro impugnado (nº, marca, classe, titular, data da concessão) e o direito anterior/vício do cliente.
2. **Foro — Justiça Federal (art. 175).** Endereçar à vara federal competente; **incluir o INPI no polo passivo** (litisconsórcio com o titular; o INPI intervém quando não for autor). Fundamentar no Tema 950 (`context/jurisprudencia-marcaria.md`).
3. **Prescrição (art. 174):** confirmar que está dentro dos **5 anos** da concessão do registro. Fora do prazo → inviável; reavaliar estratégia.
4. **Causa de nulidade (art. 165):** apontar o dispositivo violado na concessão (art. 124, inciso; 125; 126). Conferir cada artigo em `context/`.
5. **Colidência/risco de confusão:** comparar sinais e afinidade; possibilidade de confusão basta (jurisprudência — validar).
6. **Efeito (art. 167):** a nulidade retroage à data do depósito — pedir expressamente.
7. **Tutela liminar (art. 173, parágrafo único):** suspensão dos efeitos do registro e do uso, atendidos os requisitos processuais.
8. **Pedidos:** citação do titular (resposta em 60 dias — art. 175 § 1º) e do INPI; declaração de nulidade; anotação/publicação pelo INPI após o trânsito (art. 175 § 2º).
9. **Valor da causa**, provas. **Validação** por `validador-marcario`. Usar `templates/acao-nulidade.md`.
10. Atualizar `memoria-de-caso-marca`.

## Entrega obrigatória final
- Peça de nulidade redigida (endereçada à **Justiça Federal**, com o **INPI no polo**), com prescrição aferida, causa de nulidade, efeito desde o depósito, tutela liminar e valor da causa.
- `memoria-de-caso-marca` atualizado + próximo passo + prazo.
- **Validação pela `suprema-corte-marcaria` (R1–R4) antes da entrega.**

## Guard
Nenhum dispositivo/súmula/acórdão entra na peça sem `validador-marcario`. **Foro correto (R1): Justiça Federal com o INPI no polo (art. 175)** — sem o INPI a peça é reprovada; se o pedido for só abstenção, redirecionar para `acao-abstencao-uso-marca`. Confirmar prescrição de 5 anos (art. 174). Entrega só após `suprema-corte-marcaria`. Na dúvida sobre vigência/existência, bloquear e checar ao vivo.
