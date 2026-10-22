---
created_at: 2026-10-21
updated_at: 2026-10-21
version: 1.0.0
---

# Common

Este guia reúne orientações pequenas compartilhadas. Cada seção indica seu contexto; estar em Shared não torna uma propriedade obrigatória para todos os arquivos. Campos e estados de cada tipo pertencem ao seu guia em Models. Os processos ficam em [Workflow](../../Workflow.md), [Sources](../../Sources.md) e [Strategy](../../Strategy.md).

## Tags e relações

Para notas autorais em que sejam úteis, tags temáticas são opcionais. A pessoa escolhe os termos; não há taxonomia obrigatória. Preserve valores existentes e evite listas equivalentes como tags, topics, domains e categories para a mesma finalidade.

Registre relações com links e contexto a partir de quem usa o material: post para ideias, review para snapshots, experimento para evidências e decisão para as escolhas que substitui. Não mantenha também listas manuais de consumidores nas duas pontas. Backlinks e busca podem revelar o caminho inverso.

Não acrescente `type`, `owner` ou IDs só para repetir o nome ou a localização. Identificadores existentes podem continuar quando forem úteis. O Publishing Control apresenta propriedades das notas dos posts; não mantém cópias desses registros nem herda seus campos no frontmatter do painel.

## Datas

Esta tabela define o significado dos campos quando o guia do tipo os prevê; não manda acrescentar todos a cada nota.

| Campo | Significado |
| --- | --- |
| `created_at` | Criação comprovada desta nota ou registro autoral. |
| `updated_at` | Última alteração substantiva do conteúdo desta nota. |
| `posted_at` | Publicação efetivamente disponibilizada. |
| `captured_at` | Coleta dos dados documentados. |
| `reviewed_at` | Avaliação registrada pela review. |
| `started_at` | Início real da execução do plano. |

Use `YYYY-MM-DD` quando somente o dia estiver conhecido. Preserve hora e fuso comprovados quando forem relevantes. Não complete uma data com horário inventado, como `00:00`; um evento desconhecido continua com campo vazio.

Criação não é publicação, captura ou início da experiência narrada. O nome antigo e os timestamps do sistema de arquivos não comprovam criação original. Git pode ajudar a verificar o histórico, mas a primeira aparição após uma importação também não comprova a criação original.

`updated_at` acompanha mudanças no conteúdo da nota. Copiar, renomear, formatar, corrigir links ou alterar apenas Properties, como estado, posição na fila ou URL, não o atualiza. Uma reorganização não comprova coleta, avaliação ou revisão dos fatos. A data de atualização também não certifica que todas as informações estejam atuais. Registre mudanças substantivas sem apagar interpretações anteriores que tenham orientado decisões.

## Nomes e links

Notas autorais e pacotes usam nomes descritivos sem prefixo de data. Pacotes de ideia, post e biblioteca têm nota principal homônima. Datas que integram o título oficial de uma fonte continuam no nome.

Preserve nomes de arquivos originais, como PNG, XLSX e PDF. Eles não precisam receber frontmatter nem uma nota auxiliar apenas para forçar metadados. O nome especial de snapshots e reviews é explicado no [modelo de Analytics Snapshot](../Posts/Analytics%20Snapshot.md).

Prefira links Markdown com caminho relativo explícito e espaços codificados como `%20`. Confira o destino antes de renomear. Dentro de Properties, links internos usam wikilinks entre aspas, não Markdown; qualifique o destino quando houver nomes semelhantes. A origem do raciocínio não é uma herança automática de todas as fontes citadas.

## Versões

Aplica-se a Docs, modelos inseríveis, Direction e Plan, nos locais de controle definidos nos respectivos guias. A forma é `MAJOR.MINOR.PATCH`, inspirada no [Semantic Versioning 2.0.0](https://semver.org/spec/v2.0.0.html). Os critérios editoriais deste módulo são:

| Parte | Quando incrementar |
| --- | --- |
| MAJOR | Substituir uma orientação relevante ou mudar o contrato de forma que trabalhos anteriores precisem ser revistos. |
| MINOR | Acrescentar conteúdo ou capacidade compatível, como uma seção opcional. |
| PATCH | Corrigir apresentação ou precisão mantendo o significado que orienta a ação. |

Ao mudar MAJOR, zere MINOR e PATCH; ao mudar MINOR, zere PATCH. A importância depende do efeito: uma palavra pode inverter uma regra, enquanto uma reorganização extensa pode preservar o sentido. Uma correção factual que muda uma conclusão não é PATCH apenas por ser chamada de correção.

Uma página nova e preenchida pode começar em `1.0.0`. Preserve versões existentes dos modelos reutilizáveis. Direction e Plan só recebem uma primeira versão quando houver orientação ou plano real e estável; uma estrutura vazia não constitui baseline.

Atualização e versão são diferentes. Registrar execução pode alterar `updated_at` sem redefinir a versão do plano. Uma avaliação compatível pode justificar MINOR; trocar objetivo ou critério pode exigir MAJOR, preservando o plano inicial e o motivo. Corrigir links não redefine a data de alteração substantiva.

O número da versão não guarda conteúdos anteriores. Git só preserva revisões commitadas; salvar o arquivo não cria esse histórico. Não crie cópias numeradas de Direction ou pastas de versões como substituto automático.

## Guia, template e registro gerado

O frontmatter de uma página de Docs descreve a própria página: `created_at`, `updated_at` e `version`. Cada guia de modelo mantém uma linha equivalente para o template associado. Ao editar um template, atualize essa linha e a página quando cabível; não mantenha outro catálogo manual com os mesmos valores.

Os arquivos de `Templates/` contêm apenas as Properties e seções do registro gerado. Não acrescente a eles metadados de manutenção do modelo. `version` no resultado de Direction ou Plan pertence ao registro de negócio e é independente da versão do template.

As variáveis nativas são resolvidas na inserção. Ao gerar por IA ou outro editor, substitua título e datas aplicáveis por valores reais, deixando desconhecidos vazios. Datas administrativas de criação só usam o dia atual quando a nota é realmente nova. Datas de evento continuam dependentes de comprovação. Veja [Getting Started](../../Getting%20Started.md#aplicar-um-template-no-obsidian).

## Sugestões de status

Aplica-se às propriedades de estado declaradas nos guias de Idea, Library Source, Post, Plan e Experiment. Elas têm nomes separados por tipo. O autocomplete do Obsidian reúne valores utilizados sob o mesmo nome de propriedade no vault inteiro; não cadastra automaticamente todas as opções descritas nos guias e não impede outros valores digitados.

Templates também são notas e seus estados iniciais podem aparecer nas sugestões. Duas cópias no mesmo vault compartilham sugestões de uma mesma propriedade. Digite um estado previsto no guia se ele ainda não aparecer; não crie notas fictícias para popular sugestões. Referência de comportamento: [fórum do Obsidian](https://forum.obsidian.md/t/expand-types-json-with-display-name-and-suggestion-options/101456/4).
