---
created_at: 2026-10-21
updated_at: 2026-10-26
version: 1.0.1
---

# Experiment

Esta página é o guia do tipo Experiment. Seu frontmatter descreve o guia; a seção Properties descreve os registros produzidos. Os destinos abaixo seguem a [convenção de raiz do PCM](../../Architecture.md#guia-template-e-registro-de-trabalho).

## Finalidade e localização

Um experimento investiga uma hipótese específica por meio de uma mudança deliberada e de uma comparação útil. Cada registro fica em `Strategy/Experiments/`, com nome descritivo. Pode ocorrer dentro de um plano ou atravessar vários; nenhum plano precisa conter um experimento. Consulte o [manual de estratégia](../../Strategy.md) para distinguir investigação de acompanhamento da produção.

## Properties e estados

| Campo | Significado |
| --- | --- |
| `experiment_status` | Andamento do teste, separado do resultado da hipótese. |
| `created_at` | Criação comprovada do registro autoral. |
| `updated_at` | Última alteração substantiva do registro. |

| Estado | Quando usar |
| --- | --- |
| `planned` | Teste planejado, ainda não iniciado. |
| `running` | Teste em execução. |
| `closed` | Teste encerrado, inclusive quando interrompido ou inconclusivo. |

As [convenções comuns](../Shared/Common.md) orientam o preenchimento das datas. `closed` não significa hipótese apoiada; a avaliação fica no corpo.

## Como preencher

- **Hipótese e motivação:** declare a pergunta e por que vale investigá-la, sem antecipar uma conclusão favorável.
- **Plano inicial e critérios:** descreva a mudança, as condições que se pretende manter semelhantes, as evidências e janelas previstas e os critérios de avaliação antes da execução.
- **Publicações e comparação:** vincule os trabalhos comparados e registre outras diferenças que possam influenciar o resultado.
- **Adaptações durante o teste:** preserve o plano original e explique mudanças com data e motivo.
- **Resultados e evidências:** registre o observado e os links para as coletas e avaliações utilizadas.
- **Avaliação e limitações:** explique se a hipótese foi apoiada, não apoiada, ficou inconclusiva ou não chegou a ser avaliada. Delimite as condições em que a conclusão vale.
- **Encaminhamento:** registre a decisão seguinte ou o motivo de interrupção, sem apagar um teste porque não produziu o resultado esperado.

Uma diferença de desempenho não comprova sua causa. Compare apenas o que as evidências permitem e preserve interpretações anteriores que tenham orientado decisões.

## Template e controle

O arquivo inserível é [Templates/Experiment.md](../../../Templates/Experiment.md). A tabela descreve esse arquivo, não o registro criado com ele; as Properties no topo desta página descrevem o próprio guia.

| Template | created_at | updated_at | version |
| --- | --- | --- | --- |
| [Experiment](../../../Templates/Experiment.md) | 2026-10-21 | 2026-10-21 | `1.0.0` |
