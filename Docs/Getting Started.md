---
created_at: 2026-10-20
updated_at: 2026-10-26
version: 1.2.2
---

# Primeiros passos

O caminho recomendado é orientar uma IA para executar um trabalho real pequeno no PCM. A pessoa define objetivos e escolhas; a IA trabalha conforme o acesso e a autorização disponíveis. Os arquivos preparados sem conteúdo profissional não definem sua trajetória, direção, metas ou resultados. Preserve os registros que já existirem.

Você pode delegar inclusive uma primeira versão inteira e avaliar depois, ou participar durante o desenvolvimento, entre outras combinações. A forma de interação acompanha o pedido; não há uma rodada de perguntas obrigatória antes de cada tarefa. Consulte [Participação e delegação](AI%20Guide.md#participação-e-delegação).

## Começar com uma IA

1. Use seu repositório pessoal no GitHub como base principal ou uma pasta local como alternativa. Mantenha juntos Docs, Templates e as áreas de trabalho. Configure o acesso conforme [Access and Sync](Access%20and%20Sync.md).
2. Disponibilize essa localização à IA. Confira se a sessão consegue ler os arquivos atuais e se pode editá-los; uma conexão ao repositório não garante escrita.
3. Nas instruções persistentes do projeto ou ambiente da IA, coloque a [instrução para a IA](#instrução-para-a-ia), substituindo a localização pela sua cópia do PCM.
4. Faça um pedido concreto, como “Organize estas anotações como uma ideia no PCM e registre as referências que forneci”. Esse exemplo não limita os trabalhos possíveis nem muda as regras de cada registro.
5. Confira o resultado, os arquivos produzidos e as informações que continuaram em aberto. Retome a partir do próximo passo registrado no trabalho.

Com leitura e escrita, a IA pode aplicar as alterações dos arquivos abrangidos pelo pedido, sem pedir uma confirmação a cada arquivo. Com acesso somente de leitura, pode analisar e preparar o conteúdo ou as alterações para aplicação pelos meios disponíveis. A sincronização segue o escopo autorizado: editar arquivos não autoriza por si só commit ou push. Consulte [Access and Sync](Access%20and%20Sync.md) para manter uma cópia de trabalho coerente.

O [README](../README.md) encaminha aos guias. [AGENTS](../AGENTS.md) roteia a tarefa; [AI Guide](AI%20Guide.md) orienta a colaboração. Mantenha os detalhes dos modelos e processos nos guias do PCM, sem duplicá-los na instrução externa. Consulte somente o contexto necessário à tarefa.

## Instrução para a IA

Copie o texto abaixo para as instruções persistentes do projeto ou ambiente da IA e substitua `<...>` pela localização real da pasta do PCM. Ele define como consultar e aplicar o sistema; as regras de cada registro continuam nos guias. A ferramenta precisa ter acesso aos arquivos: informar a localização não cria a conexão nem concede permissão de edição.

```text
O PCM deste projeto está em <URL da pasta do PCM no meu repositório ou caminho local>. Use seus arquivos atuais como referência para organizar e executar o trabalho.

Antes de cada tarefa ou retomada, leia o AGENTS.md dessa pasta. A partir dele, consulte os guias, modelos e registros necessários para compreender o pedido e trabalhar corretamente. Uma leitura anterior ou a memória da conversa não substituem essa consulta atualizada.

Durante a execução, considere conjuntamente as orientações pertinentes e o contexto dos registros envolvidos. Reconsulte os documentos quando o escopo mudar, surgir uma dúvida ou uma alteração afetar o trabalho. Selecione o contexto pela necessidade da tarefa, sem carregar todo o acervo indiscriminadamente.

Antes de concluir, confira se o resultado segue o PCM e preserva as informações existentes. Se faltar acesso ou alguma orientação necessária estiver indisponível ou conflitante, explicite a limitação em vez de presumir conformidade.

As regras e convenções permanecem centralizadas no PCM; esta instrução estabelece como consultá-las e aplicá-las.
```

## Escolher o primeiro trabalho

Com IA, diretamente nos arquivos ou combinando os dois, escolha o guia correspondente ao que quer registrar. Estes são pontos de partida frequentes, não uma lista completa; os demais tipos estão nos [modelos do README](../README.md#modelos):

- Um pensamento, pergunta ou argumento, mesmo curto: siga o [guia de Idea](Models/Ideas/Idea.md). Crie diretamente seu pacote e uma nota homônima em Ideas.
- Uma publicação concreta: siga o [guia de Post](Models/Posts/Post.md). Pode começar diretamente ou usar ideias existentes.
- Uma referência que decidiu preservar na biblioteca: siga o [guia de Library Source](Models/Source%20Library/Library%20Source.md).
- Seu contexto profissional: siga o [guia de Deep Dive](Models/Deep%20Dive/Deep%20Dive.md), com experiências e evidências reais.

Preencha só o que conhece. Não crie exemplos de negócio para completar pastas. Se precisar de pesquisa, siga [Sources](Sources.md); fontes simples podem continuar como links na nota.

## Quando houver uma direção e um plano

Registre escolhas editoriais reais no único `Strategy/Direction.md`, seguindo o [guia de Direction](Models/Strategy/Direction.md). Quando quiser acompanhar ações e resultados, crie um plano no destino definido pelo [guia de Plan](Models/Strategy/Plan.md). O próprio registro do plano inclui **Como avaliar**, com medidas, fontes, janelas, critérios e limites escolhidos para aquele trabalho.

A rotina completa está em [Workflow](Workflow.md), e a relação entre direção, planos, testes e decisões em [Strategy](Strategy.md). Experimentos só são criados quando houver uma pergunta específica a testar.

## Usar diretamente ou combinar formas de trabalho

O PCM pode ser lido e editado sem IA, em um editor Markdown. Obsidian é uma opção para navegar pelas notas, inserir templates e visualizar a fila em uma Base. Para usá-lo, abra a pasta completa como vault independente ou mantenha-a dentro do seu vault. As mesmas regras dos registros valem nas formas manual, assistida e combinada; [Architecture](Architecture.md) explica os destinos.

## Aplicar um template no Obsidian

1. Em **Settings → Core plugins**, habilite **Templates**, se necessário.
2. Em **Settings → Core plugins → Templates → Template folder location**, selecione a pasta `Templates` deste módulo. Em um vault próprio, use `Templates`; em um vault maior, use `<caminho do módulo>/Templates`, relativo à raiz do vault.
3. Crie uma nota nova vazia no destino correto e dê a ela o nome definitivo. Para ideia, post e biblioteca, crie primeiro o pacote homônimo.
4. Com a nota ativa, use **Ctrl+P → Templates: Insert template** e escolha o modelo indicado no guia do tipo.
5. Preencha o conteúdo real e confira Properties, estados e datas conforme esse guia.

O seletor nativo usa uma pasta por vault. Trocar a preferência muda a lista oferecida e conserva os arquivos da pasta anterior. Copiar este módulo não configura automaticamente o seletor de outro vault. Aponte para `Templates/`, onde estão os arquivos inseríveis, e não para Docs ou a raiz do módulo.

`{{title}}` usa o nome da nota; `{{date:YYYY-MM-DD}}` usa o dia da inserção. Variáveis ficam entre aspas no YAML; edite os templates em modo Source. A inserção ocorre na nota ativa e não cria seus diretórios. `updated_at` não acompanha futuras edições automaticamente.

O guia de cada tipo explica quais datas recebem o dia de criação e quais permanecem vazias. Publicação, coleta, avaliação e início da execução só são preenchidos quando conhecidos. Ao gerar por IA ou outro editor, resolva as variáveis antes de salvar.

### Trabalhar em uma nota existente

Direction e Visual Identity já vêm preparadas. Preserve suas Properties e valores conhecidos e acrescente somente as seções necessárias a partir do corpo do template. Reaplicar o arquivo completo pode duplicar seções e mesclar Properties. A inserção não prova que uma nota antiga foi criada ou revisada hoje.

## Organizar a fila

A pessoa ou uma IA autorizada mantém `queue_order` nas notas dos posts, seguindo o [modelo de Post](Models/Posts/Post.md#fila-de-publicação). Alterar um estado ou um filtro não atualiza as posições registradas automaticamente.

Para visualizar no Obsidian, confira **Settings → Core plugins → Bases** e abra o [Publishing Control](../Publishing%20Control.md). Preencha `queue_order` como **Número** na nota principal do post, começando em 1. Se o campo ainda não existir, acrescente-o em Properties; não reaplique o template inteiro. O painel começa com os estados `draft`, `review` e `ready`; use **Filter → This view** para escolher outro recorte. Em outro editor ou por IA, os valores permanecem nos arquivos; a tabela dinâmica depende de Bases no Obsidian.

## Retomar e preservar o trabalho

Parta da nota em andamento, confira seu próximo passo e siga apenas os links relevantes. Com IA, indique esse trabalho na retomada e use a mesma entrada em [AGENTS](../AGENTS.md).

As convenções compartilhadas estão em [Common](Models/Shared/Common.md). Git pode preservar o histórico se configurado e usado com commits; o número de versão sozinho não reconstrói o conteúdo anterior. Você não precisa configurar Git para começar, mas deve saber qual histórico está efetivamente preservado.

Referências do recurso nativo: [Templates](https://obsidian.md/help/plugins/templates) e [Properties](https://obsidian.md/help/properties).
