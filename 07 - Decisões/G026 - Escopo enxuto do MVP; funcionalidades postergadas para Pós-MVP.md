---
tipo: decisao
codigo: G026
status: validada
dominio: Produto
requer_aval_humano: nao
origem: "[[2025-12-19 - Refinamento do MVP: mobile-first e escopo (Igor, Vitor)]]"
supera:
superada_por:
criado: 2026-07-05
atualizado: 2026-07-05
---

# G026 — Escopo enxuto do MVP; funcionalidades postergadas para Pós-MVP

**Decisão:** Manter o MVP mínimo ("canivete suíço" — recurso essencial instantâneo). **Postergadas para Pós-MVP:** permissões granulares de perfil (RBAC), notificações automáticas de novas pendências, **interação direta do paciente no pós-operatório (marcação de sintomas)** e indicadores/KPIs operacionais complexos. Mantidos no MVP: arquivamento automático por data de alta; duplicados temporários (homônimos) com merge posterior; PDF simplificado (2 modelos: visita e cirúrgico); Cadastro Rápido + OCR. Erros/dados incompletos serão chamados de **"Inconsistências"/"Notificações"** (não "Pendências").

**Racional:** Pequenas automações têm custo exponencial de validação/testes/jurídico; foco em release rápida. **Resolve o debate** sobre incluir o pós-op no MVP: a interação do paciente entra no Pós-MVP (refina [[G015 - Escopo do MVP nos perfis Médico e Paciente]]).

**Origem:** [[2025-12-19 - Refinamento do MVP: mobile-first e escopo (Igor, Vitor)]]

> ⚠️ Tensão a observar: o pós-operatório é o **wedge de marketing** ([[G028 - Plano de marketing e growth (HyperCube); pós-op como wedge]]), mas a interação do paciente ficou para Pós-MVP — ver [[Painel]].
