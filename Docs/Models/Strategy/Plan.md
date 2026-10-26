---
created_at: 2026-10-21
updated_at: 2026-10-26
version: 1.0.1
---

# Plan

Esta página é o guia do tipo Plan. Seu frontmatter descreve o guia; a seção Properties descreve os registros produzidos. Os destinos abaixo seguem a [convenção de raiz do PCM](../../Architecture.md#guia-template-e-registro-de-trabalho).

## Finalidade e localização

Cada plano tem seu próprio arquivo em `Strategy/Plans/`, com nome descritivo. Ele reúne objetivo, ações, forma de avaliação, acompanhamento e aprendizado. Atualize o mesmo registro durante sua definição, execução e fechamento; outro plano recebe outro arquivo. A pessoa escolhe duração, quantidade de conteúdos e limites. Consulte o [manual de estratégia](../../Strategy.md) para relacioná-lo à direção e aos experimentos opcionais.

## Properties e estados

| Campo | Significado |
| --- | --- |
| `plan_status` | Estado de execução do plano. |
| `updated_at` | Última alteração substantiva do registro. |
| `started_at` | Início real da execução; permanece vazio antes desse evento. |
| `version` | Edição do plano, segundo as [convenções comuns](../Shared/Common.md). |

| Estado | Quando usar |
| --- | --- |
| `draft` | Plano em elaboração; objetivo e ações ainda em definição. |
| `defined` | Objetivo e ações definidos, antes de iniciar a execução. |
| `active` | Execução iniciada. |
| `closed` | Plano encerrado, inclusive com ações abandonadas ou pendências registradas. |

O núcleo não inclui `created_at`. Datas e versão desconhecidas ficam vazias. O template começa em `draft`; passe para `defined` quando objetivo e ações estiverem definidos.

## Como preencher

- **Plano inicial:** registre objetivo, contexto, prioridades e limites. Preserve as escolhas de direção que orientaram o plano quando isso for necessário para compreendê-lo depois.
- **Como avaliar:** combine antes da execução a pergunta de avaliação; as medidas escolhidas, seu significado, unidade ou fórmula e fonte; a janela de coleta e comparação; os critérios para interpretar o resultado; e os limites conhecidos. Inclua o denominador de uma taxa quando houver. Esses critérios pertencem ao próprio plano e são escolhidos pela pessoa; não existem métricas ou metas obrigatórias.
- **Conteúdos previstos:** vincule ideias e posts selecionados, explicando a escolha e os critérios de sequência. A ordem operacional atual fica nos posts via `queue_order` e no [Publishing Control](../../../Publishing%20Control.md); siga o [guia de Post](../Posts/Post.md#fila-de-publicação), sem manter uma segunda fila manual sincronizada no plano.
- **Acompanhamento e alterações datadas:** registre execução, pendências e mudanças com data e motivo.
- **Evidências:** aponte para os dados em `Posts/<post>/Analytics/` e as interpretações individuais em `Reviews/`. O plano compara os registros pertinentes, sem absorver todas as coletas.
- **Avaliação do plano:** confronte o realizado com o objetivo e os critérios iniciais. Diferencie observação, interpretação e limitações; uma medida indisponível não significa zero.
- **Próximos passos:** explique o que continuar, interromper ou investigar e o que fica para outro plano.

Não reescreva critérios depois de conhecer o resultado para fazer o plano parecer bem-sucedido. Se houver mudança necessária, preserve o critério anterior e registre a nova escolha, sua data e seu motivo. Atualizar andamento pode mudar `updated_at` sem redefinir a versão; mudanças materiais seguem as convenções comuns. Encerrar não exige uma conclusão positiva nem resolver todas as perguntas.

## Template e controle

O arquivo inserível é [Templates/Plan.md](../../../Templates/Plan.md). A tabela descreve esse arquivo, não o registro criado com ele; as Properties no topo desta página descrevem o próprio guia.

| Template | created_at | updated_at | version |
| --- | --- | --- | --- |
| [Plan](../../../Templates/Plan.md) | 2026-10-21 | 2026-10-21 | `1.0.0` |
