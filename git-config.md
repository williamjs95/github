// iniciar git
git init      

// configurar nome
git config --global user.name "williamjs95"

configurar email
git config --global user.email "williamj.silva@live.com"

listar metadados
git config --list

adicinar modificação ao working diretory (todos os arquivos)
git add .

comitar modificações na staged area
git commit -m "created index.html"

log de commit
git log

log de commit (resumo)
git log --oneline

mostrar as 3 últimas modificações 
git log -n 3

mostrar aquivos modificados 
git status

mostrar linhas modificadas
git diff

restaurar modificação (working directory)
git restore --index.html

restaurar modificação (staged area - volta para working diretory)
git restore --staged index.html

corrigir a descrição do último commit
git commit --amend -m "change title page index.html"

desfaz o último commit (voltar para working directory)
git reset --soft HEAD~1

gerar chave ssh
ssh-keygen

atualizar cach do git
$ git rm -r --cashed .

clonar repositório
git clone git@github.com:williamjs95/github.git

buscar atualizações do repositório
git pull git

criar nova branch
git checkout -b feat/nome-da-branch

>> PULL REQUEST

Para criar uma branch - no terminal vai digitar 
git checkout -b NOMEBRANCH (exemplo: AE-403/feat_menubar)

para adicionar as mudanças realizadas a sua branch 
git add .

para adicionar uma mensagem ao commit 
git commit -m "Mensagens do commit/" (exemplo: "AE-403/feat: mensagem do commit")

e para subir o commit 
git push origin NOMEDABRANCH (exemplo: AE-403/feat_menubar)

para o commit segue o mesmo padrão 
git commit -m "AE-403/feat: mensagem do commit vem logo em seguida iniciando com o numero do card"