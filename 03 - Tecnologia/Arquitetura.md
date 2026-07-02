---
tipo: dominio
dominio: Tecnologia
titulo: Arquitetura
criado: 2026-07-02
atualizado: 2026-07-02
---

# Arquitetura

> Nota viva de tecnologia/arquitetura. Último valor vale; cada fato cita a origem. Ver decisão canônica [[G006 - Arquitetura do MVP]].

## Stack do MVP (confirmado — origem [[2025-09-26 - Arquitetura do MVP e potencial investidor (Vitor, Igor)]])
| Camada | Escolha |
|--------|---------|
| Front-end + back-end | NextJS |
| Deploy e armazenamento | Railway |
| Notificações em tempo real | Supabase |
| Autenticação | Google |
| Pagamentos/Subscrição | Stripe (ou controle manual inicial) |

## Princípios
- Terceirizar componentes críticos (auth, pagamentos, notificações) para acelerar o desenvolvimento com time enxuto — confirmado.
- Notificações despriorizadas no MVP (sistema opera sem elas).
- IA (ex.: Cursor) para gerar protótipos/versões A/B descartáveis, sem comprometer a arquitetura final — confirmado.
- Segurança: criptografia dos dados sensíveis; papéis controlador (médico) / operador (app) — ver [[Jurídico & LGPD]].
