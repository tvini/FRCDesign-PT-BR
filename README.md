# Métodos de Contribuição

## Contribuição Pública
Qualquer pessoa pode criar conteúdo para o site sem precisar ter conhecimento de Markdown ou GitHub, embora seja preferível que você aprenda a usar ambos para reduzir a carga de trabalho dos outros colaboradores.

No [servidor do Discord](https://discord.gg/qdx7pdZKx4), vá para o [canal "website-feedback"](https://discord.com/channels/1120162219502608426/1233961750639018104) e pergunte se você pode contribuir com o que deseja, preenchendo este modelo:

    Problema/conteúdo:
    Solução ou observações sobre a execução do conteúdo:
    Quando você planeja terminar?:
    Vai usar uma plataforma alternativa ou criar um fork no Github?:

Isso é para garantir que você não perca seu tempo caso seja algo que não será colocado no site ou que alguém já tenha começado a trabalhar.

Se você receber aprovação para começar a trabalhar nisso, um colaborador interno fará uma nova postagem no [canal do fórum "public-website-contribution"](https://discord.com/channels/1120162219502608426/1233993910817259663) ou irá te direcionar para uma postagem já existente para que você possa colaborar e complementar o trabalho de outro colaborador, caso o conteúdo ou problema já tenha começado a ser tratado.

Quando você começar seu trabalho, pode escolher entre:

1. Fazer um fork do repositório no Github e enviar pull requests para que seu trabalho seja aceito (se você tiver mais conhecimento em programação)
2. Trabalhar em uma plataforma alternativa, como Google Docs ou Notion, e deixar que um colaborador interno faça a transferência para o site quando você terminar

## Configurando o Github e o VS Code para Contribuir
### Pré-requisitos de instalação
Certifique-se de baixar as versões corretas para o sistema operacional que você possui (Windows, Mac ou Linux).

Os instaladores para Windows quase sempre precisarão ser a versão 64 bits, caso haja essa distinção.

- A versão mais recente do [Git Bash](https://git-scm.com/downloads)
    - Siga as instruções para o seu sistema operacional
    - Use todas as opções padrão para a instalação
- [Python 3.10.6](https://www.python.org/downloads/release/python-3106/) 
    - Quando o instalador abrir, certifique-se de selecionar "Add Python 3.10 to PATH" na parte inferior e clique em "Install Now"
    - Para usuários do Windows, você tem a opção de desabilitar o limite de comprimento do PATH no final; isso pode ser útil para outros projetos, mas não é obrigatório para contribuir com o site
- [VSCode](https://code.visualstudio.com/)
    - Baixe a versão estável para o seu sistema operacional
    - Use todas as opções padrão para a instalação, exceto a criação de um ícone na área de trabalho, caso deseje
- [GitHub Desktop](https://desktop.github.com/)
    - Após a instalação, selecione "Sign in to GitHub.com"
    - Faça login ou crie uma nova conta no GitHub, depois clique em "Authorize Desktop"
        - Se você optar por se cadastrar, será necessário verificar sua conta com um captcha no final do registro e um código enviado por e-mail
        - Se o captcha falhar, tente desativar alguma extensão de privacidade que possa estar interferindo
        - Configure o restante da sua conta (você pode optar por se inscrever no GitHub Education, mas isso não é obrigatório; a versão gratuita é suficiente)
        - Se não for direcionado para a página de autorização após se cadastrar, volte para o aplicativo GitHub Desktop, pressione "Cancel" e selecione "Sign in to GitHub.com" novamente
    - Permita que seu navegador abra o GitHub Desktop
    - Clique em "Finish"
    

### Passos para Começar a Escrever Contribuições

**Para Colaboradores Públicos:**

1. Vá para o [repositório do site](https://github.com/davidsdesignserver/dds-manual)
2. Clique em "Fork" próximo ao canto superior direito, depois clique em "Create Fork" na próxima tela
3. Abra o GitHub Desktop e selecione "Clone a repository from the Internet..." ou vá em ```file -> Clone repository...``` no canto superior esquerdo.
4. Em "GitHub.com", selecione seu repositório forkado ```[username]/dds-manual``` e clique em "Clone".
5. Após clonar o repositório (baixar uma cópia dele para seu computador), será perguntado como você planeja usar o fork. Selecione "To contribute to the parent project" e clique em "Continue"

**Para Colaboradores Internos (adicionados ao repositório principal):**

1. Abra o GitHub Desktop e selecione "Clone a repository from the Internet..." ou vá em ```file -> Clone repository...``` no canto superior esquerdo
2. Em "GitHub.com", selecione o repositório ```davidsdesignserver/dds-manual``` e clique em "Clone"
3. Após clonar o repositório (baixar uma cópia dele para seu computador), será perguntado como você planeja usar o fork. Selecione "To contribute to the parent project" e clique em "Continue".

**Como Escrever e Enviar Pull Requests de Contribuições**

1. Crie uma nova branch indo ao menu suspenso "Current branch" no topo do GitHub Desktop, clicando em "New branch", dando um nome e clicando em "Create branch".
    - Normalmente, você deve fazer alterações em branches (não na main), e depois criar o que é chamado de "pull request" para que essas mudanças sejam "puxadas" e mescladas na branch principal original
    - Nomeie a branch com algo relacionado às mudanças que você está fazendo, por exemplo, "contributors-guide" ou "3A-cleanup". Espere deletar a branch após o pull request, então mantenha o nome específico para suas alterações
    - Certifique-se de publicar a branch clicando no botão que aparece logo após criar uma nova branch
2. Clique em "Open in Visual Studio Code" para abrir o VS Code.
3. Se aparecer um pop-up dizendo "Do you trust the authors of the files in this folder?", marque a caixa ao lado de "Trust the authors of all files in the parent folder 'GitHub'" (para não receber mais esse aviso ao clonar repositórios no futuro) e clique em "Yes, I trust the authors".
4. Configure o VS Code do jeito que preferir se esta for a sua primeira vez usando-o (temas, extensões).
    - A extensão "Code Spell Checker" é recomendada.
    - Ative o salvamento automático no menu ```file``` ativando a opção
5. Faça um conjunto de alterações.
    - Todos os arquivos e pastas do site estão contidos na pasta ```docs```, exceto o arquivo ```mkdocs.yml```, que contém o diretório para a barra lateral do site

6. Sempre que você alcançar um bom ponto para parar e quiser salvar suas mudanças na nuvem, você deve fazer o que chamamos de "commit", que é quando as alterações são salvas na branch. Depois, é necessário "push" (enviar) os commits para que sejam carregados na nuvem; caso contrário, eles permanecerão apenas localmente. Você pode fazer isso pelo VS Code ou pelo GitHub Desktop, mas vamos usar o GitHub Desktop para centralizar todas as ações de controle de versão lá.
7. Abra o GitHub Desktop e certifique-se de que a aba "Changes" na barra lateral esteja selecionada. Todas as alterações selecionadas na barra lateral serão adicionadas ao commit (as mudanças estarão "preparadas" para o commit). Digite um resumo do commit (descrição opcional) e clique em "Commit to [branch]".
8. Clique no botão para enviar (push) o(s) commit(s) que você fez para a nuvem (pode estar no topo ou no meio da tela).
    - Clicar no botão "Fetch origin" irá buscar quaisquer commits na branch atual que outras pessoas tenham feito e enviado para a nuvem

9. Para manter seu código atualizado com a branch principal do repositório original, abra o menu "branch" no topo da tela e clique em "Update from main". Se alguns commits forem puxados para sua branch a partir da main, você pode fazer push para atualizar sua branch na nuvem novamente.
    - Certifique-se de atualizar sua branch a partir da main com frequência! Se não fizer isso, pode ter que resolver grandes conflitos entre suas alterações e as mudanças que outra pessoa fez na main. Se encontrar conflitos, siga as instruções no GitHub Desktop para abrir os conflitos no VS Code e resolvê-los lá. Depois que todos os conflitos forem resolvidos, volte para o GitHub Desktop para concluir a mesclagem.

10. Quando estiver satisfeito com seu conjunto de alterações para solicitar que sejam adicionadas ao site principal, e tiver feito o commit de todas as mudanças, verificado atualizações e enviado (push) todos os commits, crie um pull request pelo menu no meio do GitHub Desktop. Isso vai te levar ao site, onde você poderá descrever as alterações feitas e que deseja incorporar ao site, além de associar a uma issue que será corrigida. Um dos colaboradores internos irá revisar seu pull request após o envio e poderá aprová-lo e mesclá-lo à branch principal ou fazer comentários sobre ajustes necessários antes da mesclagem.

Para recapitular os passos de contribuição, faça a combinação de criar e publicar uma branch, fazer alterações e commits, atualizar a partir da main, enviar (push) os commits e criar um pull request.


### Como Executar a Pré-visualização Local do Site
Você pode obter uma versão hospedada localmente do site para ter uma pré-visualização ao vivo enquanto edita.

1. Abra o repositório no VS Code (não importa em qual branch)
2. Ative o painel inferior, caso não esteja aberto, usando o atalho ```Ctrl + J```
3. Clique no menu suspenso ao lado do + no canto superior direito do painel inferior e selecione "Git Bash"
4. Execute o comando ```py -m venv venv``` para criar um ambiente virtual (PRIMEIRA VEZ)
5. Execute o comando ```./installdependencies.sh``` para instalar todos os pacotes Python necessários (PRIMEIRA VEZ)
6. Execute o comando ```./runlocal.sh``` para iniciar o servidor.
7. Se tudo ocorreu bem, deve aparecer a mensagem "Serving on" seguida de algo como ```http://127.0.0.1:8000```.

Certifique-se de executar ```./runlocal.sh``` no Git Bash toda vez que abrir o VS Code para editar.

Dica: Depois de clicar no terminal no painel inferior, você pode usar Ctrl + C para encerrar o servidor local do site.

Nota: Quando você trocar de branch usando o GitHub Desktop, a pré-visualização local seguirá normalmente, sem problemas.
