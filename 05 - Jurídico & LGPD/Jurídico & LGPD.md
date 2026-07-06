---
tipo: dominio
dominio: Jurídico
titulo: Jurídico & LGPD
criado: 2026-07-02
atualizado: 2026-07-05
---

# Jurídico & LGPD

> Nota viva jurídica (base legal, contratos, propriedade intelectual). ⚠️ Todo item aqui **requer aval de humano qualificado** — sinalizado, não final. Ver [[G004 - Base legal LGPD (tutela de saúde) sem autorização hospitalar]].

## Base legal (LGPD)
- Operar sem autorização hospitalar, amparado no direito do médico de guardar cópias dos registros dos seus pacientes (tutela de saúde, LGPD) — a_reconferir (requer validação jurídica) — origem [[2025-09-07 - Análise jurídica e de negócios (Mauro, Simone)]].
- Modelo de dados: médico = **controlador**, aplicativo = **operador**; criptografia das informações — a_reconferir — origem [[2025-09-11 - Apresentação Docbook e parceria (Vitor, Igor)]].

## Propriedade intelectual & contratos
- Principal proteção do negócio: contratos bem estruturados (confidencialidade, responsabilidades, natureza da colaboração) e proteção do código-fonte — origem [[2025-09-07 - Análise jurídica e de negócios (Mauro, Simone)]].
- Risco de plágio/cópia da ideia a mitigar com PI + NDAs — ver [[Riscos]].

## Pendências jurídicas
- Contrato de confidencialidade e parceria entre sócios — ver [[G007 - Postergar PJ; contrato entre sócios]] e [[Tarefas]].

## Atualizações — out/2025
- 🔁 **Base legal principal: consentimento do paciente** (tutela de saúde considerada controversa) — [[G008 - Base legal LGPD — consentimento do paciente]] supera a abordagem anterior — origem [[2025-10-01 - Alinhamento LGPD e funcionalidades (Vitor, Igor, Anna Gabriela)]].
- Arquitetura de consentimento: módulo básico **pseudonimizado** (sem consentimento) / avançado com **consentimento eletrônico** — [[G009 - Arquitetura modular de dados (básico pseudonimizado, avançado com consentimento)]].
- Vinculação de dados pseudonimizados a paciente consentido = **tarefa manual do médico** no MVP — a_reconferir — origem [[2025-10-01 - Alinhamento LGPD e funcionalidades (Vitor, Igor, Anna Gabriela)]].
- Upload de fotos de documentos: responsabilidade sobre o conteúdo **atribuída ao médico via termos de serviço** — origem [[2025-10-01 - Alinhamento LGPD e funcionalidades (Vitor, Igor, Anna Gabriela)]].
- App **não substitui o prontuário oficial** (evita a responsabilidade legal do documento) — confirmado.
- Ponto em pesquisa: "nome + doença" é dado hipersensível? nº de prontuário/atendimento isolado é sensível? — a_reconferir — ver [[Tarefas]].
- Equipe jurídica ampliada: **Dra. Thais** entra com Anna Gabriela (termos de uso, privacidade, consentimento) — origem [[2025-10-08 - Apresentação a Peng e formação das equipes (investidor)]].
- **NDAs assinados** entre os envolvidos — a_reconferir — origem [[2025-10-03 - Roteiro pré-reunião Peng (Vitor, Luiz Carlos)]].
- Anna Gabriela também pode cuidar de **registro de marca/patente** — origem [[2025-10-09 - Pós-Peng, planejamento do MVP (Vitor, Igor)]].

## Atualizações — out/2025 (17–30/10)
- Redação dos documentos jurídicos **depende do escopo final do MVP** (quais dados serão coletados) — origem [[2025-10-17 - Apresentação a novos integrantes e escopo do MVP (Paulo, Rodrigo)]].
- Base para operar: **Política de Privacidade + Termos e Condições**; ponto-chave = termo em que o **médico se responsabiliza por ter obtido o consentimento** do paciente — origem [[2025-10-17 - Apresentação a novos integrantes e escopo do MVP (Paulo, Rodrigo)]].
- Produto considerado **juridicamente viável** por Anna Gabriela — origem [[2025-10-17 - Apresentação a novos integrantes e escopo do MVP (Paulo, Rodrigo)]].
- Escopo jurídico de Anna: termos, consentimento, direito empresarial, legal design, contratos, direito digital, PI — origem [[2025-10-26 - Modelo de sociedade e investimento (Peng, Vitor)]].
- Equipe jurídica de Peng: **Dra. Thaís** (compliance, advogada do banco de Peng) e **Dra. Sara** (criminalista) — origem [[2025-10-26 - Modelo de sociedade e investimento (Peng, Vitor)]].

