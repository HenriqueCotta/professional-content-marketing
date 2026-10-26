---
created_at: 2026-10-21
updated_at: 2026-10-26
version: 1.0.1
---

# Analytics Snapshot

Esta página é o guia do tipo Analytics Snapshot. Seu frontmatter descreve o guia; a seção Properties descreve os registros produzidos. Os destinos abaixo seguem a [convenção de raiz do PCM](../../Architecture.md#guia-template-e-registro-de-trabalho).

## Finalidade e localização

Um snapshot registra observações de desempenho de um post, com sua origem e janela. A publicação observada é documentada conforme o [guia de Post](Post.md). A nota autoral do snapshot fica em `Posts/<Nome do post>/Analytics/`. Preserve exports e outros dados brutos em `Analytics/Raw/`, mantendo os nomes e os arquivos originais.

Registre cada coleta sem sobrescrever os originais de outra. O snapshot guarda fatos e cálculos; a interpretação fica em uma review, conforme o [guia de Review](Review.md). Uma coleta nova não exige automaticamente uma review.

### Nome e cálculo de Day X

Quando a idade dos dados estiver demonstrada, use `Day X - Analytics Snapshot.md`. X é a idade da coleta desde a publicação, não a idade da nota ou o tempo desde sua edição:

```text
X = data local da captura − data local da publicação
```

A diferença é contada em dias de calendário, no fuso da publicação. O dia local da publicação é `Day 0`; a data local seguinte é `Day 1`. Não se contam blocos completos de 24 horas, nem se arredondam horas decorridas. `Day 7` não afirma que exatamente 168 horas foram observadas.

Quando houver timestamps com fuso, converta publicação e captura para o fuso da publicação antes de comparar as datas. Se os registros trouxerem somente o dia, use as datas documentadas, sem completar horários. Se diferenças de fuso puderem alterar o resultado e não houver informação suficiente, não atribua um X exato.

Sem data comprovada de publicação ou captura, use um nome descritivo sem Day X, como `Analytics Snapshot - Exportação inicial.md`. Não use a criação da nota, a data do rascunho ou o dia da cópia para preencher esses eventos.

Cuidados:

- Duas coletas no mesmo dia recebem um complemento descritivo ou horário comprovado para evitar colisão de nomes.
- Se a captura parecer anterior à publicação, confira a origem e os fusos; não transforme um valor negativo em `Day 0`.
- Uma republicação independente tem sua própria data de publicação e sua própria contagem.
- Um snapshot documentado posteriormente mantém a idade da coleta; edição, renomeação e correção de links não mudam X.
- Ao renomear, confira referências no post, nas reviews e no trabalho estratégico.

## Properties e estados

| Campo | Uso neste registro |
| --- | --- |
| `created_at` | Criação comprovada da nota autoral, que pode ser posterior à coleta. |
| `captured_at` | Data ou momento em que os dados foram coletados, preservando a precisão comprovada. |

O snapshot não recebe campo de estado no padrão mínimo. Datas desconhecidas permanecem vazias, conforme [Common](../Shared/Common.md). Uma migração não autoriza substituir criação ou captura por hoje.

## Como preencher

| Seção do template | O que registrar |
| --- | --- |
| Publicação e Raw utilizado | Link para o post e para o export ou material concreto utilizado; identifique uma origem pendente de conferência. |
| Origem e janela observada | Fonte, data da coleta, período coberto e limites conhecidos da observação. |
| Observações | Valores efetivamente disponibilizados, sem completar dados ausentes. |
| Cálculos | Fórmulas, unidades e denominadores, permitindo conferir os resultados. |
| Limitações dos dados | Indisponibilidade, divergências de origem, recortes e restrições de comparação. |

Ausência de dado não significa zero. Não preencha números por inferência nem transforme o snapshot em uma explicação causal do desempenho. Comparações exigem conferir definições, fontes e janelas, além do nome da medida.

## Template e controle

O arquivo inserível é [Templates/Analytics Snapshot.md](../../../Templates/Analytics%20Snapshot.md). A tabela descreve esse arquivo, não o registro criado com ele; as Properties no topo desta página descrevem o próprio guia.

| Template | created_at | updated_at | version |
| --- | --- | --- | --- |
| [Analytics Snapshot](../../../Templates/Analytics%20Snapshot.md) | 2026-10-21 | 2026-10-21 | `1.0.0` |
