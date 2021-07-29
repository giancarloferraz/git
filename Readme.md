git clone Repo_URL.git - Obtem repositorio do Fork / Repositorio
git add pasta\file.ext - adiciona arquivo ao commit
git add . - Adicona todos ao commit
git rm pasta/file.txt - remove do commit
git commit -m "Comentário" - comentario deve ser o numero e descrição do ticket
git pull - obtem commits da origin/branch (Remoto)
git push - envia commits para origin/branch (Remoto)
git pull/push remoto branch (origin/upstream) - Atualiza o local com a remote/branch (upstream)
git push origin nome_branch - envia branch para remoto
git push --set-upstream origin nome_branch - envia branch para remoto (esse funciona melhor, só precisa de um passo)
git branch -d nome_branch - remove branch local
git push origin --delete nome_branch
git stash - coloca alterações não comitadas no limbo
git stash apply - volta alterações do limbo
git fetch -p - atualiza lista de branchs
git remote - lista repositorios remotos
git remote add nome URL_Repo - adiciona repositorio remoto (upstream)
git remote rm nome - remove o repositorio remoto
git checkout nome_branch - muda de branch (master é uma branch)
git checkout -f - reseta o working tree
git checkout -b nome_branch - cria uma branch e muda para ela (feature_1234_descricao_task / bug_4321_descricao_bug)
git checkout -m nome_branch - faz merge das alterações na troca
git remote update - atualiza os remotes
git remote update --prune - atualiza os remotes removendo branchs deletadas
git merge para_branch - merge branch para na atual
git mergetool - abre ferramenta de merge.
git log - mostra commits
git reset --hard sha1 - hash do commit que vai ser mantido
git push -f -força o push zerando os commits da remote

---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

-- sequencia para iniciar desenvolvimento
1 - Atualizar local com upstream (na master) - git pull upstream master
2 - Atualizar origin com local (na master) - git push origin master
3 - criar branch (git checkout -b nome_branch)
4 - enviar branch para o remoto (git push --set-upstream origin nome_branch)
-- sequencia para finalizar brach para request merge
1 - Adicionar arquivos (git add pasta\file.ext)
2 - Aplicar commit (git commit -m "Comentário" - comentario deve ser o numero e descrição do ticket)
3 - Atualizar local com upstream (git pull upstream master)
4 - Atualizar remoto com local (git push origin nome_branch)
git reset --hard
TROCAR BRANCH PARA PUBLICACAO HMLG
git.exe checkout -f -B feature_15253_template_boletos_16590_16591_16592_16593 remotes/edemilson/feature_15253_template_boletos_16590_16591_16592_16593 --