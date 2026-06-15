# Metodologia Marcária — Mapa de Uso do Plugin

> Anexo central. Define como as skills se articulam, qual anexo cada uma lê, o fluxo comercial e as regras de ouro. O `marcas-master` lê este arquivo primeiro.

## Arquitetura (4 camadas + QA)
- **Camada 0 — Orquestração/QA:** `marcas-master`, `marca-inpi-onboarding`, `triagem-marca`, `memoria-de-caso-marca`, `estilo-marcario`, `suprema-corte-marcaria`.
- **Camada 1 — Fundação:** `base-legal-marcaria`, `classificacao-ncl`, `jurisprudencia-marcaria`, `validador-marcario`, `custos-gru-inpi`.
- **Camada 2 — Consultivo/Comercial:** `diagnostico-marca`, `busca-anterioridade`, `planejamento-portfolio-marca`, `proposta-comercial-marca`, `contrato-prestacao-servicos-marca`, `pedido-registro-inpi`, `notificacao-extrajudicial-marcaria`, `parecer-marcario`, `marca-coletiva-certificacao`, `indicacao-geografica`.
- **Camada 3 — Administrativo INPI:** `oposicao-registro`, `manifestacao-oposicao`, `cumprimento-exigencia`, `recurso-indeferimento-inpi`, `nulidade-administrativa-pan`, `caducidade-marca`, `marca-alto-renome-e-notoria`, `marca-internacional-madri`, `ciclo-vida-marca`.
- **Camada 4 — Judicial:** `acao-abstencao-uso-marca`, `acao-concorrencia-desleal`, `acao-nulidade-registro`, `acao-judicial-concessao-registro`, `contestacao-marcaria`, `recursos-judiciais-marcarios`, `liquidacao-danos-marcarios`.

## Anexos de `context/` (o que cada um contém)
| Anexo | Conteúdo |
|---|---|
| `lpi-9279-96.md` | Lei 9.279/96 integral |
| `lpi-marcas-titulo-iii.md` | Recorte das marcas (arts. 122–182) |
| `ncl-13-2026-classes.md` | NCL 13/2026 — 45 caputs de classe + regras |
| `tratados-cup-madri-trips.md` | CUP + Protocolo de Madri + TRIPS |
| `custos-gru-inpi.md` | Tabela de custas/GRU por classe |
| `procedimento-emarcas.md` | Passo a passo do depósito + GRU |
| `jurisprudencia-marcaria.md` | Leading cases STJ/TRF2 + súmulas |

**NCL completa (itens):** a lista de milhares de itens está no PDF oficial, não copiada inline →
`https://www.gov.br/inpi/pt-br/servicos/marcas/classificacao-marcas/Lista_Nice_NCL_13_2026.pdf`

## Fluxo comercial (conduzido pelo `marcas-master`)
```
busca-anterioridade (disponibilidade)
  → diagnostico-marca (lê CNPJ/contrato/site → atividades)
  → planejamento-portfolio-marca (classes obrigatórias + extras, cada uma justificada)
  → [usuário aprova as classes]
  → proposta-comercial-marca (orçamento POR CLASSE: honorários + custas GRU separados; PDF na paleta do escritório)
  → [cliente aprova]
  → contrato-prestacao-servicos-marca (pesquisa + depósito + acompanhamento + valores de manifestação/indeferimento)
  → custos-gru-inpi (emite as GRUs + passo a passo no e-Marcas)
  → pedido-registro-inpi (confecção do depósito)
  → acompanhamento (administrativo/judicial conforme intercorrências)
```

## Regras de ouro
1. **1 classe = 1 processo administrativo** → honorários e custas por classe.
2. **Competência:** nulidade de registro → Justiça Federal (INPI, art. 175); abstenção/concorrência desleal entre particulares → Justiça Estadual (STJ Tema 950).
3. **Recurso contra indeferimento** = GRU **3000** (não 333).
4. **"Forçar registro":** pedir anulação do indeferimento + **determinação de novo exame** (STJ REsp 1.787.676); o Judiciário não impõe prazo nem substitui o INPI (TRF2).
5. **Gate final:** toda entrega passa pela `suprema-corte-marcaria` (R1–R4).
6. **Anti-alucinação:** citações só via `validador-marcario`.
