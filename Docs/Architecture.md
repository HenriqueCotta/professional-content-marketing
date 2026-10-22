---
created_at: 2026-10-20
updated_at: 2026-10-21
version: 1.0.0
---

# Arquitetura do modelo

Este guia define áreas, destinos e responsabilidades. [Workflow](Workflow.md) explica a rotina; [Sources](Sources.md), a pesquisa e reutilização; [Strategy](Strategy.md), a relação entre direção, planos, experimentos e decisões. Cada guia em Models reúne o contrato do respectivo registro.

## Estrutura do módulo

```text
Professional Content Marketing/
├── README.md                       # entrada e índice de guias
├── AGENTS.md                       # roteamento para IA
├── Docs/
│   ├── Getting Started.md          # primeiro uso e aplicação nativa
│   ├── Architecture.md            # áreas e destinos
│   ├── Workflow.md                # rotina
│   ├── Sources.md                 # pesquisa e reutilização
│   ├── Strategy.md                # processo estratégico
│   ├── AI Guide.md                # colaboração com IA
│   └── Models/
│       ├── Shared/
│       │   ├── Common.md
│       │   └── Local Source.md
│       ├── Ideas/
│       │   └── Idea.md
│       ├── Posts/
│       │   ├── Post.md
│       │   ├── Analytics Snapshot.md
│       │   └── Review.md
│       ├── Strategy/
│       │   ├── Direction.md
│       │   ├── Plan.md
│       │   ├── Experiment.md
│       │   └── Decision.md
│       ├── Source Library/
│       │   └── Library Source.md
│       ├── Deep Dive/
│       │   └── Deep Dive.md
│       └── Visual Identity/
│           └── Visual Identity.md
├── Templates/                     # doze arquivos inseríveis
├── Deep Dive/
│   ├── Work/
│   └── Personal Projects/
├── Strategy/
│   ├── Direction.md
│   ├── Plans/
│   ├── Experiments/
│   └── Decisions/
├── Ideas/                         # um pacote por ideia
├── Source Library/                # um pacote por material
├── Posts/                         # um pacote por publicação
├── Visual Identity/
│   └── Visual Identity.md
└── Publishing Control.md          # Base embutida da fila de posts
```

Pastas vazias podem conter `.gitkeep` para existir no Git. Direction e Visual Identity vêm com campos preparados e vazios, sem conteúdo de negócio. A árvore descreve o esquema; uma cópia de trabalho pode já conter registros.

## Responsabilidades

| Área | Responsabilidade |
| --- | --- |
| Deep Dive | Contexto, experiências, contribuições, evidências e limites das afirmações. |
| Strategy | Direção vigente, planos com sua própria avaliação, testes e decisões relevantes. |
| Ideas | Argumentos e pensamentos em seus próprios pacotes, mesmo quando curtos. |
| Source Library | Materiais que a pessoa decidiu preservar como referências identificáveis. |
| Posts | Produção e histórico de cada publicação, dados e avaliações individuais. |
| Publishing Control | Visão configurável da fila, lendo a ordem nas próprias notas dos posts. |
| Visual Identity | Escolhas visuais vigentes, definidas pela pessoa, numa nota atualizada no lugar. |
| Templates | Conteúdo inserível; não contém os guias de documentação. |
| Docs/Models | Campos, estados, estrutura e controle do template de cada tipo. |

Shared agrupa documentação que cruza domínios, com aplicação explícita no guia. [Shared/Local Source](Models/Shared/Local%20Source.md) serve às notas autorais em Sources de ideias e posts. [Common](Models/Shared/Common.md) reúne orientações gerais pequenas, aplicadas conforme o contexto. Shared é uma área documental, não uma biblioteca de materiais do usuário.

Os relatos de experiências ficam em Work e Personal Projects. O [Publishing Control](../Publishing%20Control.md) contém uma Base embutida: os critérios de seleção pertencem ao plano; a ordem operacional é registrada em `queue_order` nas notas dos posts, conforme o [modelo de Post](Models/Posts/Post.md#fila-de-publicação). Filtros e colunas são adaptáveis. A Base lê os registros, sem criar outra lista manual ou guardar cópias de estados e métricas.

## Pacotes e áreas auxiliares

Ideia, post e biblioteca usam pasta e nota principal homônimas diretamente em sua área. Não agrupe pacotes de ideias em pastas temáticas; links e tags podem relacioná-los. A organização interna dos materiais segue sua necessidade, com arquivos e subpastas livres.

```text
Ideas/<Nome da ideia>/
├── <Nome da ideia>.md
├── Sources/                       # quando houver material local
└── Assets/                        # quando houver exploração visual

Source Library/<Nome do material>/
├── <Nome do material>.md
└── <arquivos e pastas pertinentes>

Posts/<Nome do post>/
├── <Nome do post>.md
├── Sources/                       # apoio factual
├── Assets/                        # material visual
│   ├── Source/                    # origem editável da peça
│   ├── Explorations/
│   └── Final/
├── Analytics/
│   └── Raw/                       # originais de desempenho
└── Reviews/                       # interpretação individual
```

Crie áreas auxiliares somente quando houver material. Sources, Assets/Source, Analytics/Raw e Reviews têm finalidades distintas, explicadas em [Sources](Sources.md). O tamanho de uma ideia não determina sua passagem para Posts; a intenção de produzir uma publicação concreta determina.

## Portabilidade e personalização

As regras permanecem dentro deste módulo. Use caminhos relativos explícitos nos links, seguindo [Common](Models/Shared/Common.md). Autocontenção não exige copiar a internet: materiais externos podem continuar externos, com origem e recorte compreensíveis.

O guia do tipo é a referência para seus campos e estados; a página também controla a versão do template associado. Os metadados do próprio guia ficam no seu frontmatter. A navegação completa está no [README](../README.md#modelos), sem catálogo paralelo de versões.

Voz, tags temáticas, canais, identidade visual e metas pertencem à pessoa. Campos preparados e exemplos não autorizam preencher lacunas por suposição. Antes de distribuir uma cópia usada, confira seu conteúdo.
