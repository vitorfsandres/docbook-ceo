---
tipo: reuniao
data: 2025-10-01
participantes: [Vitor, Igor, Anna Gabriela]
classe: ata-primaria
dominios: [Jurídico, Produto, Tecnologia]
fonte_drive: "_staging/reunioes/atas-md/2025-10-01 - Ata - Alinhamento estratégico sobre LGPD e funcionalidades do aplicativo Docbook - Vitor, Igor, Anna Gabriela.md — (link direto do Drive pendente)"
criado: 2026-07-05
atualizado: 2026-07-05
---

# 2025-10-01 — Alinhamento LGPD e funcionalidades (Vitor, Igor, Anna Gabriela)

Preparação jurídica/técnica para a reunião com o investidor. Anna Gabriela (jurídico) e Igor (técnico) concluíram que o **consentimento do paciente** é a base legal mais segura (tutela de saúde é controversa). Definiram arquitetura de **dois módulos** — básico com dados pseudonimizados (sem consentimento) e avançado com consentimento eletrônico — mantendo Docbook como operador e o médico como controlador. Segurança de infraestrutura delegada a nuvem (ex.: AWS); app não substitui o prontuário oficial.

## Unidades geradas
- **Decisões:** [[G008 - Base legal LGPD — consentimento do paciente]] (supera [[G004 - Base legal LGPD (tutela de saúde) sem autorização hospitalar]]) · [[G009 - Arquitetura modular de dados (básico pseudonimizado, avançado com consentimento)]]
- **Tarefas:** pesquisa jurídica (nome+doença é hipersensível? nº de prontuário/atendimento armazenável?) — Anna Gabriela → [[Tarefas]]
- **Fatos de domínio:** consentimento/pseudonimização, controlador/operador, "não substitui prontuário", upload de fotos → risco atribuído ao médico via termos → [[Jurídico & LGPD]] · módulos básico/avançado → [[Produto]] · infra em nuvem/AWS (⚠️ conflita com Railway de [[G006 - Arquitetura do MVP]]) → [[Arquitetura]]

> ⚠️ Teor **jurídico** — decisões com `requer_aval_humano: sim`.
