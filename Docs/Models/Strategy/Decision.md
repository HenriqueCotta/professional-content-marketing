---
created_at: 2026-10-21
updated_at: 2026-10-21
version: 1.0.0
---

# Decision

## Finalidade e localização

Uma decisão registra uma escolha relevante que precisará ser compreendida no futuro. Cada registro fica em `Strategy/Decisions/`, com nome descritivo. Não é necessário abrir uma decisão para cada tarefa ou ajuste de redação. O [manual de estratégia](../../Strategy.md) explica como as escolhas passam a orientar a execução.

## Properties e estados

| Campo | Significado |
| --- | --- |
| `created_at` | Criação comprovada do registro autoral. |
| `updated_at` | Última alteração substantiva do registro. |

Este tipo de nota não tem campo de estado. A orientação vigente fica no documento responsável, e os vínculos no corpo explicam substituições. Preencha as datas conforme as [convenções comuns](../Shared/Common.md).

## Como preencher

- **Contexto e alternativas:** apresente o problema e as opções realmente consideradas, quando houver.
- **Escolha e motivação:** registre o que foi escolhido e por quê.
- **Evidências ou preferências:** identifique o que sustenta a escolha. Uma preferência ou necessidade prática pode justificar uma decisão sem ser apresentada como resultado de experimento.
- **Aplicação e início de vigência:** explique onde a escolha será aplicada e desde quando, com a precisão conhecida.
- **Consequências e condições de revisão:** registre os efeitos esperados, os limites e o que justificaria reconsiderar a escolha.
- **Decisão anterior substituída:** vincule o registro anterior quando existir, preservando seu conteúdo e o contexto em que foi adotado.

Quando a decisão alterar a direção, um plano ou uma orientação operacional, atualize também o documento responsável. O registro da decisão explica a escolha; ele não substitui uma orientação atual utilizável. Não transforme um efeito esperado em resultado medido.

## Template e controle

O arquivo inserível é [Templates/Decision.md](../../../Templates/Decision.md). A tabela descreve esse arquivo, não o registro criado com ele; as Properties no topo desta página descrevem o próprio guia.

| Template | created_at | updated_at | version |
| --- | --- | --- | --- |
| [Decision](../../../Templates/Decision.md) | 2026-10-21 | 2026-10-21 | `1.0.0` |
