## Comandos do Git:

> HISTÓRICO

- ***git log*** - *Mostrar todos os commits, começando pelo mais novo*
- ***git log -p < file >*** - *Mostrar mudanças ao longo do tempo para um arquivo específico*
- ***git blame < file >*** - *Mostra quem alterou o quê e quando em < file >*

> MUDANÇAS LOCAIS

- ***git status*** - *Arquivos alterados em seu diretório de trabalho*
- ***git digg*** - *Mudanças em arquivos rastreados*
- ***git add .*** - *Adicione todas as mudanças atuais para o próximo commit*
- ***git add . -p < file >*** - *Adicione algumas mudanças em < file > para o próximo commit*
- ***git commit -a*** - *Confirmar todas as alterações locais em arquivos rastreados*
- ***git commit*** - *Confirmar alterações previamente preparadas*
- ***git commit --amend*** - *Mude o último commit*

> ATUALIZAR E PUBLICAR

- ***git remote -v*** - *Lista todos os controles remotos configurados atualmente*
- ***git remote show < remote >*** - *Mostrar informações sobre um controle remote*
- ***git remote add < shortname > < url >*** - *Adicione um novo repositório remoto, denomin+ado < remote >*
- ***git fetch < remote >*** - *Baixe todas as alterações de < remote >, mas não integre no HEAD*
- ***git pull < remote > < branch >*** - *Baixe as alterações e marque/integre diretamente no HEAD*
- ***git push < remote > < branch >*** - *Publique as alterações locais remotamente*
- ***git branch -gh < remote/branch >*** - *Exclua uma filial no controle remoto*
- ***git push --tags*** - *Publique suas tags*
- ***git push*** - *Publicar*

> DESFAZER

- ***git reset -hard HEAD*** - *Descarte todas as mudanças locais em seu diretório de trabalho*
- ***git checkout HEAD < file >*** - *Descarte as alterações locais em um arquivo específico*
- ***git revert < commit >*** - *Reverter um commit (produzindo um novo commit com mudanças contrárias)*
- ***git reset -hard < commit >*** - *Redefina o ponteiro HEAD para um commit anterior... e descarte todas as alterações desde então*
- ***git reset < commit >*** - *... e preserva todas as mudanças como mudanças não planejadas*
- ***git reset -keep < commit >*** - *... e preserva as mudanças locais não comprometidas*

> BRANCHES

- ***git branch -av*** - *Listar todos os ramos existentes*
- ***git checkout < branch >*** - *Mudar ramo HEAD*
- ***git checkout < new-branch >*** - *Crie uma nova filial com base*
- ***git checkout--track < remote branch >*** - *Crie uma nova filial com base*
- ***git branch -d < branch >*** - *Deletar uma filial local*
- ***git tag < tag-name >*** - *Marque o commit atual com uma tag*

> FUNDIR E REBASE

- ***git merge < branch >*** - *Funda < branch > em seu HEAD atual*
- ***git rebase < branch >*** - *Rebase seu HEAD atual em < branch >*
- ***git rebase --abort*** - *Abortar um rebase*
- ***git rebase --continue*** - *Continue um rebase após resolver os conflitos*
- ***git mergetool*** - *Use a ferramenta de fusã configurada do tour para resolver conflitos*
- ***git add < resolved-file > | git rm < resolved-file >*** - *Use o editor de tour para resolver conflitos manualmente e (após resolver) marcar o arquivo como resolvido*