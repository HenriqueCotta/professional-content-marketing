---
created_at: 2026-10-21
updated_at: 2026-10-26
version: 1.0.1
---

# Review

Esta página é o guia do tipo Review. Seu frontmatter descreve o guia; a seção Properties descreve os registros produzidos. Os destinos abaixo seguem a [convenção de raiz do PCM](../../Architecture.md#guia-template-e-registro-de-trabalho).

## Finalidade e localização

Uma review interpreta os dados de um post para responder a uma pergunta explícita. A publicação avaliada é documentada conforme o [guia de Post](Post.md). A review fica em `Posts/<Nome do post>/Reviews/` e aponta para os snapshots efetivamente analisados. Ela não substitui os dados brutos nem significa revisão do texto antes da publicação.

Use `Day X - Review.md` quando a idade estiver comprovada. X é a idade correspondente à última captura, de maior `captured_at` entre os snapshots utilizados, segundo a [regra de Day X em Analytics Snapshot](Analytics%20Snapshot.md). Identifique a janela e todas as coletas relevantes; a análise pode incluir períodos anteriores. A data em que a review foi escrita ou editada não redefine a idade dos dados.

Sem datas suficientes, use um nome descritivo sem X inventado, como `Review - Primeira avaliação.md`. Reviews da mesma janela podem receber um complemento que diferencie a pergunta analisada.

## Properties e estados

| Campo | Uso neste registro |
| --- | --- |
| `created_at` | Criação comprovada da nota autoral. |
| `updated_at` | Última alteração substantiva da nota, sem afirmar que ela incorporou coletas mais recentes. |
| `reviewed_at` | Data da avaliação registrada, distinta das datas dos dados analisados. |

A review não recebe campo de estado no padrão mínimo. Datas desconhecidas permanecem vazias; cópia, renomeação, formatação ou ajuste de links não registram uma avaliação nova. Siga [Common](../Shared/Common.md) para a manutenção dessas datas.

## Como preencher

| Seção do template | O que registrar |
| --- | --- |
| Publicação e snapshots utilizados | Links para o post e para as coletas concretas que sustentam a análise. |
| Pergunta da avaliação | O que se pretende entender sobre aquela publicação. |
| Observações | Resultados pertinentes à pergunta, com referência aos snapshots. |
| Interpretação e explicações alternativas | O que os resultados permitem concluir e quais outras explicações permanecem possíveis. |
| Limitações | Amostra, janela, diferenças entre comparações e dúvidas de origem que restringem a conclusão. |
| Encaminhamento | O que repetir, investigar ou deixar em aberto; uma avaliação pode concluir que nada precisa mudar. |
| Alterações substantivas desta review | Mudança relevante, data, motivo e relação com a interpretação anterior. |

Uma observação isolada não comprova causa. Não reapresente uma expectativa como resultado medido. A review pode apontar para decisões ou para a avaliação do conjunto no plano, sem duplicar essa análise.

### Atualizar ou criar outra review

Correções de redação, esclarecimentos de cálculo ou complementos de interpretação da mesma janela podem atualizar a review existente. Uma mudança substantiva atualiza `updated_at` e precisa de explicação quando afetar a leitura anterior; preserve a data original da avaliação.

Uma nova janela ou novos snapshots usados para avaliar a evolução normalmente geram outra review. Preserve a anterior e conecte os registros quando houver mudança de conclusão. Se uma correção reverter uma conclusão usada em decisões, conserve a interpretação anterior e explique o efeito da correção, em vez de apagá-la silenciosamente.

Não escolha entre criar e atualizar apenas pela idade do arquivo. Uma coleta nova, por si só, não obriga fazer outra review. Para retomar uma análise, confira as coletas utilizadas, sua janela, `captured_at`, `reviewed_at` e a pergunta atual; `updated_at` não certifica dados recentes.

## Template e controle

O arquivo inserível é [Templates/Review.md](../../../Templates/Review.md). A tabela descreve esse arquivo, não o registro criado com ele; as Properties no topo desta página descrevem o próprio guia.

| Template | created_at | updated_at | version |
| --- | --- | --- | --- |
| [Review](../../../Templates/Review.md) | 2026-10-21 | 2026-10-21 | `1.0.0` |
