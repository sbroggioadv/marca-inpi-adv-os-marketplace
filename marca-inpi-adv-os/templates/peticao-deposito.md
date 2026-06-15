# Template — Petição/Dados do Depósito de Marca (e-Marcas)

> Esqueleto preenchido pela skill `pedido-registro-inpi`. Reúne os dados que o e-Marcas exige no formulário do pedido (após GRU paga). **1 formulário = 1 classe = 1 GRU.**
> Ver `context/procedimento-emarcas.md` para a mecânica do sistema.

---

## A. Pré-requisitos (antes de abrir o formulário)
- [ ] Cadastro no **e-INPI** (perfil Cliente ou Procurador).
- [ ] **GRU emitida e PAGA** — código **389** (especificação pré-aprovada, R$ 880/classe) **ou 394** (livre preenchimento, R$ 1.720/classe). Total de classes na GRU = **1**.
- [ ] Enquadramento de desconto declarado no cadastro (ME/EPP/MEI/PF → 50%), se aplicável.
- [ ] "Nosso Número" da GRU em mãos.

## B. Identificação
- **Requerente/Titular:** <nome ou razão social> · <CPF/CNPJ> · endereço.
- **Procurador (se houver):** <advogado> · OAB · procuração anexada (obrigatória no peticionamento por procurador).
- Cotitulares (se houver): todos cadastrados no e-INPI.

## C. A marca
- **Natureza:** ( ) de produto/serviço ( ) coletiva ( ) de certificação.
- **Forma de apresentação:** ( ) nominativa ( ) mista ( ) figurativa ( ) tridimensional ( ) de posição.
- **Elemento nominativo:** <texto> — obrigatório se nominativa ou mista.
- **Imagem** (obrigatória se mista/figurativa/3D/posição): JPG, **mín. 945×945 px (8×8 cm), 300 dpi, máx 2 MB, RGB**; imagem colorida = reivindicação de cores; 3D/posição exigem vistas adicionais.
  > Atenção: havendo divergência texto × imagem, **prevalece a imagem**. A marca não pode ser alterada após o depósito.

## D. Especificação — UMA classe NCL
- **Classe NCL:** <nº> (uma só por pedido — multiclasse indisponível no e-Marcas).
- **Itens:** <listar itens da especificação>.
  - Se **389**: itens da lista **pré-aprovada** do INPI (menor risco de exigência).
  - Se **394**: itens de **livre preenchimento** (maior risco de exigência) — cada item deve pertencer à mesma classe, não ser vago/genérico, e refletir a atividade real do requerente.
- A especificação **só pode ser restringida** depois do depósito, nunca ampliada.

## E. Checagem de proibições (art. 124 LPI)
Antes de enviar, conferir que o sinal não incide nas vedações do art. 124 (genérico/descritivo/de uso comum para o produto; sinal enganoso; reprodução/imitação de marca de terceiro no mesmo ramo; brasão/bandeira oficial; etc.). Ver `context/lpi-marcas-titulo-iii.md`. Em risco → parar e acionar `parecer-marcario`.

## F. Envio e protocolo
- Anexos obrigatórios (procuração, vistas) — o e-Marcas bloqueia o envio se ausentes.
- Enviar formulário → anotar o **número do pedido** (recibo).
- Acompanhamento **oficial**: **RPI** (terças-feiras) — início dos prazos legais. Registrar no `memoria-de-caso-marca`.

## G. Repetição por classe
Para cada classe adicional, repetir A→F (nova GRU, novo formulário, novo número de processo).
