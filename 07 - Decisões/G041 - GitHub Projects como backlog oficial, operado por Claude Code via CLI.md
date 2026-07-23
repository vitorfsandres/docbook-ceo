---
tipo: decisao
codigo: G041
status: validada
dominio: Tecnologia
requer_aval_humano: nao
origem: "[[2026-07-23 - Automação de backlog com IA e exportação de prontuários (Vitor, Igor)]]"
supera:
superada_por:
criado: 2026-07-23
atualizado: 2026-07-23
---

# G041 — GitHub Projects como backlog oficial, operado por Claude Code via CLI

**Decisão:** O **GitHub** passa a ser o repositório central e a **fonte oficial da verdade** das tarefas de desenvolvimento: o **Kanban do GitHub Projects** e as **issues** substituem o envio manual/informal de requisitos. Três **templates de issue** padronizados: *bug*, *funcionalidade* e *UX/texto/layout*. A automação e a manipulação do backlog e da base de código ocorrem via **Claude Code integrado por CLI ao GitHub** (pelo terminal, sem depender de interface gráfica). Evolui [[G029 - Vibe Kanban + IA no fluxo de desenvolvimento]] (o board sai do Vibe Kanban) e [[G038 - Fluxo de dev com Claude Code; push direto na main no MVP]] (consolida o Claude Code como orquestrador do backlog, não só do código).

**Racional:** Oficializa e centraliza o backlog num único lugar rastreável, elimina o requisito informal por WhatsApp como fonte da verdade e aproveita a integração nativa do Claude Code com o GitHub para operar issues e código no mesmo fluxo.

**Domínio:** Tecnologia.

**Origem:** [[2026-07-23 - Automação de backlog com IA e exportação de prontuários (Vitor, Igor)]]
