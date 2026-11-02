---
created_at: 2026-11-02
updated_at: 2026-11-02
version: 1.1.0
---

# Atualizar sua cópia do PCM

O [PCM vanilla](https://github.com/HenriqueCotta/professional-content-marketing) distribui a estrutura e os guias. Sua cópia pode conter relatos, estratégia, posts e convenções próprias. Incorporar uma melhoria significa integrar as mudanças pertinentes, preservando esse trabalho; não exige recriar o repositório nem substituir suas pastas inteiras.

Este guia trata de atualizações do modelo. Buscar e enviar o trabalho entre seus dispositivos é outra operação, explicada em [Access and Sync](Access%20and%20Sync.md).

## Preparar uma cópia pessoal

Para começar um acervo pessoal a partir do PCM público, o caminho recomendado é usar **Use this template → Create a new repository**, escolher sua conta e a visibilidade **Private**. Se quiser trabalhar no computador, clone esse repositório pessoal e abra a pasta no Obsidian ou no editor escolhido. As melhorias futuras do modelo são incorporadas pelo procedimento abaixo; criar a cópia pelo template não bloqueia atualizações, mas não as conecta automaticamente.

Um fork de um repositório público também é público, e não é possível mudar isoladamente a visibilidade desse fork. Por isso, o fork direto do PCM público não é o caminho recomendado para guardar um acervo que você pretende manter privado. Veja [visibilidade de forks](https://docs.github.com/en/pull-requests/reference/forks#visibility-of-forks).

Clonar é criar uma cópia local de um repositório já existente. Usar HTTPS, SSH, GitHub Desktop ou outro cliente não transforma um repositório criado por template em fork nem cria um vínculo de atualização com o vanilla. Clone seu repositório pessoal para buscar e enviar o seu trabalho; incorporar mudanças do modelo é uma operação distinta. Veja [clonar um repositório](https://docs.github.com/en/repositories/creating-and-managing-repositories/cloning-a-repository).

## Identificar como sua cópia foi criada

| Tipo de cópia | O que isso muda na atualização |
| --- | --- |
| Repositório criado com **Use this template** | Possui histórico próprio. Não recebe as mudanças do modelo automaticamente nem oferece a sincronização de um fork. |
| **Fork** real do repositório | Compartilha o histórico de origem e pode buscar mudanças do upstream. A integração ainda precisa preservar as escolhas da cópia pessoal. |
| Repositório independente duplicado preservando o histórico Git do modelo | Pode integrar commits com Git por compartilhar a base, mesmo sem ser um fork no GitHub. Isso exige preparar os remotos e conferir o histórico que será copiado; não é o que **Use this template** faz. |
| Arquivos baixados ou copiados para outro repositório/vault | Incorpore as alterações dos arquivos envolvidos por comparação, respeitando a localização do módulo. |

“Ter uma cópia” não comprova que ela seja um fork. O GitHub informa o repositório de origem na página de um fork; no caso de um template, a nova cópia começa com seu próprio commit inicial. Veja [criar um repositório a partir de um template](https://docs.github.com/en/repositories/creating-and-managing-repositories/creating-a-repository-from-a-template).

Preservar uma base Git comum pode facilitar integrações para quem utiliza essas ferramentas, mas também leva o histórico anterior, incluindo arquivos já removidos. Essa alternativa não garante integração automática de personalizações e não exige converter as cópias pessoais que já existem. Veja [duplicar um repositório preservando seu histórico](https://docs.github.com/en/repositories/creating-and-managing-repositories/duplicating-a-repository). A duplicação é a preparação inicial; nas atualizações, integre as mudanças preservando seu trabalho. Espelhar periodicamente o vanilla sobre o repositório pessoal pode substituir suas referências e não é o procedimento de atualização de uma cópia preenchida.

## Incorporar uma atualização

1. **Escolha a mudança e preserve seu estado atual.** Consulte o commit ou a comparação publicada no modelo para saber o que mudou. Confira o trabalho local ainda não salvo ou não enviado; mantenha uma forma de recuperá-lo. Uma branch de atualização e commits do trabalho que deseja preservar são opções quando estiver usando Git, respeitando as autorizações da tarefa.
2. **Compare os arquivos afetados.** Guias, templates, README e AGENTS também podem ter sido personalizados. Se um arquivo permanece igual à base usada, a versão nova pode ser incorporada diretamente; se mudou dos dois lados, concilie os trechos para preservar as escolhas vigentes da pessoa. A mesma regra vale para um arquivo cujo caminho ou finalidade mudou.
3. **Integre o escopo escolhido.** Atualize conjuntamente os guias, templates e referências relacionados à mudança. Preserve os registros pessoais e as configurações locais. Uma alteração no template orienta novos registros; não manda reaplicar o template em todas as notas existentes.
4. **Confira o resultado.** Verifique os links, os destinos dos registros, as convenções pessoais e os dados que deveriam permanecer. Resolva conflitos relevantes antes de considerar a atualização concluída. Registre e envie as alterações ao repositório pessoal quando isso estiver autorizado.

Uma mudança de exemplo ou de pasta inicial no vanilla não obriga reorganizar conteúdo preenchido. Por exemplo, permitir organização livre em Deep Dive não exige apagar `Work/` ou `Personal Projects/`: essas pastas continuam válidas como escolhas pessoais.

### Quando for um fork

O GitHub oferece **Sync fork**, e Git também pode buscar mudanças do remoto `upstream`. Esses recursos integram commits; não avaliam se uma convenção pessoal continua correta ou se um registro deve ser alterado. Confira o diff e eventuais conflitos. Um conflito deve ser conciliado preservando o trabalho que você pretende manter, sem descartar os commits pessoais para forçar a sincronização. Veja [sincronizar um fork](https://docs.github.com/en/pull-requests/how-tos/work-with-forks/syncing-a-fork).

### Quando os históricos forem independentes

Use o diff da atualização como referência para aplicar os trechos pertinentes. Isso pode ser feito por uma IA com acesso e escrita, por comparação no editor ou com ferramentas de patch, entre outras possibilidades. Adicionar o modelo como remoto não cria ancestralidade compartilhada; unir os históricos inteiros não é necessário para atualizar a documentação.

Ferramentas de patch precisam verificar a base e as alterações locais. `git apply --check` verifica se um patch pode ser aplicado sem aplicá-lo. Ele não avalia o significado da atualização nem garante que personalizações sejam preservadas; a revisão do conteúdo continua necessária. Veja [git apply](https://git-scm.com/docs/git-apply).

## Pedir a atualização a uma IA

Com a IA configurada conforme [Getting Started](Getting%20Started.md#instrução-para-a-ia), um pedido possível é:

```text
Quero incorporar ao meu PCM a atualização <link do commit ou comparação> do modelo HenriqueCotta/professional-content-marketing.

Consulte o AGENTS.md e o estado atual da minha cópia. Compare os arquivos envolvidos e integre as mudanças pertinentes, preservando meus registros, minha organização e minhas personalizações. Concilie os arquivos modificados dos dois lados, em vez de substituir pastas inteiras.

Se houver uma incompatibilidade que dependa de uma escolha minha, explique esse ponto e avance nas partes independentes. Ao terminar, informe o que foi integrado, o que permaneceu pendente e se as mudanças ficaram apenas locais ou também foram enviadas ao GitHub, conforme o acesso e a autorização disponíveis.
```

O pedido é ilustrativo. O alcance continua sendo o da tarefa e das ferramentas disponíveis, conforme [AI Guide](AI%20Guide.md); consultar o modelo não concede acesso ou autorização para alterar o repositório pessoal.
