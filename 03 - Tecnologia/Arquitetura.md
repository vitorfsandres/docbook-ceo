---
tipo: dominio
dominio: Tecnologia
titulo: Arquitetura
criado: 2026-07-02
atualizado: 2026-07-05
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

## Atualizações — out/2025
- **MVP como PWA (web responsiva) primeiro** — [[G012 - MVP como aplicação web responsiva (PWA) primeiro]].
- ⚠️ **Conflito de infraestrutura:** [[G006 - Arquitetura do MVP]] adotou **Railway** (deploy/armazenamento); em 01/10 discutiu-se delegar a segurança/infra a uma **nuvem robusta (ex.: AWS)**. Ambos registrados até haver decisão explícita — origem [[2025-10-01 - Alinhamento LGPD e funcionalidades (Vitor, Igor, Anna Gabriela)]].
- App foca em **criptografia em trânsito**; segurança do armazenamento delegada ao provedor de nuvem — origem [[2025-10-01 - Alinhamento LGPD e funcionalidades (Vitor, Igor, Anna Gabriela)]].
- Estimativas (Emerson, 08/10): front web **R$ 15–20k**; app nativo **R$ 120–130k**; backend **60–90 dias** com 3 pessoas — a_reconferir — origem [[2025-10-08 - Apresentação a Peng e formação das equipes (investidor)]].
- Metodologia **híbrida** (Scrum/Kanban adaptado) — origem [[2025-10-09 - Pós-Peng, planejamento do MVP (Vitor, Igor)]].
- Sequência: escopo MVP → requisitos (IA) → validação jurídica → arquitetura — [[G014 - Sequência de trabalho — escopo, requisitos, jurídico, arquitetura]].
- Protótipo demo (código IA) precisará de reestruturação arquitetural — a_reconferir — origem [[2025-10-08 - Apresentação a Peng e formação das equipes (investidor)]].

## Atualizações — out/2025 (17–30/10)
- Protótipo sem backend (dados mocados); em **refatoração para arquitetura modular** e definição de interfaces de dados/APIs — origem [[2025-10-17 - Apresentação a novos integrantes e escopo do MVP (Paulo, Rodrigo)]].
- Igor **pausa** modificações no protótipo até a categorização do escopo do MVP (P0–P2) — origem [[2025-10-30 - Planejamento do MVP e negociação com Peng (Vitor, Igor)]].
- **Custos de servidor/nuvem/manutenção** a levantar (base para precificação) — origem [[2025-10-29 - Análise de mercado e modelo de negócios (Paulo, Vitor)]].
- **NotebookLM (Google)** adotado para transcrição/análise de atas e documentos (opera só sobre as fontes fornecidas, com citações) — origem [[2025-10-22 - Mapeamento de mercado e escopo do MVP (Paulo, Vitor)]].
- Ferramenta de workspace da equipe (Notion ou similar) a decidir com Igor — origem [[2025-10-22 - Mapeamento de mercado e escopo do MVP (Paulo, Vitor)]].

## Atualizações — nov–dez/2025
- **João** designado como ajudante de Igor em demandas operacionais — origem [[2025-12-05 - Diagnóstico G4 e decisão de bootstrap (Paulo, Vitor)]].
- Custos de infra (servidor/nuvem/armazenamento/suporte) a levantar com Igor (base de precificação) — origem [[2025-11-09 - Apresentação da análise de mercado (Paulo, Vitor)]].
- Board/Kanban do MVP gerido por label **"Pós MVP"** (MVP vs backlog); revisão tarefa-a-tarefa do escopo — origem [[2025-12-05 - Refinamento do MVP e feedback de médico (Igor, Vitor)]].
