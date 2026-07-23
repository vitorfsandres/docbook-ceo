---
tipo: reuniao
data: 2026-07-23
participantes: [Vitor, Igor]
classe: ata-primaria
dominios: [Tecnologia, Produto]
fonte_drive: "https://docs.google.com/document/d/1T4pgYg1UFKmL6dijczA5FJB_kw3R949Ue7j6_i5_PiY/edit?tab=t.0"
criado: 2026-07-23
atualizado: 2026-07-23
---

# 2026-07-23 — Automação de backlog com IA e exportação de prontuários (Vitor, Igor)

## Resumo
Vitor e Igor definiram a transição do fluxo de trabalho de pedidos informais por WhatsApp para uma **gestão de backlog oficial no GitHub Projects** (issues + Kanban como fonte da verdade, com três templates), operada por **Claude Code via CLI**. O WhatsApp permanece como *inbox* de captura, processado por uma **skill de IA** (ex.: `/requisitos`) que lê o `.zip` da conversa, aplica templates e gera issues, com controle de *timestamps* e verificação anti-duplicata. Discutiu-se transcrição de áudio (*Whisper*) e um **captador de voz flutuante no app** com mapeamento de rota, além da **flexibilização da exportação clínica** (export nativo com timeline+anexos basta, com granularidade). Vitor destacou o alto valor de usar relatos clínicos reais para a IA gerar **"protocolos salvadores"**, tema de reunião futura dedicada.

## Unidades geradas

### Decisões
- [[G041 - GitHub Projects como backlog oficial, operado por Claude Code via CLI]]
- [[G042 - WhatsApp como inbox; triagem por IA via export .zip]]
- [[G043 - Exportação clínica flexível (export nativo basta, com granularidade)]]

### Tarefas (estado atual em [[Tarefas]])
- Adicionar Igor como Administrador do repositório/projeto GitHub — Vitor — **feita** (concluída durante a call).
- Criar skill de automação de backlog (`/requisitos`: zip WhatsApp → issues, anti-duplicata) — Vitor.
- Desenvolver captador de áudio (ícone flutuante de microfone em todas as páginas, com rota mapeada) — Igor.
- Dar granularidade à exportação do *workspace* (selecionar só texto ou só imagem) — Igor.

### Risco
- IA recriar tarefas já consolidadas a partir dos *logs* acumulados do WhatsApp (duplicidade) — registrado em [[Riscos]].

### Pendência
- Reunião futura dedicada ao amadurecimento dos **"protocolos salvadores"** sugeridos por IA — ver [[Painel]].

### Fatos de domínio
- Tecnologia → [[Arquitetura]] (backlog no GitHub Projects, skill de triagem, captura por voz, IA como "entrevistadora" de requisitos, recomendação de checar o Vault/CLAUDE.md ao gerar código).
- Produto → [[Produto]] (captador de voz flutuante, exportação flexível/granular, geração de protocolos a partir de relatos clínicos).

## Notas de origem (da ata)
- **Insights:** refinamento de requisitos assistido por IA conceituado como "entrevista" (a IA questiona ambiguidades antes de criar a issue); a rota/URL da página anexada à transcrição de voz dispensa *screenshots*; injeção de relatos de eventos críticos reais (PCRs de 3 e 7 min revertidas, noradrenalina, acesso venoso central) gerou protocolos padronizados com precisão.
- **Desafios:** duplicidade de tarefas (logs acumulam diariamente); limitação de contexto no WhatsApp (necessidade de metadados informais tipo "Início da requisição 1"); resistência médica ao relato convencional pela rotina acelerada — validou o reporte por voz.
- **Recomendações:** grupo de WhatsApp restrito (Igor+Vitor) só como inbox; condicionar a IA a checar o Vault/`CLAUDE.md` ao criar/atualizar código, para manter padronização e glossário.
