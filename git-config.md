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