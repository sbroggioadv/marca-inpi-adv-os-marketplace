---
name: pedido-registro-inpi
description: Monta o deposito do pedido de registro de marca no e-Marcas — define natureza e forma de apresentacao (nominativa/mista/figurativa/tridimensional/de posicao), a especificacao de produtos/servicos por UMA classe NCL, e a GRU correta (389 pre-aprovada ou 394 livre, por classe, paga ANTES de peticionar). Checa as proibicoes do art. 124 LPI antes de enviar. Use depois do contrato assinado e das GRUs, ou quando o operador disser "fazer o deposito", "registrar a marca no INPI", "monta o pedido no e-Marcas", "depositar a marca", "preencher o e-Marcas", "/deposito-marca".
---

# PEDIDO-REGISTRO-INPI

> Camada 2. Confeccao do deposito. Etapa onde a estrategia vira processo no INPI. **1 formulario = 1 classe = 1 GRU.**

## Anexos obrigatorios (context/)
- `context/procedimento-emarcas.md` (passo a passo e-INPI/GRU/e-Marcas; imagem ≥945×945; GRU paga ANTES; especificacao por 1 classe; acompanhamento RPI).
- `context/ncl-13-2026-classes.md` (classe correta + 389 pre-aprovada x 394 livre).
- `context/custos-gru-inpi.md` (codigos 389/394, desconto 50%, isencao 372/373).
- `context/lpi-marcas-titulo-iii.md` (proibicoes do art. 124 — checagem de registrabilidade).
- Template: `templates/peticao-deposito.md`.

## Objetivo
Preparar, **por classe**, todos os dados que o e-Marcas exige para o deposito, com a GRU certa e a checagem do art. 124 feita antes do envio — evitando exigencia, indeferimento ou pedido inexistente.

## Quando ativar
Depois do `contrato-prestacao-servicos-marca` assinado e da emissao/pagamento da GRU (via `custos-gru-inpi`). Repetir para cada classe do portfolio.

## Metodologia
1. **Conferir pre-requisitos:** cadastro e-INPI (Cliente/Procurador); **GRU emitida e PAGA** (codigo 389 ou 394; total de classes = 1); enquadramento de desconto declarado; "Nosso Numero" em maos.
2. **Definir a marca:** natureza (produto/servico, coletiva ou certificacao) + forma de apresentacao (nominativa/mista/figurativa/3D/posicao). Para mista/figurativa/3D/posicao: imagem **JPG ≥ 945×945 px (8×8 cm, 300 dpi, ≤2 MB, RGB)**; imagem colorida = reivindicacao de cores; 3D/posicao exigem vistas adicionais. Elemento nominativo obrigatorio se nominativa/mista.
3. **Especificacao por 1 classe:** escolher **uma** classe NCL (multiclasse indisponivel) e os itens. **389** = itens da lista pre-aprovada (menor risco). **394** = livre preenchimento (maior risco; item nao vago, na mesma classe, refletindo a atividade real). Lembrar: so se pode **restringir** depois, nunca ampliar.
4. **Checar proibicoes do art. 124 (LPI):** confirmar que o sinal nao e generico/descritivo/de uso comum para o produto, nao e enganoso, nao reproduz/imita marca de terceiro no mesmo ramo (cruzar com o resultado da `busca-anterioridade`), nao usa simbolo oficial vedado, etc. (`context/lpi-marcas-titulo-iii.md`). Em risco → **parar** e acionar `parecer-marcario`.
5. **Montar o pacote** com `templates/peticao-deposito.md`: identificacao, marca, imagem, especificacao, anexos (procuracao/vistas).
6. **Orientar envio:** no e-Marcas, inserir o "Nosso Numero", conferir dados migrados, anexar obrigatorios, enviar, anotar o **numero do pedido**. Acompanhamento **oficial** = RPI (tercas) — registrar no `memoria-de-caso-marca`.
7. **Repetir por classe** (nova GRU, novo formulario, novo processo).

## Entrega obrigatoria final
- Ficha de deposito por classe (natureza/forma, imagem conforme specs, especificacao, GRU/codigo) pronta para preencher o e-Marcas, via `templates/peticao-deposito.md`.
- Resultado da checagem do art. 124 (OK ou risco → `parecer-marcario`).
- Numero do pedido a anotar + lembrete de acompanhamento na RPI + atualizacao do `memoria-de-caso-marca`.

## Guard
**GRU paga ANTES do peticionamento** — pagar depois torna o pedido inexistente. Uma classe por formulario; codigo 389/394 correto; valor confirmado na emissao. Imagem fora das specs (≥945×945) = risco de exigencia. A marca **nao pode ser alterada** apos o deposito. Checagem do art. 124 e obrigatoria antes do envio; na duvida de registrabilidade, acionar `parecer-marcario` em vez de depositar no escuro.
