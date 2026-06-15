---
name: busca-anterioridade
description: "Pesquisa de anterioridade marcaria na base do INPI (BuscaWeb) — verifica se ja existe marca igual ou semelhante que impeça o registro, nas classes pretendidas. HIBRIDO: tenta a busca viva em busca.inpi.gov.br via firecrawl; se o INPI bloquear (captcha/sessao/limite), cai para o modo GUIADO, montando termos, radicais e classes + passo a passo para a equipe executar manualmente e colar o resultado. Devolve relatorio de colidencia/disponibilidade. Use no inicio do fluxo de registro, antes de propor classes, ou quando o operador disser \"busca de anterioridade\", \"essa marca esta disponivel?\", \"pesquisa no INPI\", \"tem marca igual?\", \"colidencia\", \"/anterioridade\"."
---

# BUSCA-ANTERIORIDADE

> Camada 2. Primeiro passo do fluxo comercial: sem disponibilidade, nao adianta orcar. Resultado da BuscaWeb e **meramente indicativo** — o exame de registrabilidade e do INPI.

## Anexos obrigatorios (context/)
- `context/procedimento-emarcas.md` (Passo 0 — pesquisa por "Radical"; criterio grafia + estrutura + fonetica; protecao restrita ao segmento/classe).
- `context/metodologia-marcaria.md` (lugar deste passo no fluxo).

## Objetivo
Estimar a **disponibilidade** do sinal e mapear **colidencias** (marcas anteriores iguais/semelhantes na mesma classe ou ramo) antes de qualquer custo, reduzindo risco de indeferimento por reproducao/imitacao (art. 124, XIX, LPI).

## Quando ativar
No comeco do fluxo de registro, antes do `diagnostico`/`planejamento`, e sempre que o operador questionar se a marca esta livre.

## Metodologia
1. **Definir os parametros de busca:**
   - **Radical/nucleo** do sinal (o INPI recomenda busca por "Radical" — semelhanca/aproximacao, nao so exato).
   - Variacoes de **grafia, estrutura e fonetica** (ex.: "Phoenix"/"Fenix"/"Fenyx").
   - **Classes** pretendidas (do diagnostico/planejamento) — a protecao e, em regra, restrita ao segmento.
2. **Modo VIVO (tentar primeiro):** acessar `https://busca.inpi.gov.br/` via `firecrawl` (scrape/interact). Buscar por radical e por marca exata, filtrando por classe. Coletar: numero do processo, marca, titular, classe, situacao (deposito/registro/extinto), apresentacao.
3. **Fallback GUIADO (se bloquear):** se houver captcha, exigencia de sessao/login, limite ou retorno vazio suspeito, **nao inventar resultado** — montar para a equipe:
   - a lista de **termos e radicais** a pesquisar (exato + variacoes foneticas/graficas);
   - as **classes** a filtrar;
   - o **passo a passo** na BuscaWeb (login e-INPI > Marca > pesquisa por radical > filtra classe);
   - um **modelo de planilha** para a equipe colar os achados (Marca | Titular | Processo | Classe | Situacao | Apresentacao). Ao receber o colado, continuar a analise.
4. **Analisar colidencia:** para cada achado relevante, avaliar grau de semelhanca (alto/medio/baixo), identidade/afinidade de classe e ramo, e situacao (registro vigente bloqueia; pedido pendente e risco; extinto/arquivado nao bloqueia mas observar caducidade).
5. **Classificar a disponibilidade:** Livre · Risco baixo · Risco alto · Indisponivel (anterioridade impeditiva), com recomendacao (seguir / ajustar sinal / mudar classe / consultar `parecer-marcario`).

## Entrega obrigatoria final
- **Relatorio de colidencia/disponibilidade**: parametros buscados, modo usado (vivo/guiado), tabela de anterioridades encontradas e classificacao final (Livre/Risco/Indisponivel) com recomendacao.
- Se modo guiado: o kit completo (termos + classes + passo a passo + planilha) entregue a equipe.
- Aviso fixo: resultado da BuscaWeb e **indicativo**; a decisao de registrabilidade e do INPI.

## Guard
Nunca afirmar "disponivel" como garantia — so estimativa indicativa. Se a busca viva falhar/bloquear, **declarar** o bloqueio e usar o modo guiado; jamais fabricar processos, titulares ou situacoes. Anterioridade impeditiva real → recomendar ajuste ANTES de orcar (nao empurrar para a proposta um sinal com risco alto sem alertar).
