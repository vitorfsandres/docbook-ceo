---
name: retroativo
description: Processa o acervo histórico de reuniões (as ~50 atas em _staging/reunioes/) em ordem cronológica e em lotes pequenos, de forma resumível. Cria as Notas de Reunião, reconcilia decisões e tarefas ao longo do tempo (com supersessão), acumula fatos de domínio, trata a lacuna fev–abr/2026 e, ao final, gera um checklist de validação para o CEO. Use repetidamente, uma vez por sessão, até zerar o acervo.
---

# /retroativo — Ingestão do acervo de reuniões (lote histórico)

Você está no vault estratégico de CEO do DocBook (repositório `docbook-ceo`). Processe o **acervo histórico** de reuniões seguindo à risca a seção **"Ingestão de Reuniões"** do `CLAUDE.md` deste repositório — o esquema, o roteamento e as regras estão lá; siga-os, não os repita.

O que torna isto diferente de uma reunião avulsa: as **decisões evoluem entre reuniões**, então a ordem importa. Processe em **ordem cronológica**, em **lotes pequenos**, usando o próprio vault (G0xx, `Tarefas.md`, notas vivas) como memória entre execuções. Você roda, para, e é chamado de novo — até o acervo zerar.

## Entrada
- As atas estão em `_staging/reunioes/` como arquivos locais, exportadas do Drive. A data está no nome do arquivo.
- Transcrições são apenas lastro: só consulte se a ata estiver ambígua.
- `$ARGUMENTS` pode conter um número = quantas atas processar neste lote. Se vazio, use **5 a 8** (o suficiente para não estourar o contexto).

## Como escolher o lote
1. Liste todas as atas em `_staging/reunioes/` em **ordem de data** (crescente).
2. **Pule** as que já têm Nota de Reunião correspondente em `08 - Material Bruto/Reuniões/` — já foram processadas em lotes anteriores.
3. Pegue as próximas N atas ainda não processadas, na ordem das datas.
4. Se não sobrar nenhuma, vá direto para "Ao terminar o acervo" e pare.

## Passos, para cada ata do lote (na ordem cronológica)
1. Leia a ata. Extraia as unidades pelo esquema do `CLAUDE.md`.
2. **Reconcilie construindo o estado acumulado** (não é só empilhar):
   - **Decisão** → próximo `G0xx` sequencial. Se uma decisão posterior supera uma anterior já registrada, marque a antiga como `superada` + `superada_por`, e a nova com `supera`. (Crie `07 - Decisões/` se não existir.)
   - **Tarefa** → o tracker `00 - Painel/Tarefas.md` deve **convergir para o estado atual**: uma tarefa aberta em maio e concluída numa reunião de julho entra como `feita` (com origem em maio e a atualização registrada), **não** como aberta. Antes de criar, procure equivalente e atualize em vez de duplicar.
   - **Fato de domínio** → atualize a nota viva do domínio; último valor vale; conflito entre reuniões → mantenha os dois e sinalize. (Crie a nota do domínio se não existir.)
   - **Mudança em documento canônico** → aplique na nota viva alvo, citando a origem.
3. **Crie a Nota de Reunião** em `08 - Material Bruto/Reuniões/AAAA-MM-DD - <slug>.md`, com o frontmatter do contrato, resumo de 3–5 linhas e wikilinks para todas as unidades geradas. Em `fonte_drive`, registre o nome do arquivo da ata como âncora de rastreabilidade (o link direto do Drive será conferido depois — ver checklist final).
4. **Aval humano:** decisões de jurídico ou finanças entram com `requer_aval_humano: sim`.
5. **Não invente.** O que a ata não disser, não preencha; inferências ficam marcadas como tal.

## Lacuna fev–abr/2026
- Se ainda não existir, crie **uma vez** a nota `08 - Material Bruto/Reuniões/2026-02 a 04 - Lacuna (sem registro).md`, explicitando que não há registro nesse período (buraco visível, não silencioso).
- Se a ata de mai/2026 referenciar algo nascido na lacuna, registre com `origem: inferida (lacuna)` e **marque para o CEO confirmar**. Não invente o que teria sido decidido lá.

## Ao fim de cada lote
- Commit com a mensagem `retroativo: lote ate AAAA-MM-DD` e `git push` (o push sincroniza com a base de conhecimento do Project).

## Ao terminar o acervo (quando não sobrar ata para processar)
Gere `00 - Painel/_Validacao Retroativa.md` — o checklist de validação do CEO — reunindo:
- decisões em `status: proposta` aguardando o ok do CEO;
- todas as decisões com `requer_aval_humano: sim` (jurídico/finanças a validar com especialista);
- conflitos de fato de domínio que você sinalizou;
- tarefas em aberto sem responsável ou sem prazo;
- notas cujo `fonte_drive` ainda precisa do link direto do Doc no Drive.
Commit e push desse checklist.

## Relatório ao fim de cada execução
Reporte de forma enxuta:
- quais atas foram processadas neste lote (com datas);
- decisões criadas e superadas (códigos `G0xx`), tarefas novas/atualizadas;
- onde você parou e **quantas atas ainda restam** no acervo;
- se foi a execução final, avise que o checklist de validação foi gerado.

Escreva tudo (notas, checklist e relatório) em português do Brasil.