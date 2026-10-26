---
created_at: 2026-10-22
updated_at: 2026-10-26
version: 1.0.1
---

# Acesso e sincronização

O caminho principal é conversar com uma IA que consiga ler e alterar sua cópia do PCM. O acesso recomendado é ao seu repositório no GitHub, a referência compartilhada entre a IA e seus dispositivos. Uma pasta local também funciona, conforme o acesso disponível. O Obsidian é opcional.

## Preparar sua cópia e o acesso da IA

Use sua cópia de trabalho existente. Se estiver começando pelo GitHub, crie um repositório seu a partir do modelo público; se escolher o caminho local, use a pasta do PCM no dispositivo. O modelo distribui a estrutura e os guias; seu acervo profissional fica na sua cópia, com a privacidade que você escolher. Para material pessoal no GitHub, um repositório privado permite controlar quem acessa.

Informe à IA a localização escolhida e peça que comece pelo [AGENTS](../AGENTS.md). Se o PCM estiver dentro de um repositório ou vault maior, informe também o caminho da pasta que contém esse arquivo. Essa localização orienta a consulta; confira se a sessão realmente acessou a cópia de trabalho pretendida.

O acesso precisa funcionar na ferramenta usada pela IA. Com leitura, ela pode consultar e sugerir; com escrita, pode criar e atualizar os arquivos. Um link ou uma conta conectada, por si só, não garante essas duas permissões.

Configure o acesso e combine o escopo no início. O ambiente pode já ter permissão para manter arquivos e sincronizar as alterações com seu repositório. Quando isso estiver autorizado para a rotina, a IA pode concluir esse trabalho sem pedir aprovação arquivo por arquivo. Publicar conteúdo em uma rede social é outra ação, conforme a autorização da tarefa e o [AI Guide](AI%20Guide.md).

## Trabalhar só com IA e GitHub

Se a ferramenta consegue ler os arquivos atuais e salvar alterações no seu repositório, você pode usar o PCM assim, sem instalar o Obsidian. Diga o resultado desejado e deixe a IA consultar os guias pertinentes. Ao terminar, ela deve informar o que foi alterado e onde ficou salvo.

Um texto colado na conversa, um ZIP ou uma exportação são cópias daquele momento. Mudanças posteriores no repositório precisam ser trazidas para a ferramenta. O NotebookLM pode usar essas fontes para explicar o sistema e gerar materiais; isso não lhe dá acesso para editar o repositório. A edição depende de uma ferramenta que realmente permita escrever nele.

## Quando houver uma pasta local

A IA também pode trabalhar diretamente em uma pasta à qual tenha acesso. Se você usar o GitHub junto, buscar as alterações de lá atualiza a cópia local; enviar as alterações locais atualiza o repositório. Salvar um arquivo no computador não faz essa troca por si só.

Antes de continuar em outro dispositivo, traga as mudanças disponíveis. Ao terminar, envie o que alterou. Se duas cópias mudarem o mesmo conteúdo, será preciso conferir e conciliar as diferenças. Os automatismos podem cuidar dessas trocas quando estiverem configurados; acompanhe se a sincronização terminou.

### Computador com Obsidian, se quiser

Clone seu repositório, criando uma cópia local ligada ao GitHub, e abra essa pasta como vault no Obsidian. Se o PCM for parte de um vault maior, mantenha sua localização dentro dele. O Obsidian e a IA local precisam trabalhar sobre os mesmos arquivos.

Para sincronizar pelo próprio Obsidian no computador, são necessários Git instalado, o plugin comunitário Git instalado e habilitado e a autenticação no repositório. Se quiser trocas automáticas, configure também os intervalos ou eventos oferecidos pelo plugin. Veja [Getting Started do plugin](https://publish.obsidian.md/git-doc/Getting%20Started) e [Start here](https://publish.obsidian.md/git-doc/Start%20here).

O [GitKraken Desktop](https://help.gitkraken.com/gitkraken-desktop/how-to-install/) é uma opção de cliente Git para Windows, macOS e Linux. Seu uso é opcional.

Vídeo de configuração no computador: pendente.

### Celular com Obsidian, se quiser

Use uma ferramenta compatível com seu aparelho para manter uma cópia do repositório em uma pasta acessível ao Obsidian. Abra essa mesma pasta como vault, ou o vault que contém o PCM. A ferramenta precisa conseguir buscar e enviar as alterações com sua conta.

O [GitSync](https://gitsync.viscouspotenti.al/wiki/sync-options/background/app-based) é um exemplo, não uma exigência. Sua documentação descreve sincronização ao abrir ou fechar aplicativos, conforme o sistema, a configuração e as permissões. Isso não garante atualização contínua em segundo plano; confira o término da troca antes de mudar de dispositivo. As opções gerais estão no guia de [sincronização entre dispositivos do Obsidian](https://obsidian.md/help/sync-notes).

Vídeo de configuração no celular: pendente.

Para usar os arquivos no Obsidian depois de configurar o acesso, siga [Getting Started](Getting%20Started.md).
