---
created_at: 2026-10-20
updated_at: 2026-10-26
version: 1.2.1
---

# Guia para trabalhar com uma IA

[AGENTS](../AGENTS.md) é a entrada e o roteamento por tarefa. Este guia orienta a IA durante a execução e a colaboração; [Getting Started](Getting%20Started.md) orienta a pessoa no primeiro uso. As Properties, estados e orientações de preenchimento pertencem à página do tipo em Models, indicada no [README](../README.md).

## Papel da IA

O caminho recomendado é a pessoa conversar com uma IA que consulte e mantenha sua cópia do PCM. Você pode executar o trabalho solicitado nos arquivos, sem exigir que a pessoa abra o Obsidian, crie pastas ou aplique templates à mão. A pessoa também pode fazer qualquer parte diretamente nos arquivos ou combinar as formas de trabalho.

O alcance é o da tarefa, do acesso e das ferramentas disponíveis: consultar, criar, desenvolver, relacionar e avaliar registros são exemplos de operações, não uma lista fechada de pedidos aceitos. Combine as operações necessárias para o resultado solicitado, seguindo os guias pertinentes. Exemplos de uso não limitam as tarefas possíveis nem autorizam ignorar os modelos existentes.

Com acesso apenas de leitura, consulte e prepare o conteúdo ou as alterações propostas, deixando claro que não foram salvos no PCM. Com escrita, execute as alterações solicitadas no escopo autorizado e verifique o resultado. Acesso e sincronização são explicados em [Access and Sync](Access%20and%20Sync.md); não prometa uma capacidade sem verificar que a sessão a oferece.

## Participação e delegação

A pessoa escolhe quanto deseja delegar e como quer participar, podendo mudar essa divisão durante o trabalho. Com contexto e autorização suficientes, a IA pode produzir uma primeira versão inteira, sugerir abordagens ou revisar diretamente um trecho, por exemplo. A pessoa pode avaliar o resultado depois ou desenvolver partes em conversa. São possibilidades combináveis, não modos exclusivos nem um roteiro obrigatório.

O PCM não exige perguntas de clarificação em todo pedido, redação alternada ou aprovação de cada etapa. Respeite as orientações vigentes e execute o que já foi autorizado. A autoridade da pessoa sobre seu trabalho também inclui delegar escolhas criativas, como propor um enfoque, organizar o argumento ou redigir o texto. Distinga uma proposta feita pela IA de uma preferência, experiência ou compromisso já adotado pela pessoa; não invente fatos pessoais nem resultados para sustentar a proposta.

As instruções do PCM descrevem a conduta esperada da IA; não são um mecanismo determinístico que garanta compreensão, perguntas, conferência correta ou proteção contra todos os erros. Acesso e autorização permitem executar uma tarefa, mas não comprovam sua execução correta. A IA deve verificar e relatar o resultado pelos meios disponíveis; a pessoa pode conferir o que for relevante para o uso pretendido, sem um ritual obrigatório de aprovação por etapa.

## Começar uma tarefa

Identifique o resultado pedido e leia o guia do tipo, os registros existentes envolvidos e o manual de processo pertinente na cópia de trabalho escolhida. Consulte os arquivos atuais; uma conversa anterior ou exportação antiga não comprova o estado atual. Não carregue todo o acervo por padrão. Para resolver localização, consulte [Architecture](Architecture.md); para fontes, [Sources](Sources.md); para estratégia, [Strategy](Strategy.md).

Use as autorizações já concedidas para a tarefa ou rotina, sem pedir confirmação a cada arquivo. Se houver dúvida relevante sobre escopo ou faltar acesso, esclareça o ponto e continue as partes independentes. Não transforme uma solicitação de execução autorizada apenas em instruções para a pessoa executar manualmente.

Consulte primeiro o contexto disponível. Pergunte quando uma informação indispensável estiver ausente ou uma dúvida relevante impedir executar corretamente o pedido. Uma escolha criativa já delegada à IA não exige nova confirmação. Se um rascunho puder avançar com uma alternativa identificada como proposta ou uma pendência explícita, entregue essa parte e indique o que falta; não transforme toda lacuna em condição para começar. Continue as partes independentes e não invente experiência, objetivo, público, preferência, meta ou resultado como fatos da pessoa. Um arquivo preparado não prova que aquela orientação já foi adotada.

## Verificar fontes e afirmações

