# CLAUDE.md — marca-inpi-adv-os

> Estende o CLAUDE.md global/workspace. Aqui só as regras locais do plugin de marcas.

## Regras invioláveis do plugin
1. **Sempre ler `context/` antes de redigir.** A lei, a NCL, os custos e a jurisprudência vivem nos anexos de `context/` — consulte, não "lembre". Cada skill lista seus anexos obrigatórios.
2. **Anti-alucinação.** Nenhum dispositivo legal, súmula, tese ou acórdão entra em peça sem passar pela skill `validador-marcario` (que cruza com `context/` + guard global `anti-alucinacao-juridica`). Na dúvida sobre vigência/existência → bloquear e checar ao vivo.
3. **Gate Suprema Corte.** Antes de QUALQUER entrega ao usuário, passar pela `suprema-corte-marcaria` (R1 fatos/competência · R2 fundamentação vigente · R3 jurisprudência real · R4 forma/pedidos/custas).
4. **Precificação por classe.** Cada classe NCL = 1 processo administrativo (depósito, GRU e exigências próprios). Honorários e custas multiplicam por classe — sempre separados e explicados ao cliente.
5. **Competência correta.** Nulidade de registro → Justiça Federal (INPI no polo, art. 175 LPI). Abstenção de uso / concorrência desleal entre particulares → Justiça Estadual (STJ Tema 950).
6. **Valores de custas mudam.** A tabela em `context/custos-gru-inpi.md` é referência; confirmar o valor vigente na emissão da GRU.

## Porta única
`marcas-master` é o orquestrador. Ele classifica o setor (via `triagem-marca`), carrega o estado (`memoria-de-caso-marca`), conduz os desdobramentos e fecha pela `suprema-corte-marcaria`.
