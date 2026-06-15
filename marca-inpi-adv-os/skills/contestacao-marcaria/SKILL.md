---
name: contestacao-marcaria
description: Redige a defesa do réu em ações marcárias (abstenção de uso, concorrência desleal, nulidade de registro, ação contra indeferimento). Levanta a preliminar de competência conforme o pedido (incompetência da Justiça Estadual para discutir nulidade — STJ Tema 950; necessidade do INPI no polo na nulidade — art. 175) e faz impugnação específica. Use quando o operador disser "fui acionado por causa de marca", "me processaram dizendo que copiei a marca", "preciso contestar ação de abstenção", "defesa em ação de nulidade", "contestação marcária", "o INPI/concorrente me processou", "quero defender meu registro", ou descrever que o cliente é réu em demanda de marca e precisa de defesa. Cobre preliminares (competência/foro, INPI no polo), impugnação específica dos fatos, princípio da especialidade, convivência de marcas e marcas fracas/evocativas.
---

# CONTESTAÇÃO MARCÁRIA (defesa do réu)

> Camada 4 — Contencioso judicial. Defesa do réu. Acionada pelo `marcas-master` quando o cliente é réu em ação marcária. **O foro/preliminar dependem do pedido da inicial** — verificar antes de tudo.

## Anexos obrigatórios (context/)
- `context/lpi-marcas-titulo-iii.md` — arts. 129-132 (extensão e limites do direito do titular — art. 132 traz hipóteses que o titular NÃO pode impedir); art. 124 (XIX colidência, princípio da especialidade); arts. 173-175 (na nulidade: foro federal, INPI no polo, prescrição 5 anos).
- `context/jurisprudencia-marcaria.md` — TEMA 2 (competência — Tema 950); TEMA 7 (convivência/especialidade — REsp 1.893.426 Naturaço, marca x nome empresarial; marcas fracas/evocativas convivem — REsp 1.336.164 Bombril/Tecbril); TEMA 3 (alto renome só prospectivo), sob demanda.

## Objetivo
Produzir defesa que ataque vícios processuais (competência/foro, litisconsórcio do INPI), impugne especificamente cada fato e construa o mérito (especialidade, convivência, marca fraca, ausência de confusão).

## Quando ativar
- Cliente é **réu** em: ação de abstenção, ação de concorrência desleal, ação de nulidade de registro, ou ação contra indeferimento (quando o INPI é réu, a defesa cabe à PFE/INPI — aqui o foco é o réu particular/titular).
- Há prazo de resposta em curso (na nulidade, 60 dias — art. 175 § 1º; nas demais, prazo do CPC).

## Metodologia
1. **Estado do caso** via `memoria-de-caso-marca`: o que a inicial pede (abstenção? nulidade? concorrência desleal?), marca, classe, registros envolvidos, provas.
2. **Preliminar de competência (conforme o pedido):**
   - Se a inicial pede, na **Justiça Estadual**, o reconhecimento (ainda que incidental) de **nulidade** de registro → arguir **incompetência absoluta**: só a Justiça Federal, com o INPI, decide nulidade (STJ Tema 950; art. 175). Conferir em `context/`.
   - Se é ação de **nulidade na Justiça Federal sem o INPI** no polo → arguir **litisconsórcio necessário** do INPI (art. 175).
3. **Impugnação específica:** rebater **fato a fato** da inicial (CPC — ônus de impugnação específica); não deixar fato sem resposta.
4. **Mérito marcário:**
   - **Princípio da especialidade** (art. 124 XIX): exclusividade limitada à classe/afinidade; segmentos distintos → convivência (REsp 1.893.426 — validar).
   - **Marca fraca/evocativa:** baixa distintividade → exclusividade mitigada, convivência possível (REsp 1.336.164 — validar).
   - **Ausência de risco de confusão**, limites do art. 132, anterioridade/precedência (art. 129 § 1º), prescrição (art. 174 na nulidade; Súmula 143/STJ nas perdas e danos — confirmar vigência).
5. **Provas** e, se cabível, **reconvenção** (ex.: o réu também é titular e quer abstenção da autora — atenção: pedido de nulidade exige foro federal/INPI).
6. **Validação** por `validador-marcario`.
7. Atualizar `memoria-de-caso-marca`.

## Entrega obrigatória final
- Contestação redigida com **preliminar de competência adequada ao pedido**, impugnação específica e mérito (especialidade/convivência/marca fraca/ausência de confusão), provas e pedidos.
- `memoria-de-caso-marca` atualizado + próximo passo + prazo.
- **Validação pela `suprema-corte-marcaria` (R1–R4) antes da entrega.**

## Guard
Nenhum dispositivo/súmula/acórdão entra na peça sem `validador-marcario` — convivência/marca fraca só com precedente real (TEMA 7); Súmula 143/STJ só após confirmar vigência. **Competência (R1):** ler o pedido da inicial e calibrar a preliminar — nulidade ⇒ Justiça Federal + INPI (Tema 950 / art. 175). Entrega só após `suprema-corte-marcaria`. Na dúvida, bloquear e checar ao vivo.