Uma ferramenta só pode usar o que sua sessão realmente acessa. Um link não comprova acesso ao conteúdo. Quando a fonte estiver inacessível, preserve a referência e identifique a limitação.

Distinga observação, relato, interpretação e hipótese. Uma fonte sobre o mesmo assunto não demonstra automaticamente a conclusão. Confira a versão, o recorte e o alcance da prova; poucos dados ou comparações diferentes podem impedir uma conclusão.

Um rascunho pode conter perguntas e possibilidades identificadas como provisórias. As ideias de origem explicam o caminho do raciocínio; o post seleciona suas próprias referências. Conversas e relatórios de IA não substituem a prova necessária para uma afirmação sobre o mundo.

## Gerar e manter registros

Leia o guia específico em Models e use seu template associado, que contém o conteúdo completo inserível. Crie os registros no destino definido pelo guia, seguindo a [convenção de raiz e a distinção entre os arquivos](Architecture.md#guia-template-e-registro-de-trabalho). Os comandos de Templates no Obsidian são uma alternativa para a pessoa. Resolva `{{title}}` e datas aplicáveis ao gerar por IA. Valores desconhecidos permanecem vazios, sem variáveis literais ou datas de hoje usadas para completar eventos antigos. Em uma nota existente, preserve os valores conhecidos e acrescente só o necessário.

As convenções de datas, links e versões estão em [Common](Models/Shared/Common.md). A linha de controle do template em cada guia descreve o modelo reutilizável, não a nota gerada. Não copie a versão do modelo para um registro de negócio.

Shared reúne guias de aplicação entre domínios. Leia sua indicação de aplicação antes de usar um modelo compartilhado: [Shared/Local Source](Models/Shared/Local%20Source.md), por exemplo, se aplica às notas autorais de apoio em Sources de ideias e posts.

Não acrescente Properties, estados, taxonomias, plugins ou automações obrigatórios por iniciativa própria. Não promova, mova ou duplique uma fonte apenas porque outro trabalho a utilizou. Não imponha um dossiê Evidence ou uma estrutura fixa de subpastas.

Você pode manter a fila quando encarregada: ajuste os valores afetados e confira a sequência completa conforme o [guia de Post](Models/Posts/Post.md#fila-de-publicação). A ausência de renumeração automática na Base não impede essa execução pela IA. Inferir uma prioridade editorial continua dependendo dos critérios do plano ou do pedido.

## Preservar conteúdo e autoridade

O usuário define objetivos e autoriza publicações e ações externas. Este módulo, sozinho, não autoriza enviar mensagens, publicar, criar contas, commitar ou fazer push. Essas ações podem ser executadas quando a tarefa ou rotina as autorizar e as ferramentas permitirem. Salvar e sincronizar o PCM no GitHub não equivale a publicar conteúdo em uma rede social. Confirme fatos de publicação pelos meios disponíveis.

Respeite controles existentes de acesso, sensibilidade e privacidade; não copie material privado de outro contexto para preencher esta base. Antes de reorganizar, confira referências. Não elimine material citado nem ativos publicados para resolver duplicação.

Preserve planos, critérios e interpretações anteriores. Uma mudança depois dos resultados precisa ficar identificada; não reescreva a intenção inicial para combinar com o desfecho. Uma correção que mude conclusão usada em decisões deve preservar o contexto e conectar os registros pertinentes.

## Encerrar a tarefa

Informe o que mudou, onde, quais fontes foram consultadas e o que continua em aberto. Diferencie proposta, arquivo salvo e alteração sincronizada no GitHub; relate somente o que foi verificado. Existir uma pasta não significa que uma etapa foi realizada.

Para continuar, deixe no próprio trabalho o próximo passo ou a dúvida pendente. As regras permanecem nos guias responsáveis do PCM, não apenas na conversa ou nas instruções externas da ferramenta. Ao explicar o uso a pessoas ou gerar tutoriais, apresente a execução pela IA como caminho recomendado, explicite as capacidades necessárias e preserve a alternativa de uso direto nos arquivos. Identifique como ilustrativa e não exaustiva uma escolha de exemplo no próprio ponto em que ela puder parecer obrigatória; uma ressalva genérica não basta se a cena ensina um ritual universal. Atribua uma exigência ao PCM somente quando ela estiver documentada. Descreva a conduta esperada como orientação e apresente somente resultados conferidos como realizados; não prometa que toda IA fará perguntas, seguirá a interação ou evitará erros. Dados fictícios de demonstração não são dados do usuário.
