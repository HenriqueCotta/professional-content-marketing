---
created_at: 2026-10-20
updated_at: 2026-10-23
---

# Professional Content Marketing

Sistema autocontido para organizar contexto profissional, estratégia, ideias, fontes, produção de conteúdo e aprendizado com os resultados. A documentação orienta pessoas e IAs durante a criação, a manutenção e a retomada do trabalho.

O caminho recomendado é orientar uma IA para executar o trabalho no PCM, com os objetivos e escolhas da pessoa. Use um repositório pessoal no GitHub como base principal ou uma pasta local como alternativa, conforme o acesso disponível. Obsidian é opcional; o uso pode ser manual, com IA ou combinado.

Você escolhe quanto delegar: pode receber uma primeira versão inteira para avaliar depois, desenvolver partes em conversa ou combinar outras formas de trabalho. O PCM não exige perguntas ou aprovação a cada etapa; veja [Participação e delegação](Docs/AI%20Guide.md#participação-e-delegação).

## Começar e retomar

Siga [Getting Started](Docs/Getting%20Started.md) para a primeira tarefa e [Access and Sync](Docs/Access%20and%20Sync.md) para disponibilizar os arquivos e manter sua cópia de trabalho. Nas instruções persistentes da sua IA, use a [instrução para a IA](Docs/Getting%20Started.md#instrução-para-a-ia): ela aponta para o PCM e orienta a consulta atualizada, o acompanhamento e a conferência do trabalho. As regras detalhadas continuam nos guias deste módulo.

Depois, faça seu pedido: desenvolver uma ideia a partir de anotações, preparar um post com referências ou avaliar um plano usando os dados disponíveis, por exemplo. São exemplos, não uma lista completa: você pode combinar operações e pedir outros trabalhos, conforme o acesso e as ferramentas da sessão, seguindo as regras dos registros.

## Princípios

- **Contexto e escolhas reais:** a pessoa define objetivos, voz, público, canais e identidade visual; cada afirmação respeita as evidências disponíveis.
- **Registros com responsabilidade clara:** cada ideia, post e material preservado tem seu pacote; dados, interpretações e decisões ficam nos registros correspondentes, ligados por referências.
- **Estrutura adaptável:** tags são opcionais e livres. Campos, seções, filtros e formas de trabalhar podem evoluir conforme a necessidade; atualize os guias e templates envolvidos quando mudar uma convenção compartilhada.
- **Uso autocontido:** mantenha juntos os guias, templates e arquivos de trabalho no repositório ou na pasta. A mesma estrutura também pode funcionar dentro de outro vault ou como vault independente.

## Encontrar a orientação certa

| Quero fazer ou entender | Referência |
| --- | --- |
| Começar com IA ou usar os arquivos diretamente | [Getting Started](Docs/Getting%20Started.md) |
| Configurar acesso e sincronizar a cópia de trabalho | [Access and Sync](Docs/Access%20and%20Sync.md) |
| Conferir a árvore, os destinos e as responsabilidades | [Architecture](Docs/Architecture.md) |
| Retomar o fluxo da ideia à avaliação | [Workflow](Docs/Workflow.md) |
| Organizar e consultar a fila de posts | [Publishing Control](Publishing%20Control.md) e [Post](Docs/Models/Posts/Post.md#fila-de-publicação) |
| Relacionar direção, planos, testes e decisões | [Strategy](Docs/Strategy.md) |
| Pesquisar, guardar e reutilizar fontes | [Sources](Docs/Sources.md) |
| Consultar campos, estados e estrutura de um registro | [Modelos](#modelos) |
| Colaborar com uma IA | [AGENTS](AGENTS.md) e [AI Guide](Docs/AI%20Guide.md) |

A fila usa `queue_order` com 1, 2, 3… nos posts e requer manutenção explícita pela pessoa ou por uma IA autorizada, conforme os critérios escolhidos. O Publishing Control oferece uma Base no Obsidian; filtros mudam a visualização, sem renumerar a fila ou atualizar suas posições automaticamente.

## Modelos

Cada guia em Docs/Models reúne finalidade, localização, Properties e estados, estrutura e controle do template associado. Os arquivos inseríveis ficam em Templates, na raiz.

- **Ideas:** [Idea](Docs/Models/Ideas/Idea.md).
- **Posts:** [Post](Docs/Models/Posts/Post.md), [Analytics Snapshot](Docs/Models/Posts/Analytics%20Snapshot.md) e [Review](Docs/Models/Posts/Review.md).
- **Strategy:** [Direction](Docs/Models/Strategy/Direction.md), [Plan](Docs/Models/Strategy/Plan.md), [Experiment](Docs/Models/Strategy/Experiment.md) e [Decision](Docs/Models/Strategy/Decision.md).
- **Source Library:** [Library Source](Docs/Models/Source%20Library/Library%20Source.md).
- **Deep Dive:** [Deep Dive](Docs/Models/Deep%20Dive/Deep%20Dive.md).
- **Visual Identity:** [Visual Identity](Docs/Models/Visual%20Identity/Visual%20Identity.md).
- **Shared:** [Common](Docs/Models/Shared/Common.md) reúne convenções gerais pequenas; [Local Source](Docs/Models/Shared/Local%20Source.md) aplica-se às notas autorais em Sources de ideias e posts.

## Portabilidade

Os links dos guias são relativos ao módulo. Os registros em Markdown podem ser usados por IAs e em outros editores; os plugins nativos Templates e Bases oferecem facilidades opcionais no Obsidian. Antes de compartilhar uma cópia usada, confira as informações pessoais e os materiais de terceiros incluídos.
