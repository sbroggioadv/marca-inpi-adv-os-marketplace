---
name: proposta-comercial-marca
description: Gera o orcamento do registro de marca POR CLASSE (honorarios do escritorio + custas GRU do INPI, SEPARADOS e explicados ao cliente final) e o renderiza num PDF/HTML bonito na PALETA do escritorio (lida de marca-inpi/perfil.md). Serve tambem como resumo/apresentacao do caso (marca, atividades, busca, classes). Use depois do planejamento das classes, antes do contrato, ou quando o operador disser "monta a proposta", "orcamento do registro", "quanto custa registrar", "proposta comercial de marca", "gera o PDF da proposta", "/proposta-marca".
---

# PROPOSTA-COMERCIAL-MARCA

> Camada 2. Peca comercial que o cliente assina antes de seguir. Mostra de forma clara o que ele paga ao escritorio (honorarios) e o que paga ao INPI (custas/GRU) — separados, por classe.

## Anexos obrigatorios (context/)
- `context/custos-gru-inpi.md` (valores de GRU por classe: 389 R$880, 394 R$1.720; desconto 50%; 1o decenio isento).
- `context/metodologia-marcaria.md` (regra: custas e honorarios separados e explicados; por classe).
- Template: `templates/proposta-comercial.md`.
- Perfil: `marca-inpi/perfil.md` (identidade, paleta de cores, logo, honorarios-base por classe, enquadramento de desconto).

## Objetivo
Transformar o portfolio aprovado num **orcamento transparente por classe** e numa **apresentacao do caso** — em PDF/HTML na identidade visual do escritorio — que o cliente entenda e aprove.

## Quando ativar
Depois do `planejamento-portfolio-marca` (classes aprovadas), antes do `contrato-prestacao-servicos-marca`.

## Metodologia
1. **Ler o perfil:** `marca-inpi/perfil.md` (cor primaria/secundaria, logo, nome/OAB/cidade/e-mail, honorarios-base por classe, se atende ME/EPP/MEI/PF com desconto). Se faltar perfil, orientar `/start-marca-inpi`.
2. **Montar o resumo do caso:** marca + apresentacao, titular + enquadramento, atividades (do diagnostico), resultado da busca (do `busca-anterioridade`), classes + justificativas (do planejamento).
3. **Calcular POR CLASSE:**
   - **Custas (GRU)** = por classe, codigo **389** (pre-aprovada, R$ 880) ou **394** (livre, R$ 1.720). Aplicar **desconto 50%** se o cliente for ME/EPP/MEI/PF elegivel (R$ 440 / R$ 860). Confirmar valor vigente na emissao.
   - **Honorarios** = valor-base do perfil por classe × nº de classes.
   - **Nunca somar custas com honorarios numa unica linha** — sempre duas colunas/subtotais.
4. **Totalizar:** subtotal custas, subtotal honorarios, total geral, forma de pagamento. Lembrar que 1o decenio/certificado e **isento** hoje.
5. **Renderizar:** preencher `templates/proposta-comercial.md` e gerar **PDF/HTML** na paleta do perfil (cabecalho com logo + cores). Tabela de classes legivel, disclaimers fixos.
6. **Escopo e validade:** deixar claro o que inclui (pesquisa + deposito + acompanhamento) e o que e adicional (exigencia/oposicao/recurso) — alinhado ao contrato. Definir validade da proposta.

## Entrega obrigatoria final
- Proposta em **PDF/HTML** na paleta do escritorio: resumo do caso + tabela de classes (custas e honorarios separados) + totalizacao + escopo + validade + aceite.
- Resumo de valores em texto para o operador conferir.
- Apos aceite do cliente, handoff para o `contrato-prestacao-servicos-marca`.

## Guard
**Custas (GRU) e honorarios sempre separados e explicados** — misturar reprova no gate R4. Precificar **por classe** (cada classe = 1 processo). Valores de GRU vem de `context/custos-gru-inpi.md` e devem ser **confirmados na emissao** (a tabela muda). Honorarios e paleta vem do `perfil.md` — nunca inventar valor do escritorio. Nao prometer deferimento nem prazo do INPI.
