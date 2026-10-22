---
created_at: 2026-10-20
updated_at: 2026-10-21
---

# Instruções para a IA

Esta pasta é a raiz de um sistema autocontido de conteúdo profissional, dentro de outro vault ou como vault independente. O usuário é a autoridade para objetivos, preferências e publicações. Exemplos de documentação não são experiências, escolhas ou resultados do usuário.

## Entrada por tarefa

Leia o [README](README.md), identifique a tarefa e consulte o guia do tipo de registro na seção Modelos. Leia os registros envolvidos antes de criar ou alterar conteúdo. Não é necessário carregar todos os guias a cada tarefa.

| Tarefa | Referência |
| --- | --- |
| Começar a usar e aplicar templates | [Getting Started](Docs/Getting%20Started.md) |
| Resolver localização e responsabilidade das áreas | [Architecture](Docs/Architecture.md) |
| Capturar, desenvolver, publicar e avaliar | [Workflow](Docs/Workflow.md) |
| Criar ou alterar campos, estados e seções de um registro | Guia do tipo em Models, indicado no [README](README.md#modelos) |
| Consultar convenções gerais de tags, datas, links e versões | [Shared/Common](Docs/Models/Shared/Common.md) |
| Investigar, guardar ou reutilizar fontes | [Sources](Docs/Sources.md) e, para notas locais autorais, [Shared/Local Source](Docs/Models/Shared/Local%20Source.md) |
| Selecionar ou reorganizar a fila de posts | [Publishing Control](Publishing%20Control.md) e [Post](Docs/Models/Posts/Post.md#fila-de-publicação) |
| Definir direção, planos, testes e decisões | [Strategy](Docs/Strategy.md) e o guia do registro |
| Registrar ou consultar a identidade visual | [Visual Identity](Docs/Models/Visual%20Identity/Visual%20Identity.md) |
| Verificação, lacunas e conduta de colaboração | [AI Guide](Docs/AI%20Guide.md) |

Shared contém guias que cruzam domínios. Respeite a aplicação explícita de cada um; Common reúne orientações gerais pequenas, sem tornar todos os campos obrigatórios em todos os arquivos.

## Limites de trabalho

- Preencha somente fatos e escolhas reais. Preserve controles existentes de acesso, sensibilidade e privacidade; não copie material privado de outro contexto.
- Não acrescente Properties, estados, taxonomias ou plugins obrigatórios por iniciativa própria. Campos e seções pertencem ao guia do tipo; Templates contém somente o conteúdo inserível.
- Preserve conteúdo publicado, evidências, datas comprovadas e escolhas iniciais. Não reescreva planos ou critérios para combinarem com resultados. Antes de reorganizar, confira as referências.
- Não imponha um Evidence obrigatório, subpastas fixas de apoio ou movimentação automática de fontes quando outro trabalho as utilizar. Siga Sources.
- Publicar, enviar mensagens, criar contas, commitar e fazer push dependem da autorização da tarefa. A existência deste modelo não autoriza essas ações.

## Manutenção

As regras ficam dentro deste módulo. Mantenha cada regra no guia responsável; use resumos e links nos manuais de processo. Cada página de modelo controla a versão e as datas do template associado. Não recrie um catálogo paralelo nem insira metadados de manutenção nas notas geradas. A seção **Como avaliar** pertence a cada plano. Os critérios de seleção vêm do plano; a ordem da fila é mantida manualmente em `queue_order` dos posts. Não infira prioridades, não renumere uma visão filtrada nem acrescente tags ou datas obrigatórias para usar a fila.
