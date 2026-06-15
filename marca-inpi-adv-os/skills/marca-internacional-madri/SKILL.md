---
name: marca-internacional-madri
description: Conduz o pedido internacional de registro de marca via Protocolo de Madri pelo INPI (Brasil como Escritório de origem), internalizado pelo Decreto 10.033/2019, vigente desde 02/10/2019. Use quando o operador disser "registrar marca no exterior", "Protocolo de Madri", "pedido internacional de marca", "marca em vários países", "proteger marca fora do Brasil", "registro internacional via INPI", "formulário MM2", "eMadrid", "designar países", ou descrever a intenção de levar a marca brasileira do cliente a outros países por um único pedido. Exige pedido/registro de base no INPI; o escopo internacional é igual ou mais restrito, nunca mais amplo. Dependência de 5 anos ("ataque central"). GRU 3004 (certificação do pedido internacional) + taxas da OMPI em francos suíços.
---

# MARCA INTERNACIONAL — PROTOCOLO DE MADRI (Decreto 10.033/2019)

> Camada 3 — Contencioso/serviços administrativos INPI. Acionada pelo `marcas-master` quando o cliente quer proteger a marca em outros países por um único pedido internacional, tendo o INPI como Escritório de origem.

## Anexos obrigatórios (context/)
- `context/tratados-cup-madri-trips.md` — **Protocolo de Madri** (Decreto 10.033/2019, vigência 02/10/2019; INPI como Administração de origem e Parte Contratante designada; pedido/registro de base obrigatório; 3 etapas; designação de países; **dependência de 5 anos / "ataque central"**; transformação em 3 meses; prazo de 2 meses para manter a data BR; exame nacional em 12/18 meses; validade 10 anos renováveis; taxas OMPI em CHF); prioridade unionista (CUP art. 4 — 6 meses).
- `context/procedimento-emarcas.md` — cadastro e-INPI, emissão da GRU e operacional do peticionamento.
- `context/custos-gru-inpi.md` — GRU 3004 (certificação do pedido internacional via INPI; confirmar valor na emissão). Taxas da OMPI à parte, em francos suíços.
- `context/lpi-marcas-titulo-iii.md` — base nacional (o pedido/registro de base segue a LPI).

## Objetivo
Levar a marca do cliente a outros países por um único pedido internacional, com o INPI certificando contra a base nacional e a OMPI gerindo a inscrição internacional, respeitando o escopo da base e os prazos críticos.

## Quando ativar
- O cliente é nacional, domiciliado ou tem estabelecimento efetivo no Brasil e quer proteção em outros países membros do Sistema de Madri.
- Já existe (ou está sendo depositado) um pedido/registro de base no INPI.

## Metodologia
1. **Estado do caso** via `memoria-de-caso-marca`: marca, pedido/registro de **base** no INPI (nº, classe, situação — publicado/registrado), países-alvo, classes pretendidas.
2. **Legitimidade e base (obrigatórias):** confirmar elegibilidade (nacional/domiciliado/estabelecimento no Brasil) e a existência de **pedido ou registro de base** no INPI. O pedido internacional só pode conter produtos/serviços **dentro do escopo** da base — **igual ou mais restrito, nunca mais amplo**; para classes adicionais, apontar mais de uma base.
3. **As 3 etapas:** (1) **certificação pelo INPI** (origem) — cadastro e-INPI, **GRU 3004**, **Formulário MM2** em inglês ou espanhol no eMadrid; (2) **exame formal pela OMPI** (gera a inscrição internacional/IRN, publica e notifica os designados); (3) **exame substantivo** independente por cada país designado (12/18 meses; recusa ou concessão tácita).
4. **Designação de países:** designar as Partes Contratantes desejadas; designação posterior possível a qualquer tempo.
5. **Prazos críticos:** transmitir à OMPI em **até 2 meses** para manter a data BR; responder inconsistências do INPI em **até 60 dias**.
6. **Dependência de 5 anos ("ataque central"):** o registro internacional **depende da base por 5 anos** — se a base cair (recusada, arquivada, cancelada, extinta, não renovada), o internacional é cancelado; cabe **transformação em pedidos nacionais em até 3 meses**, mantida a data original. Alertar o cliente expressamente.
7. **Custos:** **GRU 3004** ao INPI (em reais) + **taxas da OMPI em CHF** (básica 653 ou 903 em cores + taxas individuais/complementares por país) — usar a calculadora do eMadrid.
8. **Validação:** todo dispositivo/tratado citado passa por `validador-marcario`, cruzando com `tratados-cup-madri-trips.md`.
9. Atualizar `memoria-de-caso-marca` (pedido internacional encaminhado; bases apontadas; países designados; prazos de dependência e de manutenção da data).

## Entrega obrigatória final
- Roteiro/instrução do pedido internacional (elegibilidade, base(s) apontada(s) e escopo, países designados, etapas, MM2/eMadrid) + minuta dos campos-chave.
- GRU 3004 indicada + estimativa das taxas OMPI (CHF) com remissão à calculadora eMadrid.
- Alertas: escopo nunca mais amplo que a base; **dependência de 5 anos / ataque central** + transformação em 3 meses; prazo de 2 meses para manter a data BR.
- `memoria-de-caso-marca` atualizado + próximos passos e prazos.
- **Validação pela `suprema-corte-marcaria` (R1–R4) antes da entrega.**

## Guard
Nenhum dispositivo/tratado entra na orientação sem `validador-marcario`. **Base obrigatória; escopo internacional ≤ base, nunca maior.** Não omitir a dependência de 5 anos (ataque central) nem o prazo de 2 meses para preservar a data BR. Custos do INPI (GRU 3004) e da OMPI (CHF) sempre separados e explicados. Entrega só após `suprema-corte-marcaria`. Na dúvida sobre vigência/valor de taxa, bloquear e checar ao vivo (custos do INPI e da OMPI mudam).
