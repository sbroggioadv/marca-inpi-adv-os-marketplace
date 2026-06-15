---
name: marca-coletiva-certificacao
description: Monta o pedido de registro de MARCA COLETIVA (identifica produtos/servicos de membros de uma entidade — associacao, cooperativa, sindicato) ou de MARCA DE CERTIFICACAO (atesta conformidade a normas/qualidade) no INPI, incluindo o REGULAMENTO DE UTILIZACAO obrigatorio (LPI arts. 147-154). Use quando o operador disser "marca coletiva", "marca de certificacao", "selo de qualidade", "marca de associacao/cooperativa", "regulamento de utilizacao de marca", "marca de uma entidade", "/marca-coletiva".
---

# MARCA-COLETIVA-CERTIFICACAO

> Camada 2. Marcas com regime especial: pertencem a uma coletividade (coletiva) ou atestam conformidade (certificacao). O diferencial obrigatorio e o **regulamento de utilizacao**.

## Anexos obrigatorios (context/)
- `context/lpi-marcas-titulo-iii.md` (arts. 147 — regulamento da coletiva; 148 — conteudo do pedido de certificacao; 149-154 — alteracao, uso, extincao, caducidade da coletiva/certificacao; art. 123 — definicoes).
- `context/ncl-13-2026-classes.md` (classe NCL dos produtos/servicos abrangidos).

## Objetivo
Preparar o pedido correto conforme a natureza (coletiva ou certificacao), com o **regulamento de utilizacao** que a LPI exige, evitando exigencia/indeferimento por regulamento ausente ou incompleto.

## Quando ativar
Quando o titular nao e um agente economico isolado, mas uma **entidade** (coletiva) ou um **certificador** que atesta produtos/servicos de terceiros (certificacao).

## Metodologia
1. **Definir a natureza:**
   - **Coletiva (art. 147):** identifica produtos/servicos provenientes de **membros** de uma entidade (associacao, cooperativa, sindicato). Requerente = a entidade. Quem so legitima o uso e a entidade; o uso pelos membros independe de licenca, bastando autorizacao no regulamento (art. 150).
   - **Certificacao (art. 148):** atesta que o produto/servico **esta em conformidade** com normas/especificacoes tecnicas (qualidade, natureza, material, metodologia). Requerente nao pode ter interesse comercial/industrial direto no produto certificado.
2. **Elaborar o regulamento de utilizacao (peca central):**
   - **Coletiva (art. 147):** condicoes e proibicoes de uso da marca pelos membros.
   - **Certificacao (art. 148):** caracteristicas do produto/servico objeto de certificacao + medidas de controle que o titular se obriga a adotar.
3. **Especificar classe NCL:** indicar a(s) classe(s) dos produtos/servicos abrangidos (`context/ncl-13-2026-classes.md`).
4. **Cuidar do ciclo (arts. 149-154):** alteracao do regulamento deve ser comunicada ao INPI (149); regras de uso (150); causas extras de extincao/caducidade (151-153) — registrar para o acompanhamento; previsao do art. 154 (marcas ja usadas).
5. **Montar o pedido** com os dados de deposito (natureza coletiva/certificacao no e-Marcas) + regulamento anexo.

## Entrega obrigatoria final
- Pedido estruturado (natureza, requerente, classe NCL, marca) + **regulamento de utilizacao** conforme art. 147 (coletiva) ou art. 148 (certificacao).
- Checklist de anexos e de pontos de controle do ciclo (alteracao do regulamento, uso, caducidade especifica).
- Handoff para o `pedido-registro-inpi`/`custos-gru-inpi` (deposito e GRU por classe).

## Guard
Sem **regulamento de utilizacao** valido nao ha pedido — e o requisito que distingue essas marcas. Na **certificacao**, o requerente nao pode explorar comercialmente o produto que certifica (art. 148). Dispositivos so via `validador-marcario`. Especificacao por classe (cada classe = 1 processo). Gate final: `suprema-corte-marcaria`.