## Atualizações — nov–dez/2025
- **Memorando de entendimento** entre fundadores antes da PJ — [[G023 - Memorando de entendimento entre fundadores antes da PJ]] — origem [[2025-11-26 - Marca (Evolumed), INPI e vesting societário (Paulo, Vitor)]].
- ⚠️ **Titularidade do código-fonte** (desenvolvido por Igor) em risco: hoje só há NDAs — origem [[2025-11-26 - Marca (Evolumed), INPI e vesting societário (Paulo, Vitor)]] — ver [[Riscos]].
- **Registro de marca no INPI** via nome composto/descritivo ("Docbook, Sistema Médico Pessoal"), sob a marca guarda-chuva Evolumed — origem [[2025-11-26 - Marca (Evolumed), INPI e vesting societário (Paulo, Vitor)]].

## Atualizações — dez/2025–jan/2026
- **NDA** assinado com Gabriel Bezerra antes da apresentação — origem [[2025-12-10 - Protótipo e estratégia de marketing (Vitor, Gabriel)]].
- **Registro duplo de marcas** (Docbook + Evolumed) no INPI (~R$ 800) — [[G027 - Registrar ambas as marcas (Docbook + Evolumed) no INPI]] — origem [[2026-01-15 - Marca (Docbook + Evolumed) e acordo de sócios (Paulo, Vitor)]].
- **Acordo de Sócios** (regras de saída, valuation, comportamento dos sócios) — distinto do contrato social; Paulo estudando antes de acionar a advogada — origem [[2026-01-15 - Marca (Docbook + Evolumed) e acordo de sócios (Paulo, Vitor)]].
- **OCR de dados sensíveis** exige revisão contratual/jurídica (Anna Gabriela), mesmo sem armazenamento permanente — origem [[2025-12-19 - Refinamento do MVP: mobile-first e escopo (Igor, Vitor)]].

## Atualizações — fev/2026
- **Cessão de PI:** sem CNPJ, o código pertence ao dev (Igor); a futura empresa precisará de **contrato de cessão autoral** do código — origem [[2026-02-05 - Acordo de sócios e estratégia de formalização (Vitor, Paulo, Anna Gabriela)]].
- **INPI:** registro **misto** (nome + logo + descritivo) aumenta a distintividade; alto volume e demora de até ~2 anos para concessão — origem [[2026-02-05 - Acordo de sócios e estratégia de formalização (Vitor, Paulo, Anna Gabriela)]].
- Confirmar juridicamente o **descarte das imagens** de prontuário (vs. persistir) — impacta arquitetura/custos ([[G031 - Não persistir imagens; armazenar só o texto extraído (OCR)]]) — origem [[2026-02-12 - Custos, suporte e escala do MVP (Igor, Paulo, Vitor)]].

## Atualizações — mai–jun/2026
- Registro de marca pode ser feito via **CPF** e depois transferido ao CNPJ — a confirmar com Gabriela — origem [[2026-05-19 - Fundação e estruturação da empresa (Paulo, Vitor)]].
- **Comissão de ética** do hospital **validou** a cópia de dados de pacientes (nome, prontuário, evolução) restrita à equipe que cuida do paciente, sem compartilhamento externo — origem [[2026-05-19 - Marketing, investimentos e parcerias — Império (Angelo, Gabriel, Paulo, Vitor)]].
- **NDAs** com os médicos testadores antes do V0 — origem [[2026-06-17 - Lançamento do MVP V0 e ameaça MDOCTORS (Paulo, Vitor, Clarissa)]].

## Documentação do MVP — 17/06/2026 (E6 Bloco 7) — ⚠️ requer_aval_humano: sim
> origem: "Documentação do MVP 17/06 — E6 Bloco 7" · detalhe canônico em `/docs` E6 Bloco 7.
- **Base legal do MVP = tutela da saúde / exercício da Medicina** (LGPD art. 11, II, "f") — **não** consentimento do paciente.
- **Médico/equipe = Controlador; DocBook = Operador**, firmado pelo **Termo de Compromisso** no 1º acesso (auditável).
- O MVP guarda **nome completo** → **segurança técnica é pré-requisito de embarque**.
- Direitos do titular atendidos via **médico-Controlador**; **eliminação definitiva (hard delete)** restrita ao **admin**, com **dupla confirmação**. Avisos de responsabilidade ao exportar handoff/anexos.
- **Pendências jurídicas que BLOQUEIAM o go-live (não o desenvolvimento)** — todas exigindo validação de advogado:
  1. revisão jurídica do **Termo de Compromisso**;
  2. **Política de Privacidade + Termos de Uso**;
  3. **canal/encarregado de contato LGPD** do Operador;
  4. **plano de resposta a incidente**.
- Detalhe canônico em `/docs` E6 Bloco 7.
