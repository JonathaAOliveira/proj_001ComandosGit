# ComandosGit
#Instalando GIT
apt-get install git-all

#Remover GIT terminal Linux [Desistalar]:
apt-get remove git
apt-get remove --auto-remove git
apt-get purge git
apt-get purge --auto-remove git

#Verificar versão
git --version

#Listar configurações do GIT
git config --global --list

#Adicionando configurações no GIT
git config --global user.name "JonathaAOliveira"
git config --global user.email jonatha.araujo.oliveira@gmail.com

#Obs: No linux o arquivo .gitconfig fica na pasta raiz "root"
nano .gitconfig

#Para criar um repositorio GIT
git init

#Ver status
git status

#Adicione arquivos não rastreados
git add arquivo.*

#Remover o arquivo de pronto para comitar , voltando para não rastreado
git rm --cached index.html

#Adicionar todos os arquivos não rastreados 
git add .

#Comitar "Finalizar a ação"

git commit -m "Adicionar arquivo index"

#Conjurando arquivos simuntaneos 

git add . && git commit -m "Mensagem"

#Historico de commits

git log

#Historico versão condensada

git log --oneline

#Tipos >>> Checkout | Revert | Reset
#Voltar ao estado sem alteração (checkout) | "Seguro"

git checkout 'b7d4981'

#Voltar ao estado original

git checkout master

#Reverter o commit : Essa ação fará reversão ao ponto indicado... Você ainda terá o historico mas não altera a originalidade | "Meio seguro"

git revert '4c3a61c'

#Reset Volta ao arquivo do ponto indicado, porem não tende a excluir arquivos futuros | "Não é seguro"

git reset '4c3a61c'

#Reset Volta ao arquivo do ponto indicado, porem excluindo todos os arquivos futuros | "Não é seguro"

git reset '4c3a61c' --hard


#Ignorar arquivos para o GIT não ficar monitorando....
touch .env // Exemplo de um arquivo de variavel de ambiente que pode conter acessos ao banco de dados....

touch .gitignore

#Branch -- geralmente utilizadas em feature "navas funcionalidades"
#listar todas as branchs

git branch

#adicionando um novo branch

git branch teste

#mudando de branch

git checkout teste

#conferindo branch

git branch

#Deletando uma branch

git branch -d teste

#Delete uma branch de qualquer forma

git branch -D teste 

#Renomeando branch

git branch -m NOMEDABRANCHANTIGA NOVONOMEDABRANCH

#Fundindo branchs






























