---
created_at: 2026-11-02
updated_at: 2026-11-03
version: 1.2.0
---

# Atualizar sua cópia do PCM

O modelo oficial de origem é o [PCM vanilla](https://github.com/HenriqueCotta/professional-content-marketing). Ele distribui a estrutura e os guias; sua cópia reúne seu conteúdo e suas personalizações. Ao incorporar melhorias, o destino das alterações é a cópia pessoal identificada para a tarefa. A origem é consultada como referência.

Este guia trata da evolução do modelo. A troca do seu trabalho entre dispositivos é explicada em [Access and Sync](Access%20and%20Sync.md).

## Pedir a atualização a uma IA

Com a IA configurada conforme [Getting Started](Getting%20Started.md#instrução-para-a-ia), você pode pedir, por exemplo:

```text
Atualize meu PCM com as melhorias disponíveis no PCM vanilla, preservando meus conteúdos, minha organização e minhas personalizações.
```

Esse pedido é ilustrativo; não há uma frase obrigatória. Você pode indicar uma melhoria ou versão específica, mas não precisa fornecer comandos, códigos de commits ou uma lista de arquivos. Quando o pedido for geral, cabe à IA consultar a origem e identificar o que ainda precisa ser incorporado.

O procedimento fica neste guia, acessível pelo [AGENTS](../AGENTS.md). A instrução externa da IA continua identificando a cópia pessoal e orientando essa consulta, sem duplicar as regras de atualização. Se uma cópia antiga ainda não tiver este guia ou seu encaminhamento, informe o link do vanilla no primeiro pedido para que a IA localize a orientação e incorpore as referências pertinentes.

## Incorporar as melhorias

A pessoa pode conduzir o trabalho diretamente ou delegá-lo à IA. As orientações abaixo se aplicam conforme o escopo e as ferramentas disponíveis, sem exigir terminal ou um provedor de IA específico.

1. **Identifique a cópia de trabalho e o acesso real.** Leia seu AGENTS e considere suas orientações atuais. Confira o repositório pessoal e, quando houver, a subpasta que contém o PCM. Verifique se é possível consultar a origem, ler a cópia atual e salvar alterações nela. Use as autorizações da tarefa ou rotina, conforme [AI Guide](AI%20Guide.md); com acesso somente de leitura, prepare a proposta e explicite que não foi aplicada.
2. **Identifique a atualização.** Consulte a versão solicitada ou as novidades disponíveis na origem e fixe uma referência exata, como um commit, para a comparação. Procure no histórico pessoal o que já foi incorporado, adaptado ou deixado pendente, conforme a próxima seção. O usuário não precisa escolher essa referência técnica para fazer um pedido geral.
3. **Compare o conteúdo afetado.** Quando a base anterior for conhecida, compare o modelo anterior, o modelo atualizado e sua cópia atual. Guias, templates, README e AGENTS também podem ter sido personalizados. Concilie alterações dos dois lados e identifique quais arquivos e convenções serão afetados, incluindo relações com registros preenchidos. Se o PCM estiver dentro de outro repositório, ajuste os caminhos à localização do módulo.
4. **Prepare e integre as mudanças.** Preserve um estado recuperável do trabalho existente e distinga alterações anteriores das introduzidas pela atualização. Uma branch, ou versão de trabalho separada no próprio repositório, é uma opção para preparar a integração. Atualize juntos os guias, templates e referências relacionados. Preserve conteúdo pessoal, configurações locais e escolhas de organização; mudanças que exijam adaptar registros existentes precisam ser identificadas e tratadas no escopo autorizado. Se uma incompatibilidade depender de uma escolha da pessoa, explique esse ponto e avance nas partes independentes, sem exigir aprovação arquivo por arquivo.
5. **Confira e registre o resultado.** Revise as diferenças completas, os links e os destinos dos registros. Confira caminhos e conteúdo que deveriam permanecer, inclusive personalizações nos guias. Em um acervo preenchido, verifique se os registros antigos continuam utilizáveis com as orientações novas e se o template atende a um registro novo; a forma de conferir depende da mudança e não exige criar dados fictícios no acervo pessoal. Registre o que foi incorporado e informe onde ficou salvo, quais verificações foram possíveis e o que continua pendente.

Uma alteração no template orienta novos registros; não manda reaplicá-lo em todas as notas existentes. Por exemplo, a organização livre de Deep Dive permite manter `Work/` e `Personal Projects/` como escolhas pessoais. A retirada dessas pastas vazias do modelo inicial não exige remover ou reorganizar relatos da cópia preenchida. Este é um exemplo de compatibilidade, não uma lista das organizações permitidas.

## Identificar o que já foi incorporado

Consulte os registros de atualizações anteriores e as mudanças relevantes no histórico pessoal. Uma referência da origem pode ter sido incorporada apenas em parte: confira o escopo e as pendências antes de usá-la como base. Um pedido geral inclui avaliar essas pendências; uma mudança adiada ou dispensada por uma escolha pessoal deve ser considerada nesse contexto.

Na primeira atualização, ou quando a origem anterior não puder ser comprovada, compare os arquivos e o histórico disponíveis para reconhecer as mudanças aplicáveis. Não invente uma base nem trate toda diferença em relação ao vanilla como erro. Preserve personalizações cuja intenção não esteja clara, identifique a incerteza e integre as partes que puder conferir. Pergunte somente quando uma escolha necessária não puder ser resolvida pelo contexto e pela delegação recebida.

O número `version` de um guia descreve aquele documento; não identifica a versão de todo o PCM nem comprova que uma atualização foi integrada. Mesmo com históricos Git independentes, é possível incorporar melhorias por comparação do conteúdo. Não é necessário recriar a cópia pessoal ou convertê-la em fork.

## Registrar a atualização

No histórico da cópia pessoal, registre a origem e a referência exata consultada, as mudanças incorporadas, as adaptações e eventuais pendências ou escolhas de não incorporar uma mudança. No Git, use a mensagem do commit da atualização para reunir essas informações, preservando os registros anteriores. A pessoa não precisa manter uma lista de códigos nem preencher Properties em cada nota para esse controle.

Se a integração for parcial, registre esse alcance; não declare toda a cópia atualizada até uma referência apenas porque ela foi consultada. Se o pedido não gerar alterações, informe o que foi conferido e as pendências encontradas, sem criar um commit vazio para simular uma atualização.

A conclusão deve distinguir proposta, alteração preparada, conteúdo salvo e integração concluída na cópia principal. Se o trabalho ficar numa branch ou apenas na pasta local, deixe isso explícito. Salvar, commitar, enviar ao GitHub e integrar uma branch seguem a autorização da tarefa ou rotina. Se a ferramenta não conseguir consultar ou registrar o histórico necessário, explique a limitação e o alcance do que pôde verificar, conforme [AI Guide](AI%20Guide.md#encerrar-a-tarefa).

## Trabalhar pelo GitHub ou por uma pasta local

Com ferramentas de leitura e escrita no GitHub, a IA pode consultar o modelo, preparar e registrar mudanças no repositório pessoal diretamente, inclusive quando ele foi criado por template ou por upload de arquivos. O GitHub oferece uma [API para consultar e alterar arquivos](https://docs.github.com/en/rest/repos/contents#create-or-update-file-contents). Esse caminho não exige clone no computador da pessoa nem cadastro de um remoto local chamado `pcm`. A capacidade precisa existir na integração utilizada; informar um link não concede acesso.

Com acesso à pasta local, a IA ou a pessoa pode usar o editor e as ferramentas disponíveis para fazer a mesma comparação e integração. Preserve trabalho ainda não sincronizado e confira o resultado da troca com o GitHub conforme [Access and Sync](Access%20and%20Sync.md). Uma atualização feita na nuvem abrange o conteúdo acessível no repositório; ela não comprova que alterações locais ainda não enviadas tenham sido consideradas.

## Como a criação da cópia interfere

| Tipo de cópia | O que isso muda na atualização |
| --- | --- |
| Repositório criado com **Use this template** | Tem histórico próprio. A IA pode integrar melhorias pelos arquivos, mesmo sem a sincronização de um fork. |
| **Fork** real do repositório | Compartilha o histórico de origem e permite integrar commits do upstream, conciliando as personalizações. |
| Repositório independente que preservou o histórico Git do modelo | Também pode integrar commits por compartilhar a base; essa relação precisa ser verificada. |
| Arquivos enviados para um repositório próprio ou copiados para outro vault | A comparação considera o conteúdo e a localização do módulo, sem exigir uma relação de fork. |
| Arquivos somente locais | A atualização depende de acesso à pasta ou de disponibilizar uma cópia atual à ferramenta; uma IA na nuvem não acessa automaticamente o computador. |

“Ter uma cópia” não comprova que ela seja um fork. Um fork inclui o histórico da origem; um repositório criado por template começa com seu próprio commit inicial. Veja [criar um repositório a partir de um template](https://docs.github.com/en/repositories/creating-and-managing-repositories/creating-a-repository-from-a-template).

Para começar um acervo privado a partir do PCM público, o caminho recomendado continua sendo **Use this template → Create a new repository → Private**. Se quiser uma pasta no computador, clone seu repositório pessoal. Um fork do PCM público também será público, conforme a [visibilidade de forks](https://docs.github.com/en/pull-requests/reference/forks#visibility-of-forks). O protocolo e o cliente usados para [clonar](https://docs.github.com/en/repositories/creating-and-managing-repositories/cloning-a-repository) não criam sincronização automática com o vanilla.

## Usar ferramentas Git, quando fizer sentido

Estas são alternativas de execução conforme a cópia e o acesso disponíveis, não etapas que toda pessoa precisa realizar:

- Em um fork, **Sync fork** ou a integração de commits do remoto `upstream` podem trazer mudanças. Confira o resultado e concilie conflitos, preservando os commits pessoais. Veja [sincronizar um fork](https://docs.github.com/en/pull-requests/how-tos/work-with-forks/syncing-a-fork).
- Com históricos independentes, um diff ou patch pode ajudar a aplicar os trechos escolhidos. `git apply --check` verifica se um patch pode ser aplicado sem aplicá-lo; não avalia o significado nem a compatibilidade das personalizações. Veja [git apply](https://git-scm.com/docs/git-apply).

Adicionar o modelo como remoto não cria ancestralidade compartilhada; unir os históricos inteiros não é necessário para atualizar os arquivos. Uma [duplicação inicial preservando o histórico](https://docs.github.com/en/repositories/creating-and-managing-repositories/duplicating-a-repository) é outra forma de preparar uma cópia, mas também leva arquivos já removidos do histórico. Espelhar periodicamente o vanilla sobre o repositório pessoal pode substituir suas referências e não é o procedimento de atualização de uma cópia preenchida.
