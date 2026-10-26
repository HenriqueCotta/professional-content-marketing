---
created_at: 2026-10-21
updated_at: 2026-10-26
version: 1.0.1
---

# Idea

Esta página é o guia do tipo Idea. Seu frontmatter descreve o guia; a seção Properties descreve os registros produzidos. Os destinos abaixo seguem a [convenção de raiz do PCM](../../Architecture.md#guia-template-e-registro-de-trabalho).

## Finalidade e localização

Uma ideia preserva um argumento em desenvolvimento, suas referências e o próximo passo. Registre cada ideia diretamente em `Ideas/<Nome da ideia>/<Nome da ideia>.md`, com pasta e nota homônimas, sem prefixo de data. Uma anotação curta pode começar no próprio pacote e crescer conforme o trabalho.

Consulte as [orientações compartilhadas](../Shared/Common.md) que forem pertinentes e o [guia de fontes locais](../Shared/Local%20Source.md) quando houver notas ou relatórios autorais de apoio.

## Properties e estados

- `idea_status`: `active` ou `archived`.
- `created_at`: criação comprovada da nota, não a data da experiência ou da referência citada. Se desconhecida, deixe vazia.

`active` permite desenvolver, aprofundar e reutilizar a ideia. Ela pode gerar vários posts; o uso não a arquiva automaticamente. Use `archived` quando decidir retirá-la do trabalho corrente e registre o motivo no corpo. Preserve conteúdo e vínculos. É possível voltar a `active`, explicando a retomada.

## Como preencher

Explique o que vale dizer, para quem, qual valor o argumento oferece e quais questões ainda precisam de prova. Diferencie fatos observados, interpretações e hipóteses. Termine com uma próxima ação clara; não é necessário ter uma conclusão pronta.

Relacione os materiais que sustentam o raciocínio. Uma tabela com **Material**, **Onde encontrar** e **Uso nesta ideia** pode ajudar, mas não é obrigatória. Crie `Sources/` e `Assets/` apenas quando houver material correspondente. A estrutura da ideia não obriga uma publicação.

## Template e controle

O arquivo inserível é [Templates/Idea.md](../../../Templates/Idea.md). A tabela descreve esse arquivo, não o registro criado com ele; as Properties no topo desta página descrevem o próprio guia.

| Template | created_at | updated_at | version |
| --- | --- | --- | --- |
| [Idea](../../../Templates/Idea.md) | 2026-10-21 | 2026-10-21 | `1.0.0` |
