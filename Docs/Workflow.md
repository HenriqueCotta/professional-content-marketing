---
created_at: 2026-10-20
updated_at: 2026-10-26
version: 1.1.2
---

# Fluxo de trabalho

Este guia explica as transições entre os trabalhos. Os guias de Models definem os registros; [Sources](Sources.md) orienta a pesquisa e [Strategy](Strategy.md) organiza direção e execução.

## Trabalhar por conversa ou diretamente nos arquivos

O caminho recomendado é pedir o resultado a uma IA com acesso à sua cópia do PCM. Com as ferramentas e a autorização necessárias, ela pode consultar o contexto e criar ou atualizar os registros conforme o pedido; a execução precisa ser conferida pelos meios disponíveis. Você pode fazer as mesmas operações diretamente nos arquivos, pelo Obsidian ou outro editor, ou dividir o trabalho com a IA. [Getting Started](Getting%20Started.md) explica como começar e [Access and Sync](Access%20and%20Sync.md) como disponibilizar e sincronizar sua cópia.

Você pode pedir consultas, produção, organização, comparação e manutenção, combinando essas operações conforme a necessidade. Os exemplos abaixo são ilustrativos e não exaustivos: não definem um catálogo de funcionalidades, comandos obrigatórios ou as únicas tarefas possíveis. O alcance da execução depende do acesso e das ferramentas da IA; os modelos e as escolhas reais continuam orientando o resultado.

| Exemplo de pedido à IA | Resultado no PCM, com o acesso necessário | Alternativa direta nos arquivos |
| --- | --- | --- |
| “Quais ideias ativas tenho sobre este assunto?” | Consulta das notas e seleção com links, sem mudar estados. | Consultar Ideas por conteúdo, estado, tags ou links. |
| “Registre esta experiência e prepare um post para este público.” | Registros pertinentes, baseados no relato e nos materiais disponíveis; pode haver um post direto ou uma ideia a desenvolver. | Criar o pacote, aplicar o template do tipo e preencher o conteúdo. |
| “Mostre os posts em revisão, os prontos e a ordem da fila; coloque este antes daquele.” | Consulta dos estados e, quando solicitada, atualização das posições afetadas na fila completa. | Consultar as notas ou o Publishing Control e editar as Properties pertinentes. |
| “Compare estes resultados com meu plano e registre o aprendizado.” | Avaliação sustentada nos dados acessíveis, nos registros correspondentes, com limites e pendências explícitos. | Ler os dados e atualizar a review ou avaliação pertinente. |

Os percursos seguintes explicam onde cada trabalho fica. Não são uma sequência obrigatória: você pode começar por um post, consultar o acervo sem criar nada ou retomar somente a parte necessária. O [AI Guide](AI%20Guide.md) orienta como a IA executa e verifica essas tarefas.

## Registrar uma ideia

Uma observação, pergunta ou argumento pode começar com poucas linhas. Crie diretamente um pacote em Ideas, com pasta e nota principal homônimas, seguindo o [guia de Idea](Models/Ideas/Idea.md). Não agrupe ideias por tema em diretórios intermediários; tags e links podem relacioná-las.

Anotar não é assumir um compromisso de publicação. A ideia pode ser aprofundada, retomada, reutilizada ou arquivada com motivo. Perguntas continuam perguntas até haver evidências. Antes de desenvolver um assunto semelhante, consulte ideias e posts relacionados.

## Investigar as afirmações

Consulte primeiro os materiais existentes. Uma referência simples pode ficar na nota; capturas e análises específicas entram em Sources do pacote quando necessárias. Siga o [guia de Local Source](Models/Shared/Local%20Source.md) para notas autorais de apoio e [Sources](Sources.md) para decidir localização, contexto e reutilização.

Registre o que foi observado, o que é interpretação e os limites. Uma prova pode levar à revisão da ideia; isso não exige produzir um post.

## Produzir uma publicação concreta

