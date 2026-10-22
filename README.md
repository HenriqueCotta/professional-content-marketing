---
created_at: 2026-10-20
updated_at: 2026-10-21
---

# Professional Content Marketing

Sistema autocontido para organizar contexto profissional, estratégia, ideias, fontes, produção de conteúdo e aprendizado com os resultados. A documentação orienta pessoas e IAs durante a criação, a manutenção e a retomada do trabalho.

## Princípios

- **Contexto e escolhas reais:** a pessoa define objetivos, voz, público, canais e identidade visual; cada afirmação respeita as evidências disponíveis.
- **Registros com responsabilidade clara:** cada ideia, post e material preservado tem seu pacote; dados, interpretações e decisões ficam nos registros correspondentes, ligados por referências.
- **Estrutura adaptável:** tags são opcionais e livres. Campos, seções, filtros e formas de trabalhar podem evoluir conforme a necessidade; atualize os guias e templates envolvidos quando mudar uma convenção compartilhada.
- **Uso autocontido:** esta pasta pode funcionar dentro de outro vault ou como vault independente. Mantenha juntos os guias, templates e arquivos de trabalho.

## Encontrar a orientação certa

| Quero fazer ou entender | Referência |
| --- | --- |
| Configurar o uso e aplicar templates no Obsidian | [Getting Started](Docs/Getting%20Started.md) |
| Conferir a árvore, os destinos e as responsabilidades | [Architecture](Docs/Architecture.md) |
| Retomar o fluxo da ideia à avaliação | [Workflow](Docs/Workflow.md) |
| Organizar e consultar a fila de posts | [Publishing Control](Publishing%20Control.md) e [Post](Docs/Models/Posts/Post.md#fila-de-publicação) |
| Relacionar direção, planos, testes e decisões | [Strategy](Docs/Strategy.md) |
| Pesquisar, guardar e reutilizar fontes | [Sources](Docs/Sources.md) |
| Consultar campos, estados e estrutura de um registro | [Modelos](#modelos) |
| Colaborar com uma IA | [AGENTS](AGENTS.md) e [AI Guide](Docs/AI%20Guide.md) |

O Publishing Control apresenta a fila em uma Base. A ordem manual usa `queue_order` com 1, 2, 3…; a pessoa escolhe os filtros e colunas conforme o plano. Alterar um filtro muda a visualização, preservando as posições registradas nos posts.

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

Os links dos guias são relativos ao módulo. Os registros em Markdown podem ser usados em outros editores; Templates e Bases são recursos nativos do Obsidian. Git e uma IA são opcionais. Antes de compartilhar uma cópia usada, confira as informações pessoais e os materiais de terceiros incluídos.
