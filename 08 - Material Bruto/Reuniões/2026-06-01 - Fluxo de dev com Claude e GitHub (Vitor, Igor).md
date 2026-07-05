---
tipo: reuniao
data: 2026-06-01
participantes: [Vitor, Igor]
classe: ata-primaria
dominios: [Tecnologia, Produto]
fonte_drive: "_staging/reunioes/atas-md/2026.md (compilação-mestra, seção 2026-06-01) — (link direto do Drive pendente)"
criado: 2026-07-05
atualizado: 2026-07-05
---

# 2026-06-01 — Fluxo de dev com Claude e GitHub (Vitor, Igor)

Igor capacitou Vitor a operar o desenvolvimento do MVP com **Claude Code** (conta Max) + GitHub. Optou-se por Claude Code como ambiente primário (evita tokens de API de orquestradores terceiros), **desabilitar a proteção da branch `main`** (push direto na fase MVP) e **congelar o escopo** (não refazer requisitos com Grillmy agora). OCR básico de etiquetas mantido com escopo flexível (o que falhar, preenchimento manual). Filosofia "Ship it": lançar e iterar por erro/acerto nos plantões.

## Unidades geradas
- **Decisões:** [[G038 - Fluxo de dev com Claude Code; push direto na main no MVP]] (evolui [[G029 - Vibe Kanban + IA no fluxo de desenvolvimento]])
- **Tarefas:** Vitor operar o ciclo autônomo (pedir à IA → merge → testar no celular) · importar automações de Vitor (checklists Obsidian, planilhas Apps Script) para o MVP · Igor faz hotfixes sob demanda → [[Tarefas]]
- **Fatos de domínio:** Claude Code como ambiente primário · push direto na main (MVP) · claude.md opcional nesta fase · planilhas Apps Script de Vitor reduziram ~5 min/paciente · teste via localhost inviável no celular (usar versão pública) · Bun/Zig no build → [[Arquitetura]], [[Produto]]