Quando a intenção for produzir uma publicação, crie seu pacote e nota principal em Posts, seguindo o [guia de Post](Models/Posts/Post.md). O post pode vir de uma ou várias ideias ou começar diretamente. Não crie uma ideia artificial apenas para preencher uma relação.

A pessoa pode pedir uma primeira versão completa, sugestões de enfoque, uma revisão de trecho ou desenvolvimento em conversa, por exemplo; são possibilidades combináveis, sem sequência obrigatória. A participação e as dúvidas que precisam de resposta dependem do pedido e do contexto, conforme [Participação e delegação](AI%20Guide.md#participação-e-delegação).

O tamanho de uma ideia não determina a transição. Preserve suas notas de origem e selecione no post as referências pertinentes ao argumento efetivamente produzido. Novas descobertas do post permanecem no próprio trabalho; não precisam ser sincronizadas de volta às ideias ou à biblioteca.

Fontes factuais ficam em Sources; produção visual em Assets, com editáveis em Assets/Source. Consulte [Visual Identity](../Visual%20Identity/Visual%20Identity.md) quando houver trabalho visual. Crie áreas auxiliares somente quando houver material, conforme [Architecture](Architecture.md).

## Organizar a fila, revisar e publicar

Quando selecionar um post para a fila, registre sua posição em `queue_order` e consulte o [Publishing Control](../Publishing%20Control.md). Os critérios vêm do plano; a pessoa ou a IA encarregada faz a manutenção da sequência nos posts, conforme o [guia de Post](Models/Posts/Post.md#fila-de-publicação). A Base não faz essa manutenção sozinha. Ajuste filtros para o recorte desejado, sem renumerar a visão filtrada.

Revise texto, evidências, limites das afirmações e material visual. O guia de [Post](Models/Posts/Post.md) é a referência dos estados e fatos de publicação. Conteúdo preparado ou agendado não comprova publicação; registre o evento quando realmente ocorrer, com a precisão conhecida. Ao publicar, arquivar ou retirar um item da fila, limpe sua posição e ajuste os seguintes; mudar o estado ou um filtro não faz essa manutenção automaticamente.

## Registrar e interpretar os resultados

Preserve exports originais em Analytics/Raw e registre a coleta conforme o [guia de Analytics Snapshot](Models/Posts/Analytics%20Snapshot.md). Quando houver uma pergunta útil a avaliar, crie uma review com os snapshots efetivamente usados, seguindo o [guia de Review](Models/Posts/Review.md). Uma nova captura não exige automaticamente uma review.

Dados coletados e interpretação ficam em registros separados. Uma observação não demonstra causalidade. Correções da mesma avaliação e análises de novas janelas seguem a distinção do guia de Review, preservando interpretações anteriores relevantes.

## Avaliar o plano e decidir

O registro do plano reúne ações e a seção **Como avaliar** definida para aquele trabalho; seu preenchimento segue o [guia de Plan](Models/Strategy/Plan.md). Os dados continuam nos posts; a avaliação do conjunto fica no plano, com links para as evidências. Preserve os critérios iniciais e registre mudanças com data e motivo.

Um experimento é opcional e detalha um teste específico, conforme o [guia de Experiment](Models/Strategy/Experiment.md). Um registro de decisão reúne escolhas relevantes, com motivo e aplicação, conforme o [guia de Decision](Models/Strategy/Decision.md). Nem toda review exige experimento, decisão separada ou alteração da direção. Quando uma escolha mudar a orientação atual, atualize o documento responsável preservando seu histórico.

## Retomar o trabalho

Parta dos registros atuais e consulte somente os guias e materiais relevantes à tarefa. Você pode perguntar à IA onde parou, o que está pendente e qual o próximo passo, ou consultar essas informações nas notas. Registre no próprio trabalho o próximo passo ou a dúvida pendente. O [AI Guide](AI%20Guide.md) orienta verificação, lacunas e preservação de conteúdo; [Common](Models/Shared/Common.md) reúne convenções compartilhadas.
