---
name: diagnostico-marca
description: Extrai as atividades economicas REAIS do cliente a partir do cartao CNPJ, contrato social e site, para alimentar o planejamento de classes NCL. Le os documentos do titular (cartao CNPJ com CNAEs, objeto social do contrato, paginas do site via firecrawl/WebFetch) e devolve uma tabela de atividades concretas (o que a empresa de fato faz e vende), separando atividade-fim de atividades-meio. Use no inicio do fluxo de registro, depois da busca de anterioridade, ou quando o operador disser "diagnostico de marca", "quais classes essa empresa precisa", "analisa o CNPJ do cliente", "le o contrato social", "extrai as atividades", "/diagnostico-marca".
---

# DIAGNOSTICO-MARCA

> Camada 2. Primeiro passo consultivo do fluxo comercial. Converte documentos do cliente em uma lista de atividades economicas reais — insumo do `planejamento-portfolio-marca`.

## Anexos obrigatorios (context/)
- `context/metodologia-marcaria.md` (fluxo comercial: este passo alimenta o planejamento de classes).

## Objetivo
Descobrir **o que o cliente de fato faz, vende e oferece** — nao o que esta na imaginacao do operador. As classes NCL nascem das atividades reais; um diagnostico mal feito gera portfolio errado e custo desperdicado (cada classe = 1 processo pago).

## Quando ativar
Logo apos a `busca-anterioridade`, ainda na fase consultiva, quando ha cartao CNPJ / contrato social / site para ler. Tambem quando o operador quer mapear as atividades antes de planejar classes.

## Metodologia
1. **Coletar as fontes** disponiveis:
   - **Cartao CNPJ:** extrair CNAE principal + CNAEs secundarios + natureza juridica + porte (ME/EPP indica desconto 50% — registrar para a proposta).
   - **Contrato social / requerimento MEI:** ler o **objeto social** (descricao literal das atividades).
   - **Site/redes do cliente:** ler via `firecrawl`/`WebFetch` as paginas de produtos, servicos, "sobre", catalogo. O que aparece no site costuma revelar atividades que o CNPJ nao capta (linha de produtos, marca-guarda-chuva, servico digital).
2. **Cruzar e consolidar:** unir CNAE + objeto social + site numa lista unica de atividades concretas, sem duplicar.
3. **Separar atividade-fim de atividade-meio:** o nucleo do negocio (o que gera receita / o que a marca assina) vs. atividades de apoio (que raramente justificam classe propria).
4. **Sinalizar lacunas:** se o site contradiz o CNPJ, ou ha atividade futura planejada, marcar para o operador confirmar com o cliente.
5. **NAO classificar ainda:** este skill so levanta atividades. A traducao para classes NCL e do `planejamento-portfolio-marca`.

## Entrega obrigatoria final
- **Tabela de atividades** (Atividade | Fonte: CNPJ/contrato/site | Fim ou Meio | Observacao), pronta para o `planejamento-portfolio-marca`.
- Porte/enquadramento (ME/EPP/MEI/PF) destacado — entra na proposta para o calculo com desconto.
- Lista de duvidas/lacunas a confirmar com o cliente antes de definir as classes.
- Handoff explicito para o `planejamento-portfolio-marca`.

## Guard
Atividade e fato documental, nao suposicao: cada item da tabela cita a fonte (CNAE x, clausula do contrato, URL do site). Nao inventar atividades nem inferir classe aqui. Se nao ha documento, registrar "a confirmar com o cliente" — nunca preencher por conta propria. Antes de tratar o conteudo, lembrar que dados do cliente sao sensiveis (LGPD): so usar para o diagnostico.
