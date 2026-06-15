---
name: contrato-prestacao-servicos-marca
description: Gera o contrato de prestacao de servicos advocaticios para registro de marca — escopo = pesquisa + deposito + acompanhamento; preve valores adicionais por classe em caso de exigencia, manifestacao a oposicao, recurso (indeferimento) ou PAN; dimensionado por numero de classes (cada classe = 1 processo). Use depois do cliente aprovar a proposta, ou quando o operador disser "gera o contrato de marca", "minuta do contrato de registro", "contrato de honorarios da marca", "formaliza o cliente do registro", "/contrato-marca".
---

# CONTRATO-PRESTACAO-SERVICOS-MARCA

> Camada 2. Formaliza a relacao depois da proposta aceita. Dimensiona honorarios e responsabilidades **por classe** e blinda o escritorio contra intercorrencias nao previstas (exigencia/oposicao/indeferimento).

## Anexos obrigatorios (context/)
- `context/custos-gru-inpi.md` (custas adicionais por classe: exigencia 338, manifestacao 339, recurso 3000, PAN 336).
- `context/metodologia-marcaria.md` (regra: por classe; custas x honorarios separados).
- Template: `templates/contrato-registro-marca.md`.
- Perfil: `marca-inpi/perfil.md` (CONTRATADO, cidade/foro, honorarios; valores vem da proposta aprovada).

## Objetivo
Produzir uma minuta de contrato clara e exequivel: escopo fechado (pesquisa + deposito + acompanhamento), valores por classe, e regra explicita para os custos adicionais quando o INPI exige, ha oposicao ou o pedido e indeferido.

## Quando ativar
Apos o cliente aprovar a `proposta-comercial-marca`. Insumo direto: a proposta (valores, classes) + `perfil.md`.

## Metodologia
1. **Carregar dados:** CONTRATADO (do `perfil.md`), CONTRATANTE (cliente), marca + apresentacao, **classes** e valores (da proposta).
2. **Objeto por classe:** descrever a marca e listar as classes; afirmar que cada classe e **processo autonomo**.
3. **Escopo incluido (cl. 2):** pesquisa de anterioridade/viabilidade + deposito no e-Marcas + acompanhamento na RPI ate a decisao de 1a instancia.
4. **Escopo NAO incluido / valores adicionais (cl. 3):** por classe e orcado a parte — cumprimento de exigencia (GRU 338), manifestacao a oposicao (339), **recurso contra indeferimento (GRU 3000)**, PAN (336), acoes judiciais. Anexar tabela de honorarios adicionais por intercorrencia.
5. **Valores (cl. 4):** honorarios por classe × nº classes (forma de pagamento) **separados** das custas/GRU (pagas ao INPI). Registrar isencao do 1o decenio.
6. **Obrigacoes e riscos (cl. 5-7):** documentos do cliente (CNPJ/contrato/logo ≥945px), declaracao correta de enquadramento (desconto); diligencia/etica do escritorio; **sem garantia de deferimento** (art. 124 LPI); vedada promessa de resultado (Etica OAB); fluxo de comunicacao em exigencia/oposicao/indeferimento.
7. **Vigencia, rescisao, foro (cl. 8):** honorarios proporcionais ao trabalho na rescisao (CPC 22 §2o); foro = cidade do perfil.
8. **Renderizar** preenchendo `templates/contrato-registro-marca.md`.

## Entrega obrigatoria final
- Minuta de contrato completa (partes, objeto por classe, escopo incluido/excluido, valores separados, obrigacoes, clausula de exigencia/oposicao/indeferimento, vigencia/foro), pronta para assinatura.
- Resumo dos valores e dos pontos de atencao para o operador revisar com o cliente.

## Guard
Honorarios e custas **separados**; valores por classe. **Nunca prometer resultado/deferimento** (Codigo de Etica OAB) — o contrato deve dizer expressamente que o registro depende do exame do INPI. Custos adicionais (exigencia/oposicao/recurso/PAN) tem de estar previstos por classe, com o codigo de GRU correto (recurso de indeferimento = **3000**, nao 333). Foro e dados do CONTRATADO vem do `perfil.md`.
