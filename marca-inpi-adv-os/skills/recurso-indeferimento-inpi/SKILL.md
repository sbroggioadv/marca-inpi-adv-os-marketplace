---
name: recurso-indeferimento-inpi
description: Redige recurso administrativo contra o indeferimento de pedido de registro de marca pelo INPI, com fundamento no art. 212 da LPI. Use quando o operador disser "minha marca foi indeferida", "fui indeferido no INPI", "recorrer do indeferimento", "recurso contra indeferimento de marca", "o INPI negou meu registro", "quero recorrer da decisão do examinador", ou descrever que o pedido foi indeferido (geralmente por art. 124, falta de distintividade ou colidência) e cabe recurso ao Presidente do INPI. ATENÇÃO À GRU — recurso contra indeferimento usa a GRU 3000 (R$ 700), NÃO a 333. Prazo de 60 dias da publicação do indeferimento (art. 212).
---

# RECURSO CONTRA INDEFERIMENTO (art. 212 LPI)

> Camada 3 — Contencioso administrativo INPI. Acionada pelo `marcas-master` quando o pedido de marca do cliente foi **indeferido** e cabe recurso administrativo ao Presidente do INPI.

## Anexos obrigatórios (context/)
- `context/lpi-marcas-titulo-iii.md` — art. 124 (motivos de indeferibilidade, para rebater o fundamento da decisão); art. 122-123 (registrabilidade e conceito de marca); art. 160 (decisão de deferimento/indeferimento).
- `context/lpi-9279-96.md` — art. 212 (recurso, prazo 60 dias; efeitos); arts. 212-220 (disposições gerais sobre recursos administrativos no INPI).
- `context/custos-gru-inpi.md` — **GRU 3000 — recurso contra INDEFERIMENTO do pedido (R$ 700 por classe). NÃO confundir com a 333** (recurso de marcas demais hipóteses).
- `context/jurisprudencia-marcaria.md` — distintividade adquirida (secondary meaning), teoria da distância, sob demanda.

## Objetivo
Reverter o indeferimento, demonstrando que o pedido é registrável e que o fundamento da decisão (em regra art. 124 ou ausência de distintividade) não se sustenta, obtendo o deferimento em grau de recurso.

## Quando ativar
- O pedido de marca do cliente foi indeferido pelo INPI (decisão publicada na RPI).
- O prazo de 60 dias da publicação do indeferimento ainda está aberto (art. 212).

## Metodologia
1. **Estado do caso** via `memoria-de-caso-marca`: pedido (nº, classe, sinal), **fundamento exato do indeferimento** (inciso do art. 124, falta de distintividade, colidência com anterioridade citada), data da publicação.
2. **Tempestividade:** confirmar os **60 dias** da publicação do indeferimento (art. 212).
3. **Atacar o fundamento:** rebater especificamente o motivo da decisão — se art. 124 XIX/colidência, sustentar diferença de sinais e/ou ramo (`ncl-13-2026-classes.md`); se art. 124 VI/descritividade, sustentar suficiente forma distintiva ou distintividade adquirida; se anterioridade citada, demonstrar convivência/especialidade.
4. **Novos elementos:** apresentar provas e argumentos que reforcem a registrabilidade (uso, distintividade adquirida, coexistência, eventual carta de consentimento).
5. **Custas — ponto crítico:** indicar **GRU 3000** (recurso contra indeferimento), **nunca a 333**. Uma GRU por classe (`metodologia-marcaria.md`).
6. **Validação:** todo dispositivo/jurisprudência passa por `validador-marcario`.
7. Atualizar `memoria-de-caso-marca` (recurso protocolado; próximo passo: julgamento pelo Presidente do INPI — se mantido o indeferimento, avaliar via judicial → Camada 4 `acao-judicial-concessao-registro`, anulando o ato + novo exame, sem o Judiciário impor prazo nem substituir o INPI).

## Entrega obrigatória final
- Peça de recurso (qualificação, tempestividade, síntese do indeferimento, razões recursais atacando cada fundamento, provas, pedido de reforma e deferimento).
- **GRU 3000** indicada por classe + alerta explícito de não usar a 333.
- `memoria-de-caso-marca` atualizado + próximo passo (julgamento; eventual via judicial).
- **Validação pela `suprema-corte-marcaria` (R1–R4) antes da entrega.**

## Guard
Nenhum dispositivo/súmula/acórdão entra na peça sem `validador-marcario`. **GRU 3000, não 333** — erro recorrente e custoso. Conferir prazo de 60 dias (art. 212). "Forçar registro" na via judicial = anular o indeferimento + determinar novo exame (o Judiciário não impõe prazo nem substitui o INPI). Entrega só após `suprema-corte-marcaria`. Na dúvida sobre vigência/valor de GRU, bloquear e checar ao vivo.
