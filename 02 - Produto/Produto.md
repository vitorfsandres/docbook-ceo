---
tipo: dominio
dominio: Produto
titulo: Produto
criado: 2026-07-02
atualizado: 2026-07-05
---

# Produto

> Nota viva do produto (proposta de valor, funcionalidades, escopo do MVP). Último valor vale; cada fato cita a origem.

## Proposta de valor
Aplicativo para equipes médicas cirúrgicas que ataca três dores centrais — confiança: confirmado — origem [[2025-09-11 - Apresentação Docbook e parceria (Vitor, Igor)]]:
1. Passagem de plantão desorganizada (papel/WhatsApp) → sistema centralizado e rastreável.
2. Monitoramento pós-operatório ineficiente → acompanhamento remoto pós-alta, prevenindo reinternações.
3. Pressão hospitalar por indicadores → ferramenta própria da equipe para métricas (reinternação, complicações, óbitos, tempo de resposta).

## Funcionalidades (confirmado — origem [[2025-09-11 - Apresentação Docbook e parceria (Vitor, Igor)]])
- **Dashboard do plantão:** visão centralizada de pacientes, visitas, evoluções, prescrições e pendências.
- **Gestão de pacientes com OCR:** registro de evoluções e boletins/descrições cirúrgicas via OCR (foto/PDF), minimizando digitação.
- **Dashboard cirúrgico:** status das cirurgias em tempo real (agendada/em andamento/finalizada) com timestamps para auditoria.
- **Controle de interconsultas:** registro e gestão de pedidos de avaliação de outras equipes.
- **Monitoramento pós-operatório remoto:** paciente responde questionários de sintomas; sistema gera score de risco e dispara alertas automáticos à equipe. **Diferencial-chave.**

## Escopo do MVP
- Notificações **não** são prioridade para o lançamento inicial — origem [[G006 - Arquitetura do MVP]].
- Ideias futuras (a_reconferir): integração com PACS/imagem, IA para otimização de fluxos, dados estatísticos para pesquisa e benchmarking entre equipes — origem [[2025-09-11 - Apresentação Docbook e parceria (Vitor, Igor)]].

## Princípios de UX
- Adesão depende de experiência extremamente fluida, mínimo de cliques e esforço; médicos são avessos a sistemas burocráticos — confirmado — origem [[2025-09-11 - Apresentação Docbook e parceria (Vitor, Igor)]].

## Atualizações — out/2025
- **Arquitetura de dados em 2 módulos** (básico pseudonimizado / avançado com consentimento) — confirmado — [[G009 - Arquitetura modular de dados (básico pseudonimizado, avançado com consentimento)]] · origem [[2025-10-01 - Alinhamento LGPD e funcionalidades (Vitor, Igor, Anna Gabriela)]].
- **MVP como PWA (web responsiva) primeiro**, nativo depois — confirmado — [[G012 - MVP como aplicação web responsiva (PWA) primeiro]].
- App **não substitui o prontuário oficial** (explícito nos termos) — confirmado — origem [[2025-10-03 - Roteiro pré-reunião Peng (Vitor, Luiz Carlos)]].
- Protótipo **demo** atual gerado com IA, sem BD (dados simulados/locais); serve de guia, não de produto final — a_reconferir — origem [[2025-10-08 - Apresentação a Peng e formação das equipes (investidor)]].
- Escopo do MVP a ser **congelado a partir do demo** antes de codificar — [[G014 - Sequência de trabalho — escopo, requisitos, jurídico, arquitetura]].
- Meta: versão funcional até fim de **dez/2025–jan/2026** — a_reconferir — origem [[2025-10-08 - Apresentação a Peng e formação das equipes (investidor)]].

## Atualizações — out/2025 (17–30/10)
- **Escopo do MVP: perfis Médico e Paciente** (secretária/instrumentador → futuro) — [[G015 - Escopo do MVP nos perfis Médico e Paciente]] — origem [[2025-10-17 - Apresentação a novos integrantes e escopo do MVP (Paulo, Rodrigo)]].
- ⚠️ **Escopo em aberto:** incluir o **monitoramento pós-operatório** no MVP? Vitor defende (diferencial validado pelo médico-chefe); Paulo/Igor querem MVP enxuto — ver [[Painel]] — origem [[2025-10-22 - Mapeamento de mercado e escopo do MVP (Paulo, Vitor)]], [[2025-10-30 - Planejamento do MVP e negociação com Peng (Vitor, Igor)]].
- **MVP enxuto / time-to-market**; backlog a categorizar em **P0–P1–P2** (Vitor) — origem [[2025-10-30 - Planejamento do MVP e negociação com Peng (Vitor, Igor)]].
- **Validação:** testar o MVP com rede de médicos amigos de confiança antes do lançamento — origem [[2025-10-29 - Análise de mercado e modelo de negócios (Paulo, Vitor)]].
- App pós-op é ferramenta de **triagem**, não diagnóstico (evita reinternações desnecessárias) — origem [[2025-10-17 - Apresentação a novos integrantes e escopo do MVP (Paulo, Rodrigo)]].

