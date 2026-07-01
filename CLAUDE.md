# DocBook — Vault Estratégico (CEO)

Vault estratégico do CEO do DocBook, separado do repositório do app.

## Ingestão de Reuniões
Bruto (ata + transcrição) fica no Google Drive. O vault recebe só a *Nota de Reunião*.
Ata = fonte primária (sinal). Transcrição = lastro, só consultada se a ata for ambígua.

Cada reunião gera UMA Nota de Reunião em `08 - Material Bruto/Reuniões/AAAA-MM-DD - <slug>.md`:
  frontmatter: tipo: reuniao | data | participantes: [..] | classe: ata-primaria|transcricao-lastro | dominios: [..] | fonte_drive: <links> | criado | atualizado
  corpo: resumo de 3–5 linhas + wikilinks para TODAS as unidades geradas (âncora de rastreabilidade).

A Nota distribui unidades para as casas canônicas:
- Decisão → `07 - Decisões/G0xx - <título>.md` | status: proposta|validada|superada | campos: decisao, racional, dominio, origem: [[reunião]], supera/superada_por, requer_aval_humano: sim|nao
- Tarefa → linha em `00 - Painel/Tarefas.md` | titulo|responsavel|prazo|status: aberta|fazendo|feita|cancelada|dominio|origem: [[reunião]]|atualizado
- Pendência → seção "Pendências" em `00 - Painel/Painel.md`
- Risco → `01 - Estratégia & Governança/Riscos.md` (descrição, dominio, severidade, origem)
- Fato de domínio → nota viva do domínio (02/03/04…): valor + confianca: confirmado|a_reconferir + origem
- Mudança em doc canônico → aplicar na nota viva alvo, citando a origem

Regras:
- Fonte da verdade do STATUS de tarefa = `Tarefas.md`, não a reunião. A reunião é a origem; o estado atual mora no tracker.
- G0xx sequencial. Superação: a nova aponta `supera: G0xx`; a antiga vira `status: superada` + `superada_por: G0yy`.
- Jurídico/finanças: `requer_aval_humano: sim` até um humano qualificado validar. Sinalize, não trate como final.
- Antes de criar decisão/tarefa, busque no vault uma equivalente (anti-duplicata).
- Toda unidade linka à Nota de Reunião de origem. NÃO inventar.
