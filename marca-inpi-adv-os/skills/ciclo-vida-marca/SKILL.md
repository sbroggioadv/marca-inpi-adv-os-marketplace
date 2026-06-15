---
name: ciclo-vida-marca
description: Gere a marca pós-registro — prorrogação decenal (art. 133), cessão de pedido/registro (arts. 134-135), licença de uso (arts. 139-141) e anotações de cessão, ônus e alterações de nome/sede/endereço (arts. 136-137). Use quando o operador disser "prorrogar marca", "renovar registro de marca", "vencimento da marca", "ceder marca", "transferir titularidade", "licenciar marca", "contrato de licença de uso de marca", "averbar licença", "anotar mudança de nome da empresa", "marca vai expirar", ou descrever administração de marca já registrada. Prorrogação — pedido no último ano de vigência (133 § 1º) ou nos 6 meses seguintes com retribuição adicional (133 § 2º). GRU 374 (prorrogação ordinária R$ 1.000) / 375 (extraordinária R$ 2.000), por classe.
---

# CICLO DE VIDA DA MARCA — pós-registro (arts. 133-141 LPI)

> Camada 3 — Serviços administrativos INPI. Acionada pelo `marcas-master` para a gestão da marca já registrada: prorrogação, cessão, licença e anotações.

## Anexos obrigatórios (context/)
- `context/lpi-marcas-titulo-iii.md` — **art. 133 (vigência 10 anos da concessão, prorrogável; § 1º pedido no último ano; § 2º + 6 meses com retribuição adicional; § 3º exige art. 128)**; arts. 134-135 (cessão — cessionário deve atender aos requisitos legais; a cessão deve compreender todas as marcas iguais/semelhantes do cedente, sob pena de cancelamento/arquivamento dos não cedidos); arts. 136-137 (anotações de cessão, ônus e alteração de nome/sede/endereço; efeitos a terceiros a partir da publicação); art. 138 (recurso); **arts. 139-141 (licença de uso — controle de qualidade pelo titular; averbação para efeitos a terceiros; art. 140 § 2º dispensa de averbação para prova de uso; recurso do indeferimento)**.
- `context/custos-gru-inpi.md` — GRU 374 (prorrogação ordinária R$ 1.000) / 375 (extraordinária R$ 2.000), por classe; demais serviços conforme tabela.
- `context/tratados-cup-madri-trips.md` — cessão livre e vedação de licença compulsória de marca (TRIPS art. 21); cessão (CUP art. 6 quater), sob demanda.

## Objetivo
Manter e administrar o registro de marca: renovar a vigência no prazo, transferir titularidade corretamente, licenciar o uso com segurança e registrar as anotações necessárias para eficácia perante terceiros.

## Quando ativar
- Registro próximo do fim do decênio (prorrogação).
- Transferência de titularidade (cessão de pedido ou registro).
- Licenciamento do uso da marca a terceiro (franquia, parceria, grupo econômico).
- Mudança de nome/sede/endereço do titular ou constituição de ônus (anotações).

## Metodologia
1. **Estado do caso** via `memoria-de-caso-marca`: registro(s) (nº, classe, titular, **data da concessão e do decênio**), ato pretendido (prorrogar/ceder/licenciar/anotar).
2. **Prorrogação (art. 133):** vigência de **10 anos da concessão**, prorrogável. Pedido no **último ano de vigência** (§ 1º) ou nos **6 meses seguintes** com **retribuição adicional** (§ 2º); a prorrogação exige o art. 128 (§ 3º). Custas: **GRU 374** (ordinária) / **375** (extraordinária), por classe. **Alertar o prazo decadencial** — perder o decênio extingue o registro (art. 142 I).
3. **Cessão (arts. 134-135):** o cessionário deve atender aos requisitos legais para requerer registro; a cessão deve **compreender todas as marcas iguais/semelhantes** do cedente para produtos/serviços idênticos/afins, **sob pena de cancelamento/arquivamento** das não cedidas (art. 135). Providenciar a **anotação** (art. 136 I).
4. **Licença de uso (arts. 139-141):** redigir/orientar contrato com **controle de qualidade pelo titular** (art. 139); **averbar no INPI** para efeitos a terceiros (art. 140), lembrando que a averbação **não é exigida** apenas para prova de uso (art. 140 § 2º). Do indeferimento da averbação cabe recurso (art. 141).
5. **Anotações (arts. 136-137):** cessão, ônus/limitações e **alterações de nome/sede/endereço** — produzem efeitos a terceiros a partir da **publicação** (art. 137).
6. **Custos:** indicar a(s) GRU(s) aplicável(is) por classe (`custos-gru-inpi.md`).
7. **Validação:** todo dispositivo citado passa por `validador-marcario`.
8. Atualizar `memoria-de-caso-marca` (ato praticado, novo termo de vigência, anotações pendentes, próximo decênio).

## Entrega obrigatória final
- Peça/requerimento ou minuta adequada ao ato (prorrogação · cessão + anotação · contrato de licença + averbação · anotação de alteração/ônus).
- GRU(s) indicada(s) por classe (374/375 na prorrogação; demais conforme o ato).
- Alertas de prazo: decênio (último ano + 6 meses com adicional) e de eficácia das anotações (a partir da publicação).
- `memoria-de-caso-marca` atualizado + próximo passo (novo decênio, averbação pendente).
- **Validação pela `suprema-corte-marcaria` (R1–R4) antes da entrega.**

## Guard
Nenhum dispositivo/súmula/acórdão entra na peça sem `validador-marcario`. **Prorrogação é prazo decadencial** — não deixar perder o decênio. Cessão deve abranger todas as marcas iguais/semelhantes (art. 135). Licença averbada para efeitos a terceiros (art. 140). Custas por classe. Entrega só após `suprema-corte-marcaria`. Na dúvida sobre vigência/valor de GRU, bloquear e checar ao vivo.
