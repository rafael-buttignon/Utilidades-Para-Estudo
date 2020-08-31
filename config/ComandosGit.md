# Comandos Git - **Que mais utilizo** - [Git-Commands](https://www.notion.so/Git-e-GitHub-principais-comandos-232de171470d4f9f9e41f90f4de2153f)

## Configuração do Usuário
As configurações do GIT são armazenadas no arquivo **.gitconfig** localizado dentro do diretório do usuário do Sistema Operacional.

**Setar usuário**

`git config --global user.name "Rafael Buttignon"`

**Setar E-mail**

`git config --global user.email rafael.buttignon@example.com.br`

**Setar editor**

`git config --global core.editor "code --wait"`
[Dúvidas](https://dzone.com/articles/git-operations-with-visual-studio-part-2)

**Setar ferramenta de merge**

`git config --global merge.tool kdiff3` 
[Dúvidas](https://www.intertech.com/Blog/git-mergetool-specifying-which-merge-tool-git-should-use/)

***
## Subir arquivos para a Branch

**Caso não tenha branch, utilize esse comando para criar**

`git checkout -b "NOME DA BRANCH"`

**Verificar modificaçoes**

`git status`

**Adicionara todas alteraçoes**

`git add .`

**Adiciona uma descrição do que voce fez**

`git commit -m "ESCREVER OQ FEZ"`

**Definitivamente os arquivos esta na sua branch**

`git push origin (NOME DA BRANCH SEM O PARENTESES)`

**Caso queria ver se ocorreu tudo certo com os arquivos**

`gitk`

***

## Fazer Rebase

**Vai trazer todas as alterações da DEVELOP(Master)**

`git fetch --all`

**Vai fazer rebase com a develop**

`git rebase origin/develop`

**Vai iniciar o merge**

`git mergetool`

**Continua rebase**

`git rebase --continue`

**Abortar rebase**

`git rebase --abort`

**Remover arquivos .orig**

`git clean -f`

***

## Juntar Commits

**Juntar Commits (~2 => são os tantos de commits que você tem)**

`git rebase -i HEAD~2`
[Dúvidas](https://www.internalpointers.com/post/squash-commits-into-one-git)

**Para alterar no TFS**

`git push origin [nome da branch] -f`

***

## Remover Arquivos da Branch

**Remover arquivo de Branch**

`git reset origin/develop -- src/Exemplo/do/seu/arquivo.js` 

**Caso de erro na hora do Reset**

`git reset 'HEAD@{1}'`



















