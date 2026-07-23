---
tipo: decisao
codigo: G042
status: validada
dominio: Tecnologia
requer_aval_humano: nao
origem: "[[2026-07-23 - Automação de backlog com IA e exportação de prontuários (Vitor, Igor)]]"
supera:
superada_por:
criado: 2026-07-23
atualizado: 2026-07-23
---

# G042 — WhatsApp como inbox; triagem por IA via export .zip

**Decisão:** O **WhatsApp continua como caixa de entrada** (*brain dump*) de ideias e requisitos brutos, para não gerar fricção no dia a dia. O processamento se dá **exportando o arquivo .zip da conversa** para que a IA (via skill customizada, provavelmente `/requisitos`) descompacte, leia anexos, aplique os templates de issue e gere as tarefas no GitHub — com **controle estrito de *timestamps*** e **verificação ativa no repositório** para **barrar duplicatas**. Recomenda-se um grupo de WhatsApp restrito a Igor e Vitor servindo puramente de inbox.

**Racional:** Preserva o canal de captura natural da equipe (voz/texto no WhatsApp) e transfere o esforço de estruturação para a IA, sem obrigar ninguém a escrever tarefas formais. Complementa [[G041 - GitHub Projects como backlog oficial, operado por Claude Code via CLI]].

**Domínio:** Tecnologia / Operações.

**Origem:** [[2026-07-23 - Automação de backlog com IA e exportação de prontuários (Vitor, Igor)]]

> ⚠️ Risco associado (duplicidade de tarefas a partir dos logs acumulados) registrado em [[Riscos]].
