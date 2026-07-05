---
tipo: reuniao
data: 2026-02-12
participantes: [Paulo Busato, Igor, Vitor]
classe: ata-primaria
dominios: [Tecnologia, Operações, Negócio, Jurídico]
fonte_drive: "_staging/reunioes/atas-md/2026.md (compilação-mestra, seção 2026-02-12) — (link direto do Drive pendente)"
criado: 2026-07-05
atualizado: 2026-07-05
---

# 2026-02-12 — Custos, suporte e escala do MVP (Igor, Paulo, Vitor)

Levantamento das despesas de tecnologia para o plano de negócios, em escalas de 0/50/500/1000+ usuários. Igor mostrou que evitar a persistência de imagens (só extrair texto via OCR) reduz drasticamente o custo de storage (infra até ~50k usuários/mês por US$ 25–35 com Supabase/Firebase). Definiu-se **suporte híbrido** (IA + humano assíncrono via ticket, SLA 24–48h). Pagamentos entram como custo **variável**. Igor consolidará os cenários (pessimista/realista/otimista) em planilha em ~15 dias.

## Unidades geradas
- **Decisões:** [[G031 - Não persistir imagens; armazenar só o texto extraído (OCR)]] · [[G032 - Suporte híbrido (IA + humano assíncrono via ticket)]]
- **Tarefas:** planilha de custos fixos/variáveis (Igor, 15 dias) · verificar custos de app stores (Igor) · validar parceria com "fábrica de software" (sócios) · confirmar juridicamente o descarte de imagens (Igor/Vitor) → [[Tarefas]]
- **Fatos de domínio:** custo de infra ~US$ 25–35/mês até 50k usuários (sem imagens) · suporte via ticket (sem chat) · pagamentos como custo variável · parceria com fábrica de software impacta orçamento (equity vs contratação) → [[Arquitetura]], [[Modelo de Negócio]], [[Societário & Captação]]
