---
tipo: checklist
titulo: Validação Retroativa
criado: 2026-07-05
atualizado: 2026-07-05
---

# Validação Retroativa — checklist do CEO

Gerado ao **fim da ingestão retroativa** do acervo de reuniões (mai/2025 → jun/2026): **33 Notas de Reunião** (incl. 1 nota de lacuna), decisões **G001–G039**. Este checklist reúne o que precisa da sua validação humana antes de tratar como final.

---

## 1. Decisões que precisam de aval humano (jurídico / finanças / societário)

> `requer_aval_humano: sim` — sinalizadas, **não** tratadas como final. Validar com advogado/contador qualificado.

| Código | Decisão | Domínio | Observação |
|--------|---------|---------|------------|
| [[G002 - Sociedade Eduardo e Vitor]] | Sociedade Eduardo + Vitor (mai/2025) | Societário | ⚠️ Não reconfirmada desde set/2025 — **confirmar se ainda vigora**. |
| [[G005 - Sociedade Vitor e Igor]] | Sociedade Vitor + Igor | Societário | A reenquadrar como **Igor CTO ≥20% sob vesting**. |
| [[G008 - Base legal LGPD — consentimento do paciente]] | Base legal = consentimento do paciente | Jurídico | Enquadramento LGPD a validar. |
| [[G009 - Arquitetura modular de dados (básico pseudonimizado, avançado com consentimento)]] | Módulo básico pseudonimizado / avançado com consentimento | Produto/Jurídico | Validar se a pseudonimização afasta consentimento. |
| [[G013 - Constituir o projeto como empresa de tecnologia]] | Constituir empresa de tecnologia | Societário | Implementado por G037. |
| [[G022 - Adoção de plano de vesting para sócios e equipe]] | Plano de vesting | Societário | Minuta a elaborar/validar. |
| [[G023 - Memorando de entendimento entre fundadores antes da PJ]] | Memorando / termo pré-societário | Jurídico | Proteger PI/código antes do contrato social. |
| [[G024 - Bootstrap — desenvolver com recursos próprios; não captar agora]] | Bootstrap (não captar agora) | Captação | Deferimento reversível; rodada de Taiwan após validar MVP. |
| [[G027 - Registrar ambas as marcas (Docbook + Evolumed) no INPI]] | Registrar Docbook + Evolumed (INPI) | Jurídico | Via CPF, depois transferir ao CNPJ. |
| [[G031 - Não persistir imagens; armazenar só o texto extraído (OCR)]] | Não persistir imagens de prontuário | Tecnologia/Jurídico | **Confirmar juridicamente** o descarte das imagens. |
| [[G036 - Império como parceria estratégica (participação), não prestação de serviço]] | Império — parceria com participação | Societário | Desenhar/assinar termos da participação. |
| [[G037 - Abrir a empresa só no nome de Vitor (Simples Nacional)]] | Empresa só no nome de Vitor (Simples Nacional) | Societário/Tributário | Validar com contador/advogado. |

**Superadas, mas com teor jurídico/financeiro (só histórico, sem ação):** [[G004 - Base legal LGPD (tutela de saúde) sem autorização hospitalar]], [[G007 - Postergar PJ; contrato entre sócios]], [[G010 - Captação Plano A — investidor Peng Lang]], [[G017 - Estrutura societária proposta por Peng (Peng majoritário via fundo)]], [[G019 - Negociação direta Peng–Vitor; Rodrigo fora]].

---

## 2. Decisões em `status: proposta` aguardando o ok do CEO

**Nenhuma.** Todas as 39 decisões estão como `validada` (28) ou `superada` (5 do caminho Peng + G003, G016). As decisões acima só precisam do aval humano jurídico/financeiro, não de reclassificação.

---

## 3. Conflitos / ambiguidades que sinalizei (decidir/confirmar)

- **Infra: Railway × AWS** — [[G006 - Arquitetura do MVP]] adotou Railway; em out/2025 discutiu-se AWS; em 2026 o dev migrou para **Firebase** (05-04/06-01). Confirmar o stack final.
- **Pós-operatório: wedge × Pós-MVP** — é o **wedge de marketing** ([[G028 - Plano de marketing e growth (HyperCube); pós-op como wedge]]) mas a interação do paciente foi adiada para Pós-MVP ([[G026 - Escopo enxuto do MVP; funcionalidades postergadas para Pós-MVP]]). Alinhar expectativa lançamento × campanha.
- **Sociedade Eduardo × Igor** — a sociedade de mai/2025 (Eduardo) nunca foi reconfirmada; o quadro atual é Vitor (+ Igor sob vesting). Confirmar.
- **Equity do Igor** — discutido de 1% (out) a **≥20%** (nov, Paulo). A definir na minuta de vesting.
- **Projeção de faturamento** — variou entre ~R$ 40 mi (out) e ~R$ 27,4 mi realista (nov). A_reconferir.
- **QR no PDF** — mecânica de growth "Member get Member" (12-10) foi **removida** do PDF do MVP (12-19); adiada.
- **Correção de data aplicada:** captação com Luiz Carlos movida de 2025-10-01 → **2025-09-23** (pela compilação-mestra). Ver a Nota renomeada.

---

## 4. Tarefas abertas sem prazo/responsável claro

- **Prazos:** as atas quase nunca fixaram datas — **a grande maioria das ~36 tarefas abertas/fazendo está sem prazo** (só o lançamento do V0 tem prazo firme: **29/06/2026**). Recomendo priorizar/datar no tracker.
- **Responsável a revisar:**
  - "Organizar documentação do projeto" e "plano de marketing/financeiro" → atribuídas a **Luiz Carlos**, que **saiu do radar** desde out/2025. Reatribuir ou cancelar.
  - "Validar parceria com fábrica de software" → responsável genérico **"Sócios"**. Definir dono.
  - "Avaliar ferramenta de workspace (Notion)" → parada desde out/2025 (a equipe adotou NotebookLM/Obsidian). Reavaliar relevância.
- Fonte completa e status atual: [[Tarefas]].

---

## 5. Rastreabilidade — links do Drive pendentes

- **Todas as ~32 Notas de Reunião** têm `fonte_drive` com o **nome do arquivo** como âncora, mas **falta o link direto** do Doc no Google Drive. Completar quando possível.
- As Notas de **fev/2026** (05, 12, 23) e **jun/2026** (01, 17) foram extraídas da **compilação-mestra `2026.md`** (não havia arquivo avulso) — priorizar a conferência do original dessas.

---

## 6. Panorama do estado atual (jun/2026)

- **Produto:** MVP **V0** em teste com grupo **alfa** (~4–5 médicos, sob NDA); funções de equipe adiadas ("em construção"). Diferencial vs. concorrente **MDOCTORS**: foco no médico/paciente.
- **Captação:** **bootstrap**; rodada de Taiwan (~US$ 2M) só após validar o MVP.
- **Societário:** empresa em abertura **só no nome de Vitor** (Simples Nacional); demais via termo pré-sócios + vesting; **Império** como parceira estratégica com participação.
- **Marca:** Evolumed (guarda-chuva) + Docbook (módulo); registrar ambas.
- **Riscos quentes:** MDOCTORS (cópia), titularidade do código-fonte (só NDAs), resguardo dos NDAs, fadiga do fundador. Ver [[Riscos]].
