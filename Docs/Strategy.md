---
created_at: 2026-10-20
updated_at: 2026-10-21
version: 1.0.1
---

# Como organizar a estratégia

Este guia explica como as partes estratégicas se relacionam. Campos, estados e preenchimento ficam nas páginas de cada modelo. As escolhas estratégicas pertencem à pessoa e devem refletir seu contexto real.

## Responsabilidades

| Parte | Pergunta que responde | Guia do registro |
| --- | --- | --- |
| Direction | Qual é a direção editorial atual? | [Direction](Models/Strategy/Direction.md) |
| Plans | O que vamos fazer e como avaliar esse trabalho? | [Plan](Models/Strategy/Plan.md) |
| Experiments | Qual hipótese específica vale testar? | [Experiment](Models/Strategy/Experiment.md) |
| Decisions | Qual escolha relevante foi feita e por quê? | [Decision](Models/Strategy/Decision.md) |

O contexto de Deep Dive sustenta as escolhas; Direction reúne objetivos, público, posicionamento, temas e limites definidos pela pessoa. Atualize o mesmo arquivo de direção. Um plano anterior conserva as escolhas e o contexto que orientaram sua execução, mesmo que a direção atual mude.

## Planejar e combinar como avaliar

Cada plano tem um arquivo próprio em Strategy/Plans. Nele ficam objetivo, ações, conteúdos previstos, acompanhamento e a seção **Como avaliar**. Outro plano recebe outro arquivo e pode usar medidas e critérios diferentes.

Na definição do plano, combine a pergunta de avaliação, as medidas ou observações, suas definições e fontes, a forma de coleta, a janela, os critérios de interpretação e as limitações. Não adote metas, métricas ou intervalos só porque outra pessoa os usa. Defina apenas o que fizer sentido para o objetivo e puder ser observado.

Os números e exports continuam em Analytics de cada post; interpretações individuais em Reviews. O plano aponta para os registros e avalia o conjunto. Não replique todos os dados nem transforme o plano em outro painel de métricas.

Se os critérios mudarem durante a execução, registre data, motivo e aplicação, preservando a definição inicial. Comparar planos exige conferir definição, unidade, fonte e janela das medidas; usar o mesmo nome não garante comparabilidade.

O plano explica os critérios de seleção e a sequência pretendida. A ordem operacional atual fica em `queue_order` nas notas dos posts e aparece no [Publishing Control](../Publishing%20Control.md), conforme [Post](Models/Posts/Post.md#fila-de-publicação). Não mantenha uma segunda fila sincronizada no plano; seus links preservam a seleção e o contexto relevantes ao acompanhamento. A fila pode mudar conforme o plano; a pessoa ou a IA encarregada atualiza os valores. Filtros e mudanças de estado não reorganizam as posições sozinhos.

## Executar, avaliar e decidir

Um plano pode produzir conteúdo e avaliar resultados sem nenhum experimento. Crie um experimento quando houver uma hipótese específica, mudança deliberada e uma forma útil de observar o resultado. Ele pode apoiar um plano ou atravessar mais de um, preservando seu próprio protocolo e as adaptações realizadas.

Uma métrica indisponível não vale zero. Um resultado melhor não demonstra sozinho que texto ou imagem causou a diferença. Distinga o observado, a interpretação e o que permanece sem resposta; registre limites e comparações inadequadas.

A avaliação do conjunto fica no próprio plano. Pode indicar o que repetir, interromper, investigar ou manter. Uma decisão separada só é necessária quando houver uma escolha relevante que mereça ser compreendida no futuro. Não há uma pasta obrigatória de retrospectivas ou princípios.

Quando uma decisão mudar a direção, atualize Direction. Quando mudar o que um plano fará ou avaliará, registre a aplicação nesse plano, preservando suas escolhas iniciais. Conecte decisões substituídas sem apagar o motivo anterior.

## Relação entre os registros

```text
Contexto profissional → Direction
                          ↓
             Plan: ações + Como avaliar
                 ├── Posts → Analytics → Reviews
                 └── Experiment opcional
                          ↓
              Avaliação no próprio Plan
                          ↓
               Decisions quando úteis
                          ↓
             Direção atual e próximos planos
```

O modelo não fixa duração, quantidade de posts ou calendário. Preserve o plano inicial e o histórico das escolhas. As convenções de versões e o alcance do histórico Git estão em [Common](Models/Shared/Common.md#versões).
