---
name: reuniao
description: Processa UMA reunião nova cuja ata está em _staging/reunioes/. Extrai decisões, tarefas, pendências, riscos e fatos de domínio; cria a Nota de Reunião; reconcilia contra o estado atual do vault; atualiza o Painel; commita e faz push. Use ao adicionar uma nova ata de reunião ao vault de CEO.
---

# /reuniao — Ingestão de uma reunião nova

Você está no vault estratégico de CEO do DocBook (repositório `docbook-ceo`). Sua tarefa é processar **UMA** reunião nova, seguindo à risca a seção **"Ingestão de Reuniões"** do `CLAUDE.md` deste repositório — o esquema de extração, o roteamento e as regras estão lá; não os repita, siga-os.

## Entrada
- A ata está em `_staging/reunioes/`, exportada do Drive (Markdown).
- `$ARGUMENTS` pode conter o link do Google Drive da ata original. Se vier um link, use-o como `fonte_drive`. Se não vier, **pergunte ao usuário o link do Drive** antes de finalizar a Nota — a rastreabilidade até o original é obrigatória.
- A transcrição é apenas lastro: só a consulte se a ata estiver ambígua.

## Qual ata processar
1. Liste os arquivos em `_staging/reunioes/` que ainda **não** têm Nota de Reunião correspondente em `08 - Material Bruto/Reuniões/`.
2. Se houver exatamente uma ata pendente, processe-a.
3. Se houver mais de uma, liste-as e pergunte qual processar (esta skill processa uma por vez).
4. Se não houver nenhuma pendente, avise e pare.

## Passos
1. Leia a ata. Extraia as unidades pelo esquema do `CLAUDE.md` (decisões, tarefas, pendências, riscos, fatos de domínio, mudanças em documentos).
2. **Reconcilie contra o estado atual ANTES de criar** (anti-duplicata):
   - **Decisão nova** → crie em `07 - Decisões/` como próximo `G0xx` na sequência. Se supera uma existente, marque a antiga como `superada` + `superada_por`, e a nova com `supera`. (Crie a pasta `07 - Decisões/` se ainda não existir.)
   - **Tarefa** → se já existe equivalente em `00 - Painel/Tarefas.md`, atualize a linha (status/atualizado); não duplique. Se é nova, adicione a linha.
   - **Fato de domínio** → atualize a nota viva do domínio (`02`/`03`/`04`…); último valor vale; se conflitar com o registrado, mantenha os dois e sinalize. (Crie a nota do domínio se ainda não existir.)
   - **Mudança em documento canônico** → aplique na nota viva alvo, citando a origem.
3. **Crie a Nota de Reunião** em `08 - Material Bruto/Reuniões/AAAA-MM-DD - <slug>.md`, com o frontmatter do contrato, `fonte_drive` preenchido, resumo de 3–5 linhas e wikilinks para TODAS as unidades geradas.
4. **Salvaguarda de aval humano:** toda decisão de **jurídico ou finanças** entra com `requer_aval_humano: sim` — sinalize, não trate como final.
5. **Atualize o Painel** (`00 - Painel/Painel.md`): pendências novas e a "última atualização" dos domínios tocados.
6. **Não invente.** O que a ata não disser, não preencha. Onde inferir algo, marque como inferência.
7. **Commit + push:** commit com a mensagem `reuniao: AAAA-MM-DD <slug>` e faça `git push`. O push é o que sincroniza o vault com a base de conhecimento do Project.

## Relatório final
Ao terminar, reporte de forma enxuta:
- decisões criadas e superadas (com os códigos `G0xx`);
- tarefas novas e atualizadas;
- **itens que precisam do aval humano** do CEO (jurídico/finanças);
- conflitos ou ambiguidades que você sinalizou;
- confirmação de que commit e push foram feitos.

Escreva tudo (notas e relatório) em português do Brasil.