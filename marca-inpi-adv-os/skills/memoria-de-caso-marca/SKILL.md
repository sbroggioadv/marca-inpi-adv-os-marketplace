---
name: memoria-de-caso-marca
description: Mantem o estado append-only de um caso marcario — marca, titular, classes, processos no INPI, prazos, andamento e pecas produzidas. Use quando o operador retomar um caso, perguntar "onde paramos", pedir o status de um pedido de marca, ou quando o marcas-master precisar carregar/atualizar o estado do caso. Tambem ao iniciar um caso novo.
---

# MEMORIA-DE-CASO-MARCA

> Tier 0. Registro append-only do caso. O `marcas-master` le no inicio e atualiza no fim de cada ato.

## Objetivo
Nunca perder o fio do caso: o que e a marca, quais classes, quais processos correm, quais prazos vencem e o que ja foi feito.

## Onde grava
Pasta `marca-inpi/casos/<slug-do-caso>.md` no diretorio de trabalho. Append-only: cada ato vira uma nova linha no historico, nunca apaga o anterior.

## Estrutura do arquivo de caso
```markdown
# Caso: <nome/marca>
## Identificacao
- Titular: <nome/CNPJ>
- Marca: <sinal> | Apresentacao: nominativa/mista/figurativa/3D/posicao
- Classes NCL: <ex: 25, 35>  (cada classe = 1 processo)
## Processos INPI
- Processo <numero> | Classe <n> | Status: <deposito/exame/oposicao/deferido/indeferido/registro>
## Prazos
- <data> | <ato> | <fonte: RPI n>
## Historico (append-only)
- <data> | <ato praticado> | <skill> | <resultado>
## Proximo passo
- <acao> ate <data>
```

## Metodologia
1. Ao iniciar caso: criar o arquivo com identificacao + classes.
2. A cada ato: **acrescentar** linha no Historico + atualizar Processos/Prazos/Proximo passo.
3. Nunca sobrescrever historico anterior (auditabilidade).

## Entrega obrigatoria final
- Arquivo de caso criado/atualizado + resumo do estado atual (classes, processos, proximo prazo).

## Guard
Estado e fato, nao opiniao. Registrar numeros de processo e prazos exatamente como constam na fonte (RPI/INPI) — nao estimar datas.
