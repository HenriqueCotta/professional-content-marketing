---
created_at: 2026-10-20
updated_at: 2026-10-21
version: 1.0.0
---

# Primeiros passos

Comece com um trabalho real pequeno. Os arquivos preparados sem conteúdo profissional não definem sua trajetória, direção, metas ou resultados. A cópia de trabalho pode já conter registros; preserve-os.

## Abrir o módulo

Copie a pasta completa para seu vault ou abra a pasta como um vault independente no Obsidian. Mantenha juntos Docs, Templates e as áreas de trabalho. Também é possível usar um editor Markdown; Git e uma IA são opcionais.

O [README](../README.md) aponta para cada guia. Consulte [Architecture](Architecture.md) quando precisar decidir o destino. Não é necessário ler todos os manuais antes de criar a primeira nota.

## Aplicar um template no Obsidian

1. Em **Settings → Core plugins**, habilite **Templates**, se necessário.
2. Em **Settings → Core plugins → Templates → Template folder location**, selecione a pasta `Templates` deste módulo. Em um vault próprio, use `Templates`; em um vault maior, use `<caminho do módulo>/Templates`, relativo à raiz do vault.
3. Crie uma nota nova vazia no destino correto e dê a ela o nome definitivo. Para ideia, post e biblioteca, crie primeiro o pacote homônimo.
4. Com a nota ativa, use **Ctrl+P → Templates: Insert template** e escolha o modelo indicado no guia do tipo.
5. Preencha o conteúdo real e confira Properties, estados e datas conforme esse guia.

O seletor nativo usa uma pasta por vault. Trocar a preferência muda a lista oferecida e conserva os arquivos da pasta anterior. Copiar este módulo não configura automaticamente o seletor de outro vault. Aponte para `Templates/`, onde estão os arquivos inseríveis, e não para Docs ou a raiz do módulo.

`{{title}}` usa o nome da nota; `{{date:YYYY-MM-DD}}` usa o dia da inserção. Variáveis ficam entre aspas no YAML; edite os templates em modo Source. A inserção ocorre na nota ativa e não cria seus diretórios. `updated_at` não acompanha futuras edições automaticamente.

O modelo de cada tipo explica quais datas recebem o dia de criação e quais permanecem vazias. Publicação, coleta, avaliação e início da execução só são preenchidos quando conhecidos. Ao gerar por IA ou outro editor, resolva as variáveis antes de salvar.

### Trabalhar em uma nota existente

Direction e Visual Identity já vêm preparadas. Preserve suas Properties e valores conhecidos e acrescente somente as seções necessárias a partir do corpo do template. Reaplicar o arquivo completo pode duplicar seções e mesclar Properties. A inserção não prova que uma nota antiga foi criada ou revisada hoje.

## Criar o primeiro trabalho

Escolha o guia correspondente ao que quer registrar:

- Um pensamento, pergunta ou argumento, mesmo curto: [Idea](Models/Ideas/Idea.md). Crie diretamente seu pacote e uma nota homônima em Ideas.
- Uma publicação concreta: [Post](Models/Posts/Post.md). Pode começar diretamente ou usar ideias existentes.
- Uma referência que decidiu preservar na biblioteca: [Library Source](Models/Source%20Library/Library%20Source.md).
- Seu contexto profissional: [Deep Dive](Models/Deep%20Dive/Deep%20Dive.md), com experiências e evidências reais.

Preencha só o que conhece. Não crie exemplos de negócio para completar pastas. Se precisar de pesquisa, siga [Sources](Sources.md); fontes simples podem continuar como links na nota.

## Quando houver uma direção e um plano

Registre escolhas editoriais reais no único `Strategy/Direction.md`, seguindo [Direction](Models/Strategy/Direction.md). Quando quiser acompanhar ações e resultados, crie um [Plan](Models/Strategy/Plan.md). O próprio plano inclui **Como avaliar**, com medidas, fontes, janelas, critérios e limites escolhidos para aquele trabalho.

A rotina completa está em [Workflow](Workflow.md), e a relação entre direção, planos, testes e decisões em [Strategy](Strategy.md). Experimentos só são criados quando houver uma pergunta específica a testar.

## Organizar a fila

No Obsidian, confira **Settings → Core plugins → Bases**. Abra o [Publishing Control](../Publishing%20Control.md), que já contém a Base da fila. Escolha um post existente e preencha `queue_order` como **Número** em sua nota principal, começando em 1. Se o campo ainda não existir, acrescente-o em Properties; não reaplique o template inteiro.

O [modelo de Post](Models/Posts/Post.md#fila-de-publicação) explica inclusão, movimentação, saída e manutenção manual. O painel começa com os estados `draft`, `review` e `ready`; use **Filter → This view** para escolher outro recorte. Nenhum filtro renumera a fila. Em outro editor, os valores podem ser mantidos no Markdown, mas a tabela dinâmica depende de Bases no Obsidian.

## Retomar e preservar o trabalho

Abra a nota em andamento, confira seu próximo passo e siga apenas os links relevantes. Para trabalhar com IA, comece por [AGENTS](../AGENTS.md) e [AI Guide](AI%20Guide.md).

As convenções compartilhadas estão em [Common](Models/Shared/Common.md). Git pode preservar o histórico se configurado e usado com commits; o número de versão sozinho não reconstrói o conteúdo anterior. Você não precisa configurar Git para começar, mas deve saber qual histórico está efetivamente preservado.

Referências do recurso nativo: [Templates](https://obsidian.md/help/plugins/templates) e [Properties](https://obsidian.md/help/properties).
