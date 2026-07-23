---
tipo: decisao
codigo: G043
status: validada
dominio: Produto/Tecnologia
requer_aval_humano: nao
origem: "[[2026-07-23 - Automação de backlog com IA e exportação de prontuários (Vitor, Igor)]]"
supera:
superada_por:
criado: 2026-07-23
atualizado: 2026-07-23
---

# G043 — Exportação clínica flexível (export nativo basta, com granularidade)

**Decisão:** A exportação de dados clínicos do app **não precisa ser restrita a um único arquivo Markdown formatado como *Vault***. A **exportação nativa que respeita a linha do tempo e os anexos é suficiente**, pois a IA é capaz de interpretar os metadados brutos. Além disso, o *export* deve ganhar **granularidade** — permitir selecionar componentes específicos (ex.: exportar **apenas texto** ou **apenas imagem**). O objetivo prático é alimentar a IA com o histórico de intercorrências para gerar protocolos médicos padronizados.

**Racional:** Reduz o esforço de engenharia do *export* (não é preciso um formatador Vault dedicado) sem perder utilidade, já que a IA lida com os metadados nativos; a granularidade atende a diferentes usos (privacidade, custo, análise só de texto).

**Domínio:** Produto / Tecnologia.

**Origem:** [[2026-07-23 - Automação de backlog com IA e exportação de prontuários (Vitor, Igor)]]

> Contexto: no MVP o destino do export é **download local** (Google Drive como destino ficou para o Pós-MVP — D034); ver [[Arquitetura]]. A retenção do anexo original segue a regra de [[G040 - Persistir o anexo original até o desfecho (reverte G031)]].
