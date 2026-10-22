---
created_at: 2026-10-20
updated_at: 2026-10-21
version: 1.0.0
---

# Fluxo de trabalho

Este guia explica as transições entre os trabalhos. Os guias de Models definem os registros; [Sources](Sources.md) orienta a pesquisa e [Strategy](Strategy.md) organiza direção e execução.

## 1. Registrar uma ideia

Uma observação, pergunta ou argumento pode começar com poucas linhas. Crie diretamente um pacote em Ideas, com pasta e nota principal homônimas, seguindo [Idea](Models/Ideas/Idea.md). Não agrupe ideias por tema em diretórios intermediários; tags e links podem relacioná-las.

Anotar não é assumir um compromisso de publicação. A ideia pode ser aprofundada, retomada, reutilizada ou arquivada com motivo. Perguntas continuam perguntas até haver evidências. Antes de desenvolver um assunto semelhante, consulte ideias e posts relacionados.

## 2. Investigar as afirmações

Consulte primeiro os materiais existentes. Uma referência simples pode ficar na nota; capturas e análises específicas entram em Sources do pacote quando necessárias. Use [Shared/Local Source](Models/Shared/Local%20Source.md) para notas autorais de apoio e [Sources](Sources.md) para decidir localização, contexto e reutilização.

Registre o que foi observado, o que é interpretação e os limites. Uma prova pode levar à revisão da ideia; isso não exige produzir um post.

## 3. Produzir uma publicação concreta

Quando a intenção for produzir uma publicação, crie seu pacote e nota principal em Posts, seguindo [Post](Models/Posts/Post.md). O post pode vir de uma ou várias ideias ou começar diretamente. Não crie uma ideia artificial apenas para preencher uma relação.

O tamanho de uma ideia não determina a transição. Preserve suas notas de origem e selecione no post as referências pertinentes ao argumento efetivamente produzido. Novas descobertas do post permanecem no próprio trabalho; não precisam ser sincronizadas de volta às ideias ou à biblioteca.

Fontes factuais ficam em Sources; produção visual em Assets, com editáveis em Assets/Source. Consulte [Visual Identity](../Visual%20Identity/Visual%20Identity.md) quando houver trabalho visual. Crie áreas auxiliares somente quando houver material, conforme [Architecture](Architecture.md).

## 4. Organizar a fila, revisar e publicar

Quando selecionar um post para a fila, preencha sua posição em `queue_order` e consulte o [Publishing Control](../Publishing%20Control.md). Os critérios vêm do plano; a manutenção da sequência é manual, conforme [Post](Models/Posts/Post.md#fila-de-publicação). Ajuste filtros para o recorte desejado, sem renumerar a visão filtrada.

Revise texto, evidências, limites das afirmações e material visual. O guia de [Post](Models/Posts/Post.md) é a referência dos estados e fatos de publicação. Conteúdo preparado ou agendado não comprova publicação; registre o evento quando realmente ocorrer, com a precisão conhecida. Ao publicar, arquivar ou retirar um item da fila, limpe sua posição e ajuste os seguintes; mudar o estado ou um filtro não faz essa manutenção automaticamente.

## 5. Registrar e interpretar os resultados

Preserve exports originais em Analytics/Raw e registre a coleta conforme [Analytics Snapshot](Models/Posts/Analytics%20Snapshot.md). Quando houver uma pergunta útil a avaliar, crie uma [Review](Models/Posts/Review.md) com os snapshots efetivamente usados. Uma nova captura não exige automaticamente uma review.

Dados coletados e interpretação ficam em registros separados. Uma observação não demonstra causalidade. Correções da mesma avaliação e análises de novas janelas seguem a distinção do guia de Review, preservando interpretações anteriores relevantes.

## 6. Avaliar o plano e decidir

O [Plan](Models/Strategy/Plan.md) reúne ações e a seção **Como avaliar** definida para aquele trabalho. Os dados continuam nos posts; a avaliação do conjunto fica no plano, com links para as evidências. Preserve os critérios iniciais e registre mudanças com data e motivo.

Um [Experiment](Models/Strategy/Experiment.md) é opcional e detalha um teste específico. Uma [Decision](Models/Strategy/Decision.md) registra escolhas relevantes, com motivo e aplicação. Nem toda review exige experimento, decisão separada ou alteração da direção. Quando uma escolha mudar a orientação atual, atualize o documento responsável preservando seu histórico.

## Retomar com uma IA

Parta da nota do trabalho e consulte somente os guias e materiais relevantes à tarefa. Registre no próprio trabalho o próximo passo ou a dúvida pendente. O [AI Guide](AI%20Guide.md) orienta verificação, lacunas e preservação de conteúdo; [Common](Models/Shared/Common.md) reúne convenções compartilhadas.
