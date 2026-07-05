---
tipo: decisao
codigo: G004
status: superada
dominio: Jurídico
requer_aval_humano: sim
origem: "[[2025-09-07 - Análise jurídica e de negócios (Mauro, Simone)]]"
supera:
superada_por: G008
criado: 2026-07-02
atualizado: 2026-07-05
---

# G004 — Base legal LGPD (tutela de saúde) sem autorização hospitalar

**Decisão:** O desenvolvimento inicial não dependerá de autorização formal dos hospitais, amparando-se no direito do médico de guardar cópias dos registros de seus próprios pacientes (tutela de saúde, LGPD). Modelo de dados: médico = controlador, aplicativo = operador, com criptografia.

**Racional:** Viabiliza o produto sem depender de contratos hospitalares, sustentado na base legal da LGPD para fins assistenciais.

**Origem:** [[2025-09-07 - Análise jurídica e de negócios (Mauro, Simone)]] · aprofundada em [[2025-09-11 - Apresentação Docbook e parceria (Vitor, Igor)]]

> ⚠️ **Aval humano (jurídico):** interpretação da LGPD/tutela de saúde precisa ser validada por advogado qualificado. Sinalizada, não tratar como final.

> 🔁 **SUPERADA por [[G008 - Base legal LGPD — consentimento do paciente]]** (reunião [[2025-10-01 - Alinhamento LGPD e funcionalidades (Vitor, Igor, Anna Gabriela)]]): a equipe considerou "tutela de saúde" controversa e adotou o **consentimento do paciente** como base legal principal. O modelo controlador (médico) / operador (app) e o não-uso de autorização hospitalar permanecem válidos e evoluem em [[G009 - Arquitetura modular de dados (básico pseudonimizado, avançado com consentimento)]].
