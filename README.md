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




