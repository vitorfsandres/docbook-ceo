---
tipo: decisao
codigo: G029
status: validada
dominio: Tecnologia
requer_aval_humano: nao
origem: "[[2026-01-22 - Vibe Kanban e automação de dev com IA (Igor, Vitor)]]"
supera:
superada_por:
criado: 2026-07-05
atualizado: 2026-07-05
---

# G029 — Vibe Kanban + IA no fluxo de desenvolvimento

**Decisão:** Adotar o **Vibe Kanban** integrado a agentes de IA para automatizar a escrita de código e a abertura de PRs a partir do movimento de tarefas no board. Vitor usa **Codex (GPT)** via Vibe Kanban; Igor usa **Claude via Cursor**. Fluxo git: inicialmente merges na `main`; depois `dev` + `production` (produção com merge restrito a Igor). **Firebase Preview Channels** por PR para validação visual. Igor criará um **servidor compartilhado** para o board (hoje roda em localhost).

**Racional:** Elimina passos manuais — a IA escreve o código, descreve as mudanças e abre o PR; ao humano resta revisar e fazer merge.

**Origem:** [[2026-01-22 - Vibe Kanban e automação de dev com IA (Igor, Vitor)]]

> A padronização das descrições de PR geradas pela IA (templates) e o servidor compartilhado seguem como próximos passos técnicos.

> 🔁 **Evoluída por [[G038 - Fluxo de dev com Claude Code; push direto na main no MVP]]** (01/06/2026): Vitor migra para o Claude Code e adota push direto na `main` na fase MVP.
