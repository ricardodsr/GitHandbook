# Cria um novo repositório ou reinicializa um ja existente
        $ git init

# Imprime e define algumas variáveis de configuração básicas (global)
        $ git config --global user.email
        $ git config --global user.name

        $ git config --global user.email "MyEmail@Zoho.com"
        $ git config --global user.name "My Name"

# Ver rapidamente os comandos disponiveis
        $ git help

# Ver todos os comandos disponiveis
        $ git help -a

# Requerer *help* sobre um comando especifico - manual de utilizador
# git help <command_here>
        $ git help add
        $ git help commit
        $ git help init

# Apresenta o *branch*, ficheiros não monitorizados, alterações e outras difereças
        $ git status

# Para aprender mais detalhes sobre git *status*
        $ git help status

# adiciona um ficheiro no directório do projecto atual
        $ git add HelloWorld.java

# adiciona um ficheiro num sub-directório
        $ git add /path/to/file/HelloWorld.c

# permite usar expressões regulares!
        $ git add ./*.java

# listar *branches* existentes e remotos
        $ git branch -a

# criar um novo *branch*
        $ git branch myNewBranch

# apagar um *branch*
        $ git branch -d myBranch

# alterar o nome de um *branch*
# git branch -m <oldname> <newname>
        $ git branch -m myBranchName myNewBranchName

# editar a descrição de um *branch*
        $ git branch myBranchName --edit-description

# Checkout de um repositório - por predefinição para o branch master
        $ git checkout

# Checkout de um branch especifico
        $ git checkout branchName

# Cria um novo branch e faz checkout para ele.
# Equivalente a: "git branch <name>; git checkout <name>"
        $ git checkout -b newBranch

# Clona ricardodsr/Git-NOT-Github       
        $ git clone https://github.com/ricardodsr/Git-NOT-Github

# commit com uma mensagem
        $ git commit -m "Added multiplyNumbers() function to HelloWorld.c"

# Apresenta a diferença entre o directório atual e o index
        $ git diff

# Apresenta a diferença entre o index e os commits mais recentes
        $ git diff --cached

# Apresenta a diferença entre o directório atual e o commit mais recente
        $ git diff HEAD

# Define a apresentação de números de linha nos resultados do grep
        $ git config --global grep.lineNumber true

# Torna os resultados da pesquisa mais fáceis de ler, agrupando-os
        $ git config --global alias.g "grep --break --heading --line-number"

# Pesquisa por "variableName" em todos os ficheiros de java
        $ git grep 'variableName' -- '*.java'

# Pesquisa por uma linha que contém "arrayListName" e "add" ou "remove"
        $ git grep -e 'arrayListName' --and \( -e add -e remove \)

# Apresenta todos os commits
        $ git log

# Apresenta X commits
        $ git log -n 10

# Apresenta apenas commits de merge
        $ git log --merges

# Junta o branch especificado com o atual
        $ git merge branchName

# Para gerar sempre um commit ao juntar os branches
        $ git merge --no-ff branchName

# Alterar o nome de um ficheiro
        $ git mv HelloWorld.c HelloNewWorld.c

# Mover um ficheiro
        $ git mv HelloWorld.c ./new/path/HelloWorld.c

# Forçar a alteração de nome ou mudança local
# "existingFile" já existe no directório, será sobre-escrito.
        $ git mv -f myFile existingFile

# Atualiza o repositório local, juntando as novas alterações
# do repositório remoto 'origin' e branch 'master'
# git pull <remote> <branch>
# git pull => aplica a predefinição => git pull origin master
        $ git pull origin master

# Juntar alterações do branch remote e fazer rebase commits do branch
# no repositório local, como: "git pull <remote> <branch>, git rebase <branch>"
        $ git pull origin master --rebase

# Envia e junta as alterações de um repositório local
# para um remoto denominado "origin" no branch "master".
# git push <remote> <branch>
# git push => aplica a predefinição => git push origin master
        $ git push origin master

# Faz Rebase de experimentBranch para master
# git rebase <basebranch> <topicbranch>
        $ git rebase master experimentBranch

# Restabelece a camada intermediária de registo para o último
# commit (o directório fica sem alterações)
        $ git reset

# Restabelece a camada intermediária de registo para o último commit, e
# sobre-escreve o projecto atual
        $ git reset --hard

# Move a head do branch atual para o commit especificado, sem alterar o projecto.
# todas as alterações ainda existem no projecto
        $ git reset 31f2bb1

# Inverte a head do branch atual para o commit especificado
# fazendo com que este esteja em sintonia com o directório do projecto
# Remove alterações não registadas e todos os commits após o commit especificado
        $ git reset --hard 31f2bb1

# remove HelloWorld.c
        $ git rm HelloWorld.c

# Remove um ficheiro de um sub-directório
        $ git rm /pather/to/the/file/HelloWorld.c