---
name: custos-gru-inpi
description: Calcula as custas do INPI por classe, indica o código GRU correto para cada ato (depósito, oposição, exigência, recurso, PAN, caducidade, prorrogação) e ensina o passo a passo de emissão e pagamento no sistema GRU/e-Marcas do INPI. Use quando precisar orçar custas, emitir GRU ou orientar o protocolo, ou disser "quanto custa registrar a marca", "qual código da GRU", "custas do INPI", "emitir GRU", "GRU de oposição/recurso/PAN", "passo a passo do e-Marcas", "código 389 ou 394", "valor por classe", "tem desconto de 50%?".
---

# CUSTOS-GRU-INPI — Custas, código GRU e emissão

> Camada 1 (Fundação). Traduz atos marcários em custas por classe, código GRU correto e o passo a passo de emissão no INPI. Alimenta proposta, contrato e protocolo.

## Anexos obrigatorios (context/)
- `context/custos-gru-inpi.md` — tabela de retribuições/GRU por classe (referência vigente). **Confirmar o valor na emissão.**
- `context/procedimento-emarcas.md` — passo a passo oficial e-INPI → GRU → e-Marcas + códigos confirmados na Tabela.

## Objetivo
Entregar o cálculo das custas (por classe), o código GRU certo para cada ato e o roteiro de emissão/pagamento, separando custas (INPI) de honorários (escritório) de forma clara ao cliente.

## Quando ativar
- É preciso orçar/cobrar as custas de um registro ou de um ato (oposição, recurso, PAN, prorrogação).
- O operador vai emitir uma GRU ou precisa do código correto.
- A `proposta-comercial-marca` ou o `contrato-prestacao-servicos-marca` precisam dos valores.

## Metodologia
1. **Identificar o(s) ato(s)** a praticar e o nº de classes (ver `classificacao-ncl`).
2. **Mapear o código GRU** de cada ato (ver `context/custos-gru-inpi.md` e `procedimento-emarcas.md`):
   - Depósito **pré-aprovada** = **389** (R$ 880 / R$ 440 c/ desconto, por classe).
   - Depósito **livre preenchimento** = **394** (R$ 1.720 / R$ 860, por classe).
   - Oposição = **332** (R$ 520, por classe) · oposição restrita art. 124, XIX = 3022.
   - Cumprimento de exigência (exame formal) = 338.
   - **Recurso contra INDEFERIMENTO** = **3000** (R$ 700, por classe) — NÃO 333 (333 = recurso de marcas exceto indeferimento).
   - PAN — nulidade administrativa = **336** (R$ 850, por classe).
   - Caducidade = 337 · Prorrogação decenal = **374/375** (ordinário R$ 1.000 / extraordinário R$ 2.000, por classe).
   - 1º decênio + certificado = 372/373 = **ISENTO** desde 20/09/2025.
3. **Calcular custas:** soma das GRUs aplicáveis × nº de classes (cada classe = 1 processo, 1 GRU; multiclasse indisponível no e-Marcas).
4. **Aplicar desconto** quando cabível (50% para PF sem empresa do ramo, ME/EPP/MEI, ICTs, entidades sem fins lucrativos, órgãos públicos; 100% hipossuficiente/PcD nos atos elegíveis). O desconto NÃO incide em todos os códigos e depende do enquadramento declarado no e-INPI — sem regularidade, sai valor cheio.
5. **Roteiro de emissão (e-INPI → GRU → e-Marcas)** (ver `procedimento-emarcas.md`): cadastro no e-INPI → emitir GRU no módulo GRU (código + nº de classes "1") → **pagar ANTES** do peticionamento (boleto/Pix/cartão; guardar o "Nosso Número") → preencher o e-Marcas com o "Nosso Número" → enviar → anotar o número do pedido → acompanhar pela RPI (terças-feiras).
6. **Apresentar ao cliente** custas e honorários **separados e explicados**, lembrando que concessão/certificado hoje são gratuitos.

## Entrega obrigatoria final
- Tabela: ato · código GRU · valor cheio · valor c/ desconto · nº de classes · subtotal.
- Total de custas (INPI) destacado de honorários (escritório).
- Roteiro de emissão e pagamento (passos e-INPI/GRU/e-Marcas) + aviso de "confirmar valor vigente na emissão".

## Guard
Os valores em `context/custos-gru-inpi.md` são referência — **confirmar o valor vigente** na emissão (Tabela muda periodicamente). Nunca trocar 3000 por 333. Precificação sempre por classe. Qualquer dispositivo legal citado passa pelo `validador-marcario`; a entrega do caso fecha pela `suprema-corte-marcaria`.