## Atualizações — nov–dez/2025
- **Requisito crítico: input de dados extremamente ágil** (competir com "tirar foto") — origem [[2025-12-05 - Refinamento do MVP e feedback de médico (Igor, Vitor)]].
- **Validação:** cirurgião com 20 anos valida a proposta (arquiva tudo manualmente, sem organização/estatísticas) — origem [[2025-12-05 - Refinamento do MVP e feedback de médico (Igor, Vitor)]].
- **Gestão de escopo no board:** tarefas sem a label **"Pós MVP"** = MVP atual; demais vão ao backlog — origem [[2025-12-05 - Refinamento do MVP e feedback de médico (Igor, Vitor)]].
- **Validação de campo (17/11):** dores reais de coordenação/comunicação/metas na equipe cirúrgica reforçam o valor do produto — origem [[2025-11-17 - Equipe de Cirurgia Geral — escalas e metas (contexto clínico)]].

## Atualizações — dez/2025–jan/2026
- **Mobile-first** (UX em listas sanfona) — [[G025 - MVP mobile-first]] — origem [[2025-12-19 - Refinamento do MVP: mobile-first e escopo (Igor, Vitor)]].
- **Escopo enxuto; Pós-MVP:** RBAC, notificações automáticas, **interação do paciente no pós-op** e KPIs complexos postergados — [[G026 - Escopo enxuto do MVP; funcionalidades postergadas para Pós-MVP]] — origem [[2025-12-19 - Refinamento do MVP: mobile-first e escopo (Igor, Vitor)]].
- **Mantido no MVP:** arquivamento automático (por alta), duplicados temporários (merge posterior), PDF simplificado (2 modelos), Cadastro Rápido + OCR — origem [[2025-12-19 - Refinamento do MVP: mobile-first e escopo (Igor, Vitor)]].
- **Terminologia:** erros/dados incompletos = "Inconsistências"/"Notificações" (não "Pendências") — origem [[2025-12-19 - Refinamento do MVP: mobile-first e escopo (Igor, Vitor)]].
- **OCR** reafirmado como maior diferencial ("bloco de notas refinado") — origem [[2025-12-19 - Refinamento do MVP: mobile-first e escopo (Igor, Vitor)]].
- ⚠️ **Pós-op = wedge de marketing** ([[G028 - Plano de marketing e growth (HyperCube); pós-op como wedge]]) embora a interação do paciente esteja no Pós-MVP — tensão a observar — origem [[2026-01-21 - Plano de marketing e growth — HyperCube (Gabriel, Vitor, Paulo)]].

## Atualizações — fev/2026
- 🔁 **MVP reconstruído do zero** (base limpa, em vez de retrabalhar o demo) — [[G030 - Reconstruir o MVP do zero (autonomia técnica de Igor)]] — origem [[2026-02-05 - Acordo de sócios e estratégia de formalização (Vitor, Paulo, Anna Gabriela)]].

## Atualizações — mai–jun/2026
- **Versão 00 do MVP** congelada após rodar um fluxo completo de plantão — [[G034 - Congelar o MVP na Versão 00 (fluxo completo de plantão)]] — origem [[2026-05-04 - Desenvolvimento do MVP: Versão 00 (Vitor, Igor)]].
- 🚀 **MVP V0 lançado ao grupo alfa** (~4–5 médicos, sob NDA), limite 29/06/2026; funções de **equipe adiadas** ("em construção") — [[G039 - Lançar o MVP V0 até 29-06 (grupo alfa) frente à MDOCTORS]] — origem [[2026-06-17 - Lançamento do MVP V0 e ameaça MDOCTORS (Paulo, Vitor, Clarissa)]].
- Detalhes V00: OCR por câmera em tempo real; aba de cirurgias; pendências em texto livre; visibilidade pública no workspace — origem [[2026-05-04 - Desenvolvimento do MVP: Versão 00 (Vitor, Igor)]].
- Motor orgânico: botão **"Painel Handoff"** (resumos padronizados para WhatsApp da equipe) — origem [[2026-06-17 - Lançamento do MVP V0 e ameaça MDOCTORS (Paulo, Vitor, Clarissa)]].
