---
name: nulidade-administrativa-pan
description: Conduz o Processo Administrativo de Nulidade (PAN) de registro de marca já concedido pelo INPI, com fundamento nos arts. 168 a 172 da LPI — tanto para requerer a nulidade (cliente atacante) quanto para defender o registro (cliente titular intimado). Use quando o operador disser "PAN", "processo administrativo de nulidade", "nulidade administrativa de marca", "quero anular um registro de marca", "registro foi concedido indevidamente", "fui intimado de um PAN", "defender meu registro de nulidade", ou descrever registro concedido em desacordo com a LPI. Prazo para instaurar — 180 dias da concessão (art. 169). Titular intimado — 60 dias (art. 170). GRU 336 (R$ 850 por classe). Atenção — PAN é via administrativa; ação judicial de nulidade prescreve em 5 anos (art. 174) e corre na Justiça Federal (art. 175).
---

# NULIDADE ADMINISTRATIVA — PAN (arts. 168-172 LPI)

> Camada 3 — Contencioso administrativo INPI. Acionada pelo `marcas-master` para atacar (ou defender) registro de marca **já concedido** pela via administrativa do PAN.

## Anexos obrigatórios (context/)
- `context/lpi-marcas-titulo-iii.md` — art. 168 (nulidade quando concedido com infringência à Lei); art. 169 (instauração de ofício ou por legítimo interesse, prazo 180 dias da expedição do certificado); art. 170 (titular intimado, prazo 60 dias); art. 171 (decisão do Presidente do INPI, encerra a instância); art. 172 (prossegue ainda que extinto o registro); art. 124 (fundamentos de nulidade).
- `context/custos-gru-inpi.md` — GRU 336 (PAN — nulidade administrativa, R$ 850 por classe).
- `context/jurisprudencia-marcaria.md` — colidência, má-fé, anterioridade, sob demanda.

## Objetivo
- **Atacante:** requerer a nulidade administrativa de registro concedido em infração à LPI, dentro do prazo de instauração.
- **Defensor:** manifestar-se para preservar o registro do cliente quando intimado de PAN.

## Quando ativar
- Registro de marca já foi concedido e o cliente tem legítimo interesse em anulá-lo (colidência com direito anterior, má-fé, vedação do art. 124).
- O cliente é titular de registro e foi **intimado** de PAN instaurado por terceiro ou de ofício.

## Metodologia
1. **Estado do caso** via `memoria-de-caso-marca`: registro atacado (nº, classe, titular, data da concessão), fundamento da nulidade, legítimo interesse do cliente; ou, na defesa, data da intimação.
2. **Cabimento e prazo:**
   - **Instaurar PAN:** **180 dias contados da expedição do certificado** de registro (art. 169). Fora desse prazo → o PAN não cabe; resta a **ação judicial de nulidade** (prescreve em 5 anos da concessão, art. 174; Justiça Federal, art. 175 → Camada 4).
   - **Defesa do titular:** **60 dias da intimação** (art. 170).
3. **Fundamentos (atacante):** indicar o(s) dispositivo(s) violado(s) na concessão — em regra art. 124 (XIX colidência, V nome empresarial, XXIII má-fé), arts. 125/126, ou outra infração à Lei (art. 168).
4. **Teses (defensor):** ausência de infração, distintividade, especialidade, convivência, validade da concessão, eventual decadência do direito de instaurar (180 dias).
5. **Instância única administrativa:** lembrar que a decisão do Presidente do INPI **encerra a instância administrativa** (art. 171) e que o processo prossegue ainda que extinto o registro (art. 172).
6. **Custas:** indicar **GRU 336** por classe.
7. **Validação:** todo dispositivo/jurisprudência passa por `validador-marcario`.
8. Atualizar `memoria-de-caso-marca` (PAN instaurado/respondido; próximo passo: decisão do Presidente; eventual via judicial).

## Entrega obrigatória final
- Peça de requerimento de PAN **ou** de manifestação do titular (qualificação, legítimo interesse, tempestividade, fundamentos por dispositivo, pedido de nulidade ou de manutenção).
- GRU 336 indicada por classe (no requerimento).
- Alerta de prazos (180 dias art. 169 instaurar · 60 dias art. 170 defesa) e da alternativa judicial (5 anos art. 174 · Justiça Federal art. 175) quando o prazo administrativo já tiver escoado.
- `memoria-de-caso-marca` atualizado + próximo passo.
- **Validação pela `suprema-corte-marcaria` (R1–R4) antes da entrega.**

## Guard
Nenhum dispositivo/súmula/acórdão entra na peça sem `validador-marcario`. Não confundir prazo de instauração do PAN (180 dias, art. 169) com prescrição da ação judicial (5 anos, art. 174). Nulidade judicial = Justiça Federal (INPI no polo, art. 175). Custas por classe (GRU 336). Entrega só após `suprema-corte-marcaria`. Na dúvida sobre vigência/valor de GRU, bloquear e checar ao vivo.
