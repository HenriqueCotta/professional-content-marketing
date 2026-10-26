---
created_at: 2026-10-21
updated_at: 2026-10-26
version: 1.0.3
---

# Post

Esta página é o guia do tipo Post. Seu frontmatter descreve o guia; a seção Properties descreve os registros produzidos. Os destinos abaixo seguem a [convenção de raiz do PCM](../../Architecture.md#guia-template-e-registro-de-trabalho).

## Finalidade e localização

Um post registra a produção de uma publicação concreta e preserva o texto efetivamente publicado. Crie seu pacote em `Posts/<Nome do post>/<Nome do post>.md`, sem prefixo de data. A intenção de produzir a publicação determina essa criação, não o tamanho da ideia.

O trabalho pode partir de nenhuma, uma ou várias ideias. Quando existirem, mantenha links para elas como origem do raciocínio, sem copiar seus pacotes ou herdar automaticamente todas as suas referências.

A pessoa pode delegar a redação inteira ou escolher outra divisão do trabalho; este modelo não exige coescrita, perguntas ou aprovação de cada trecho. Consulte [Participação e delegação](../../AI%20Guide.md#participação-e-delegação) para ajustar a execução ao pedido e ao contexto.

## Properties e estados

| Campo | Uso neste registro |
| --- | --- |
| `post_status` | Estado da produção, conforme a tabela abaixo. |
| `created_at` | Criação comprovada da nota. |
| `updated_at` | Última alteração substantiva da nota; não certifica a atualidade de todos os fatos. |
| `posted_at` | Data ou momento comprovado da publicação; permanece vazio enquanto desconhecido. |
| `url` | Opcional, quando o endereço da publicação estiver disponível. |
| `scheduled_at` | Opcional, somente quando houver agendamento real. |
| `queue_order` | Opcional, posição numérica inteira positiva na fila atual; vazio significa fora da fila. |

Datas desconhecidas e manutenção seguem [Common](../Shared/Common.md). Preserve a precisão conhecida: uma data sem horário não autoriza acrescentar `00:00`. Preparar o texto ou agendá-lo não comprova publicação.

| post_status | Significado |
| --- | --- |
| `draft` | Texto em desenvolvimento. |
| `review` | Texto em revisão antes da publicação. |
| `ready` | Conteúdo pronto para publicar. |
| `posted` | Publicação realizada e comprovada. |
| `archived` | Trabalho retirado da fila de produção, preservando seu registro. |

Agendar um conteúdo pronto mantém `ready` até a publicação. `review` não significa análise de desempenho: coletar dados ou escrever uma review não muda um post `posted`. Publicações realizadas permanecem `posted`.

## Fila de publicação

`queue_order` é opcional e pertence somente à nota principal do post. Use **Número**, com inteiro positivo sem aspas: 1, 2, 3… A posição se refere à fila atual; não conta publicações históricas. Campo ausente ou vazio significa fora da fila. Não é preciso criar tags, datas planejadas ou um vínculo adicional ao plano para participar.

O [Publishing Control](../../../Publishing%20Control.md) apresenta os valores dos próprios posts em uma Base nativa. O plano em vigor explica os critérios de seleção e a sequência desejada; a pessoa ou a IA, quando encarregada, registra a ordem escolhida nos posts. A documentação não atribui prioridade a conteúdos existentes.

| Operação | Atualização nos registros, pela pessoa ou IA encarregada |
| --- | --- |
| Incluir no fim | Preencha a próxima posição da fila atual. |
| Inserir ou mover | Escolha a posição e ajuste os demais itens afetados para manter 1, 2, 3… sem empates. |
| Retirar da fila | Limpe o campo e ajuste as posições seguintes. |
| Publicar ou arquivar | Atualize o estado conforme o fato, limpe a posição e reorganize os itens restantes. |

A visão inicial inclui posts com `draft`, `review` ou `ready` e posição válida. Apenas notas homônimas diretamente em `Posts/<Nome>/<Nome>.md` participam; README, Analytics, Reviews, Sources e Assets ficam fora. Posts `posted` e `archived` não aparecem nessa visão, mesmo que uma posição antiga ainda precise ser limpa.

Os filtros adicionais, colunas e outras visões são escolhidos pela pessoa: por exemplo, somente `ready` ou `ready` junto com `draft`. Propriedades e tags próprias podem ser acrescentadas quando úteis. Filtrar não altera a ordem registrada: se os itens visíveis são 2 e 5, continuam 2 e 5. Reorganize considerando a fila completa, incluindo itens ocultos por filtros. Alterar uma propriedade pela tabela altera a nota original.

Na Base, os filtros de **All views** limitam a tabela aos pacotes de `Posts/` deste módulo e a posições numéricas inteiras positivas; os de **This view** definem o recorte de trabalho e podem variar entre visões. Em **Properties**, escolha as colunas; para preservar a sequência, mantenha `queue_order` crescente em **Sort**. A tabela fica vazia enquanto nenhum post tiver posição válida e um estado incluído na visão. Referências do Obsidian: [Bases](https://obsidian.md/help/bases) e [filtros e ordenação](https://obsidian.md/help/bases/views).

Bases não faz renumeração, publicação ou agendamento. A pessoa pode pedir à IA que reorganize a fila; com escrita e autorização, ela pode fazer essa manutenção e conferir a sequência completa. Verifique os valores efetivamente registrados, inclusive nos itens ocultos por filtros. Mudar a posição altera só uma Property e não atualiza `updated_at`, conforme [Common](../Shared/Common.md#datas). Um filtro alterado não muda a nota. Na primeira utilização em outro vault, confira que `queue_order` está com tipo **Número** em Properties; valores vazios não selecionam o tipo por si só.

## Como preencher

| Seção do template | O que registrar |
| --- | --- |
| Objetivo e leitor | Finalidade da publicação e valor para quem a lê. |
| Origem do trabalho | Ideias de origem ou contexto de uma criação direta; não invente uma ideia intermediária. |
| Referências e materiais utilizados | Fontes que sustentam o texto produzido, com indicação de seu uso. |
| Afirmações e pontos a verificar | O que está sustentado, seus limites e o que ainda exige conferência. |
| Rascunho | Texto em desenvolvimento, com perguntas ou possibilidades identificadas como provisórias. |
| Texto final | Versão exata destinada à publicação; preserve a versão realmente utilizada. |
| Decisão visual | Se uma peça ajuda, qual foi escolhida e onde encontrá-la; não atribua uso publicado sem confirmação. |
| Registro de publicação | Fatos de aprovação, agendamento e publicação efetivamente conhecidos. |
| Registros relacionados | Links pertinentes para fontes, dados, avaliações e trabalho estratégico. |

Referências novas descobertas durante a produção pertencem ao trabalho do post. Não sincronize automaticamente essas descobertas de volta às ideias de origem. Material factual local fica em `Sources/`; material visual, em `Assets/`, com `Assets/Source/` para a origem editável da peça. Crie as áreas somente quando houver conteúdo.

Os dados observados ficam em `Analytics/`, conforme o [guia de Analytics Snapshot](Analytics%20Snapshot.md). A interpretação individual fica em `Reviews/`, conforme o [guia de Review](Review.md). A nota principal pode apontar para esses registros sem duplicar suas métricas ou conclusões.

## Template e controle

O arquivo inserível é [Templates/Post.md](../../../Templates/Post.md). A tabela descreve esse arquivo, não o registro criado com ele; as Properties no topo desta página descrevem o próprio guia.

| Template | created_at | updated_at | version |
| --- | --- | --- | --- |
| [Post](../../../Templates/Post.md) | 2026-10-21 | 2026-10-21 | `1.0.0` |
