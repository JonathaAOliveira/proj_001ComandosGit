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

#Zera tudo até o momento da criação da branch
git reset HEAD --hard


#Ignorar arquivos para o GIT não ficar monitorando....
touch .env // Exemplo de um arquivo de variavel de ambiente que pode conter acessos ao banco de dados....

touch .gitignore

#Branch -- geralmente utilizadas em feature "navas funcionalidades"
#listar todas as branchs

git branch

#adicionando um novo branch

git branch teste

ou

git branch -b teste "Em casos do primeiro comando não dá certo"

#adicionando uma nova branch com todos os arquivos atualizados no momento.... "Repositorio online"
git checkout -b release/alfanumerico origin/release/alfanumerico

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

git merge NOMEDOBRANCH

#atualiza seu repositório local com as últimas alterações de todos os repositórios remotos que você configurou.

git fetch --all

----------////--------------

#Subir alterações para o GITHUB
#git push envia as suas alterações locais (aqueles commits que você fez) para um repositório remoto.

git push git@ithub.com:JonathaAOliveira/testes master

git remote 

#Configurando chave SSH
ssh-keygen -t ed25519 -C "your_email@example.com"

Comando para criar a Chave SSH no formato RSA
ssh-keygen -t rsa -b 4096 -C "jonatha.araujo.oliveira@gmail.com"

Cópiar chave SSH, Exemplo:

cat /root/.ssh/id_rsa.pub























