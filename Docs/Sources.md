---
created_at: 2026-10-20
updated_at: 2026-10-22
version: 1.0.0
---

# Fontes e biblioteca

Este guia orienta a pesquisa, a localização e a reutilização de materiais. Os modelos de registro ficam em [Shared/Local Source](Models/Shared/Local%20Source.md) e [Library Source](Models/Source%20Library/Library%20Source.md). O fluxo de produção está em [Workflow](Workflow.md).

## Fonte e evidência

Fonte é o material usado para investigar, contextualizar ou sustentar uma afirmação: artigo, documento, conversa, dados, captura, código ou registro de uma experiência. Pode ser interna ou externa; essa origem não decide sua pasta.

Evidência é o papel do material ao sustentar uma afirmação. Uma captura pode comprovar uma observação sem demonstrar sua causa. Comparações e relatórios explicam essa relação quando necessários, com nomes descritivos. Não há um arquivo Evidence nem um dossiê obrigatório.

## Decidir onde guardar

| Situação | Destino |
| --- | --- |
| Um link simples atende à referência | A própria nota da ideia ou post. |
| Captura, análise ou material produzido para uma ideia | Sources dentro do pacote da ideia. |
| Material obtido durante uma publicação concreta | Sources dentro do pacote do post. |
| A pessoa decidiu preservar um material na biblioteca | Pacote próprio em Source Library. |
| O mesmo material e versão já existem em outro pacote | Link para o caminho existente. |

Sources local comporta arquivos diretos e subpastas úteis à tarefa. Não exige cadastro de cada anexo nem subpastas fixas para logs, capturas ou análises. A nota principal explica o papel dos materiais no raciocínio. Uma nota ou relatório autoral local segue [Shared/Local Source](Models/Shared/Local%20Source.md), cuja aplicação cruza Ideas e Posts.

Source Library recebe materiais por intenção explícita de preservação, mesmo no primeiro contato. Um pacote representa um objeto identificável, com origem e escopo; um tema amplo não basta. Pode conter só sua nota com link para o original. Campos, estados e estrutura ficam em [Library Source](Models/Source%20Library/Library%20Source.md).

## Reutilizar e preservar a origem

Antes de capturar novamente, procure na biblioteca e nos pacotes relacionados. A mesma versão pode ser referenciada por várias ideias e posts, inclusive a partir do Sources de outro pacote. Outro uso não obriga mover, promover ou duplicar o arquivo.

Materiais semelhantes podem corresponder a versões, períodos, amostras ou transformações diferentes. Identifique o que muda e qual original foi utilizado. Ao reorganizar, conserve a rastreabilidade e os vínculos de quem usou a versão anterior. Não elimine material citado ou publicado para resolver uma aparente duplicação.

Links a partir de quem utiliza o material oferecem contexto, sem exigir listas manuais de todos os consumidores na fonte. Uma fonte nova de um post pertence àquele trabalho; não sincronize suas descobertas automaticamente com as ideias de origem.

O arquivamento da nota de biblioteca segue seu guia. Material antigo pode continuar válido como evidência histórica; seu uso por outro trabalho não determina alteração automática de estado.

## Guardar a fonte ou explicar o que ela mostrou

Quem lê uma afirmação precisa entender de onde ela veio e conseguir conferir, ao menos em parte. Algumas situações dificultam isso e muitas vezes aparecem juntas. As soluções citadas abaixo são apenas exemplos: outras são igualmente válidas, cada caso pode pedir uma diferente, e nem todas precisam aparecer.

**Fonte grande.** Quando a fonte é muito extensa, como um livro, um site inteiro ou os dados brutos de um teste longo, guardá-la inteira no vault costuma não valer a pena: pesa e não ajuda quem lê. A afirmação, porém, continua precisando de sustentação. Mesmo sem a fonte completa, quem lê precisa entender o que ela mostrou e como se chegou a isso, e ter algum caminho para chegar à fonte ou conferir parte dela. Por exemplo, uma explicação curta do resultado e do método pode atender à primeira necessidade; um trecho representativo guardado no vault, um link para o material ou a descrição de como repetir um teste podem atender à segunda. Outras formas que atendam a essas necessidades valem tanto quanto essas. Se a fonte for guardada inteira, a explicação continua útil, para que ninguém precise percorrê-la toda.

**Fonte que pode mudar.** Uma página ou um documento atualizado pode não mostrar amanhã o que mostrou hoje. Quem lê precisa saber qual versão sustentou a afirmação. Muitas vezes basta o dia em que a fonte foi vista; às vezes a própria fonte informa uma edição; às vezes vale guardar um trecho daquele momento. São só exemplos; outras formas também servem. Uma fonte que não muda, como um livro, dispensa essa preocupação.

**Fonte que só você consegue abrir.** Um arquivo no seu computador não pode ser aberto por outra pessoa nem pela IA em outro aparelho. Quem lê precisa de algo que consiga alcançar. Pode ser, por exemplo, o essencial levado para a nota, a indicação de onde a mesma fonte pode ser encontrada ou a explicação de como obtê-la de novo, entre outras possibilidades. Se não houver como, isso deve ficar dito.

Quando as situações se somam, as necessidades também se somam. Por exemplo, um manual extenso publicado num site é grande e pode mudar: quem lê precisa entender o que importa, chegar ao material e saber qual versão foi consultada. Um livro guardado só no seu computador é grande e só você abre: quem lê precisa entender o que importa e saber onde encontrá-lo.

As datas da nota (`created_at` e `updated_at`) contam quando ela foi escrita e alterada, não quando a fonte foi vista.

O contexto fica no registro responsável, sem repetição integral em cada uso. Uma conversa ou relatório de IA registra o que foi dito naquele contexto; afirmações sobre o mundo continuam exigindo prova ou indicação de verificação pendente.

## Fontes, produção visual e desempenho

| Área | Responsabilidade |
| --- | --- |
| Sources local ou Source Library | Consulta, investigação e sustentação das afirmações. |
| Assets | Material visual editorial da publicação. |
| Assets/Source | Origem editável da peça visual. |
| Analytics/Raw | Arquivos brutos de desempenho. |
| Reviews | Interpretação individual do desempenho. |

Uma captura consultada para entender um problema fica em Sources. Uma peça visual derivada dela fica em Assets e pode apontar para a referência. Um export de desempenho fica em Analytics/Raw; sua documentação e interpretação seguem os guias de [Analytics Snapshot](Models/Posts/Analytics%20Snapshot.md) e [Review](Models/Posts/Review.md).

Nomes de originais e convenções gerais estão em [Common](Models/Shared/Common.md). Frontmatter pertence às notas autorais que o respectivo modelo prevê; não o aplique automaticamente a PNG, PDF, XLSX ou outros anexos.
