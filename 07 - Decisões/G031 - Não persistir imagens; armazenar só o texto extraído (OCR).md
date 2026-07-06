---
tipo: decisao
codigo: G031
status: superada
dominio: Tecnologia
requer_aval_humano: sim
origem: "[[2026-02-12 - Custos, suporte e escala do MVP (Igor, Paulo, Vitor)]]"
supera:
superada_por: G040
criado: 2026-07-05
atualizado: 2026-07-06
---

# G031 — Não persistir imagens; armazenar só o texto extraído (OCR)

**Decisão (preliminar):** **Não salvar as imagens** de prontuários/documentos nos servidores. Fluxo: o app lê a imagem, extrai o texto via OCR e **descarta a imagem** (ou a mantém apenas no dispositivo do usuário). Reafirmada no teste da Versão 00 ([[2026-05-04 - Desenvolvimento do MVP: Versão 00 (Vitor, Igor)]]).

**Racional:** Reduz drasticamente o custo de storage (infra para até 50k usuários ativos/mês na faixa de US$ 25–35 com Supabase/Firebase, se não houver imagens pesadas) e resguarda questões jurídicas ao não reter dados sensíveis em nuvem.

**Origem:** [[2026-02-12 - Custos, suporte e escala do MVP (Igor, Paulo, Vitor)]]

> ⚠️ **Aval humano (jurídico):** confirmar a necessidade (ou não) de persistir a imagem original do prontuário vs. apenas o texto — mudança posterior impactaria a arquitetura e os custos. Cenário "pessimista" com armazenamento de imagens deve ser mantido no plano.

> 🔁 **Superada pela documentação do MVP de 17/06 (D033 + E6 Bloco 7):** o MVP preserva o anexo original até o desfecho da internação, em vez de descartar a imagem e guardar só o OCR. Reversão confirmada pelo CEO em 2026-07-06. Ver [[G040 - Persistir o anexo original até o desfecho (reverte G031)]].
