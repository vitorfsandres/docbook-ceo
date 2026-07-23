---
tipo: dominio
dominio: Tecnologia
titulo: Arquitetura
criado: 2026-07-02
atualizado: 2026-07-23
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

## Atualizações — dez/2025–jan/2026
- **Mobile-first** (UX em listas sanfona) — [[G025 - MVP mobile-first]] — origem [[2025-12-19 - Refinamento do MVP: mobile-first e escopo (Igor, Vitor)]].
- **Metodologia de tickets:** Casos de Uso + Critérios de Aceitação + "Deep Dive" — origem [[2025-12-19 - Refinamento do MVP: mobile-first e escopo (Igor, Vitor)]].
- **Cadastro Rápido + OCR**; ambiente de simulação com BD local — origem [[2025-12-19 - Refinamento do MVP: mobile-first e escopo (Igor, Vitor)]].
- **Vibe Kanban + IA** (Codex/GPT p/ Vitor; Claude/Cursor p/ Igor) automatiza código→PR — [[G029 - Vibe Kanban + IA no fluxo de desenvolvimento]] — origem [[2026-01-22 - Vibe Kanban e automação de dev com IA (Igor, Vitor)]].
- **Fluxo git:** merges na `main` por ora → depois `dev`/`production` (produção restrita a Igor); **Firebase Preview Channels** por PR; servidor compartilhado do board a criar — origem [[2026-01-22 - Vibe Kanban e automação de dev com IA (Igor, Vitor)]].

## Atualizações — fev/2026
- 🔁 **Reconstruir o MVP do zero** (autonomia de Igor; 1,5–3 meses) — [[G030 - Reconstruir o MVP do zero (autonomia técnica de Igor)]] — origem [[2026-02-05 - Acordo de sócios e estratégia de formalização (Vitor, Paulo, Anna Gabriela)]].
- **Não persistir imagens:** OCR extrai o texto e descarta a imagem (só texto no servidor; imagem fica no device) — [[G031 - Não persistir imagens; armazenar só o texto extraído (OCR)]] — origem [[2026-02-12 - Custos, suporte e escala do MVP (Igor, Paulo, Vitor)]].
- **Custo de infra** ~US$ 25–35/mês até 50k usuários (Supabase/Firebase, sem imagens pesadas) — a_reconferir — origem [[2026-02-12 - Custos, suporte e escala do MVP (Igor, Paulo, Vitor)]].
- **Suporte técnico híbrido** (IA + humano assíncrono via ticket, SLA 24–48h) — [[G032 - Suporte híbrido (IA + humano assíncrono via ticket)]] — origem [[2026-02-12 - Custos, suporte e escala do MVP (Igor, Paulo, Vitor)]].

## Atualizações — mai–jun/2026
- 🔁 **Claude Code** (conta Max de Vitor) como ambiente primário de dev; **push direto na `main`** na fase MVP (proteção desabilitada); Vibe Kanban vira open-source local — [[G038 - Fluxo de dev com Claude Code; push direto na main no MVP]] — origem [[2026-06-01 - Fluxo de dev com Claude e GitHub (Vitor, Igor)]].
- Firebase para dados; teste no celular via **versão pública** (localhost inviável no aparelho do hospital); Bun/Zig no build — origem [[2026-06-01 - Fluxo de dev com Claude e GitHub (Vitor, Igor)]].
- Lovable montou a base funcional do app em ~9 créditos, apoiado em documentação robusta — origem [[2026-06-17 - Lançamento do MVP V0 e ameaça MDOCTORS (Paulo, Vitor, Clarissa)]].

## Atualizações — jul/2026
- 🔁 **GitHub Projects (issues + Kanban) vira o backlog oficial e a fonte da verdade** das tarefas de dev; três templates de issue (*bug*, *funcionalidade*, *UX/texto/layout*); **Claude Code integrado por CLI ao GitHub** opera backlog e código pelo terminal — [[G041 - GitHub Projects como backlog oficial, operado por Claude Code via CLI]] (evolui o board do [[G029 - Vibe Kanban + IA no fluxo de desenvolvimento]]) — origem [[2026-07-23 - Automação de backlog com IA e exportação de prontuários (Vitor, Igor)]]. Igor promovido a admin do repo/projeto.
- **WhatsApp como inbox de captura**; skill de IA (ex.: `/requisitos`) processa o `.zip` da conversa → issues, com controle estrito de *timestamps* e verificação anti-duplicata no repositório — [[G042 - WhatsApp como inbox; triagem por IA via export .zip]] — origem [[2026-07-23 - Automação de backlog com IA e exportação de prontuários (Vitor, Igor)]].
- **Refinamento de requisitos como "entrevista":** a IA questiona ambiguidades (layout, localização de botões, conflitos) antes de efetivar a issue, mitigando inconsistências na origem — origem [[2026-07-23 - Automação de backlog com IA e exportação de prontuários (Vitor, Igor)]].
- **Captura de voz com mapeamento de rota:** anexar a rota/URL da página à transcrição (Whisper/open-source) dispensa *screenshots* e contextualiza o reporte — base do captador flutuante no app (ver [[Produto]]) — origem [[2026-07-23 - Automação de backlog com IA e exportação de prontuários (Vitor, Igor)]].
- **Padronização:** ao gerar/atualizar código, condicionar a IA a checar o Vault/`CLAUDE.md` para manter glossário técnico e padrões harmonizados — origem [[2026-07-23 - Automação de backlog com IA e exportação de prontuários (Vitor, Igor)]].

## Documentação do MVP — 17/06/2026 (E6 + D0xx)
> origem: "Documentação do MVP 17/06 — E6 + D0xx" · detalhe canônico em `/docs` E6 (Blocos 6–7) e decisões D0xx.
- **Plataforma do MVP = PWA instalável** (nativo reavaliado no Norte) — D032.
- Captura: **OCR→texto com conferência manual**; o **anexo original é PRESERVADO** (regra de não-destruição) e só descartado **após o desfecho da internação** — D011/D026/D033 (reverte a antiga G031; ver [[G040 - Persistir o anexo original até o desfecho (reverte G031)]]).
- **Google Drive como destino de exportação = Pós-MVP**; MVP = **download local** — D034.
- **Criptografia local no PWA é limitada** (risco técnico; stack a definir no build).
- Detalhe canônico em `/docs` E6 (Blocos 6–7) e decisões D0xx.
