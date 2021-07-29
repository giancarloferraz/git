
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