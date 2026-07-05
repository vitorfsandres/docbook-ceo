---
tipo: decisao
codigo: G009
status: validada
dominio: Produto
requer_aval_humano: sim
origem: "[[2025-10-01 - Alinhamento LGPD e funcionalidades (Vitor, Igor, Anna Gabriela)]]"
supera:
superada_por:
criado: 2026-07-05
atualizado: 2026-07-05
---

# G009 — Arquitetura modular de dados (básico / avançado)

**Decisão:** Desenvolver o app em dois módulos para calibrar a exigência de consentimento:
- **Módulo Básico (padrão):** uso interno da equipe médica (checklist, passagem de plantão) com **dados pseudonimizados** (primeiro nome/iniciais, nº do leito, nº de atendimento) — não exige consentimento prévio.
- **Módulo Avançado (opcional):** interação direta com o paciente (ex.: monitoramento remoto pós-cirúrgico) — o médico habilita e o paciente cria conta e dá **consentimento eletrônico** específico.

Segurança da infraestrutura delegada a provedor de nuvem robusto; o app foca na segurança da aplicação (criptografia em trânsito). Vinculação de dados pseudonimizados a paciente consentido, no MVP, é tarefa manual do médico.

**Racional:** Viabilizar a gestão interna sem atrito de consentimento, reservando o consentimento formal às funções que tocam o paciente.

**Origem:** [[2025-10-01 - Alinhamento LGPD e funcionalidades (Vitor, Igor, Anna Gabriela)]]

> ⚠️ **Aval humano (jurídico):** validar com advogado se pseudonimização proposta afasta a exigência de consentimento. Base legal em [[G008 - Base legal LGPD — consentimento do paciente]].
