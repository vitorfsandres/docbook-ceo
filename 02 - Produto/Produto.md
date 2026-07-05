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
