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
