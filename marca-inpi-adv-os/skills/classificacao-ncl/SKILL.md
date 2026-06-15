---
name: classificacao-ncl
description: Indica as classes NCL (Classificação de Nice 13/2026) que a marca do cliente precisa cobrir — obrigatórias e extras — cada uma JUSTIFICADA pela atividade real, e explica especificação pré-aprovada (389) vs livre preenchimento (394). Use quando precisar enquadrar atividades em classes, ou disser "em que classe registrar", "quais classes da minha marca", "classificação NCL", "código de classe da Nice", "preciso de mais de uma classe?", "produto ou serviço, qual classe", "especificação 389 ou 394", "lista de itens da classe", "classificar a atividade do cliente".
---

# CLASSIFICACAO-NCL — Enquadramento de classes

> Camada 1 (Fundação). Converte as atividades reais do cliente em classes NCL justificadas, com a regra "1 classe = 1 processo" sempre à frente.

## Anexos obrigatorios (context/)
- `context/ncl-13-2026-classes.md` — os 45 caputs de classe + regras de uso da NCL 13/2026 (vigente desde 01/01/2026). **Ler antes de classificar.**
- `context/metodologia-marcaria.md` — fluxo comercial e regras de ouro (precificação por classe).

## Objetivo
Entregar a lista de classes NCL que a marca deve cobrir — obrigatórias (núcleo da atividade) e extras (expansão/proteção defensiva) — cada uma com justificativa ligada à atividade do cliente, e orientar especificação 389 vs 394.

## Quando ativar
- Há atividades/CNPJ/site/contrato do cliente e é preciso definir as classes.
- O operador pergunta em que classe registrar ou se precisa de mais de uma.
- Antes do `planejamento-portfolio-marca` e da `proposta-comercial-marca` (que precificam por classe).

## Metodologia
1. **Levantar as atividades** do cliente (objeto social, produtos, serviços, canais, planos de expansão). Se vier do `diagnostico-marca`, reusar.
2. **Mapear produto x serviço:** classes 1–34 = produtos; classes 35–45 = serviços (ver `context/ncl-13-2026-classes.md`). Uma mesma marca pode precisar de classe de produto E de serviço.
3. **Selecionar as classes** lendo os 45 caputs no anexo. Para cada classe candidata, casar o caput com a atividade concreta (ex.: vestuário → classe 25; venda/loja desses produtos → classe 35; restaurante → classe 43; software → classe 9 produto e/ou 42 serviço).
4. **Separar obrigatórias x extras:**
   - **Obrigatórias** = núcleo do que o cliente faz/vende hoje.
   - **Extras** = expansão prevista, proteção defensiva contra colidência, ou serviço acessório (ex.: e-commerce em 35).
5. **Justificar cada classe** em 1 linha, ligada à atividade — nunca classe "por garantia" sem fundamento.
6. **Explicar a especificação** (ver anexo): **389** = lista pré-aprovada pelo INPI (menor risco de exigência, mais barata); **394** = livre preenchimento (quando o item não está na lista pré-aprovada — maior risco de exigência). Recomendar 389 sempre que os itens existirem na lista.
7. **Apontar o PDF oficial de itens** (a lista de milhares de itens NÃO é copiada inline): `https://www.gov.br/inpi/pt-br/servicos/marcas/classificacao-marcas/Lista_Nice_NCL_13_2026.pdf` (+ Listas Auxiliares de Produtos/Serviços citadas no anexo).
8. **Reforçar a regra de ouro:** cada classe = 1 processo administrativo, 1 GRU, 1 exame → honorários e custas multiplicam por classe (multiclasse não está disponível no e-Marcas).

## Entrega obrigatoria final
- Tabela de classes: nº · caput resumido · obrigatória/extra · justificativa · 389 ou 394.
- Total de classes (= total de processos/GRUs) para alimentar a precificação.
- Link do PDF oficial de itens + alerta de que a especificação fina sai da lista pré-aprovada.

## Guard
Não inventar número de classe nem item: tudo confere com `context/ncl-13-2026-classes.md` e com o PDF oficial. Qualquer dispositivo legal citado passa pelo `validador-marcario`. Precificação sempre por classe. A entrega do caso fecha pela `suprema-corte-marcaria`.
