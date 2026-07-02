---
tipo: decisao
codigo: G006
status: validada
dominio: Tecnologia
requer_aval_humano: nao
origem: "[[2025-09-26 - Arquitetura do MVP e potencial investidor (Vitor, Igor)]]"
supera:
superada_por:
criado: 2026-07-02
atualizado: 2026-07-02
---

# G006 — Arquitetura do MVP

**Decisão:** Adotar arquitetura simplificada para o MVP:
- **Front-end + back-end:** NextJS
- **Deploy e armazenamento:** Railway
- **Notificações em tempo real:** Supabase
- **Autenticação:** Google
- **Pagamentos/Subscrição:** Stripe (ou controle manual inicial)

Terceirizar componentes críticos (auth, pagamentos, notificações) para acelerar o desenvolvimento. Notificações **não** são prioridade para o lançamento do MVP — o sistema opera sem elas.

**Racional:** Time enxuto (1 dev + idealizador). Terceirizar o complexo economiza tempo (mais valioso que o custo). IA (ex.: Cursor) pode acelerar protótipos descartáveis sem comprometer a arquitetura final.

**Origem:** [[2025-09-26 - Arquitetura do MVP e potencial investidor (Vitor, Igor)]]
