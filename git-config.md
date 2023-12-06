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
git pull

criar nova branch
git checkout -b feat/nome-da-branch



>>>>>>>>>>> PULL REQUEST

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




>>>>>>>>>> COMMIT SEMANTICO

feat- Commits do tipo feat indicam que seu trecho de código está incluindo um novo recurso (se relaciona com o MINOR do versionamento semântico).

fix - Commits do tipo fix indicam que seu trecho de código commitado está solucionando um problema (bug fix), (se relaciona com o PATCH do versionamento semântico).

docs - Commits do tipo docs indicam que houveram mudanças na documentação, como por exemplo no Readme do seu repositório. (Não inclui alterações em código).

test - Commits do tipo test são utilizados quando são realizadas alterações em testes, seja criando, alterando ou excluindo testes unitários. (Não inclui alterações em código)

build - Commits do tipo build são utilizados quando são realizadas modificações em arquivos de build e dependências.

perf - Commits do tipo perf servem para identificar quaisquer alterações de código que estejam relacionadas a performance.

style - Commits do tipo style indicam que houveram alterações referentes a formatações de código, semicolons, trailing spaces, lint... (Não inclui alterações em código).

refactor - Commits do tipo refactor referem-se a mudanças devido a refatorações que não alterem sua funcionalidade, como por exemplo, uma alteração no formato como é processada determinada parte da tela, mas que manteve a mesma funcionalidade, ou melhorias de performance devido a um code review.

chore - Commits do tipo chore indicam atualizações de tarefas de build, configurações de administrador, pacotes... como por exemplo adicionar um pacote no gitignore. (Não inclui alterações em código)

ci - Commits do tipo ci indicam mudanças relacionadas a integração contínua (continuous integration).

raw - Commits to tipo raw indicam mudanças relacionadas a arquivos de configurações, dados, features, parametros.