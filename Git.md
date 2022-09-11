# Git e Github

## Chaves SSH
Verificar se já existem chaves
```
ls -al ~/.ssh
```
Gerando par de chaves SSH
```
ssh-keygen -t ed25519 -C <endereço_email>
```
Imprimindo a Chave SSH pública (adicionar esta chave ao Github)
```
cat <chave_pública>
```
Inicializar Agente SSH (na pasta .ssh)
```
eval $(ssh-agent -s)
```
Adicionar a Chave Privada ao Agente SSH
```
ssh-add <chave_privada>
```
Exemplo:
```
ssh-add id_ed25519
```
## Comandos Git
### Configuração Inicial
Define o nome do autor dos commits
```
git config --global user.name "<nome>"
```
Define o e-mail do autor dos commits
```
git config --global user.email "<email>"
```

### Clone
Clonar Repositório
```
git clone <endereço_ssh_repositório>
```

### Repositórios
Iniciar um repositório do Git (dentro da pasta)
```
git init
```
Adiciona (stage) um arquivo ao Commit
```
git add <arquivo>
```
Adiciona (stage) todos os arquivos da pasta
```
git add *
```
Restora Alterações ainda não comitadas como adicionar ou remover arquivos
```
git restore <file>
```
Deleta o arquivo
```
git rm <file>
```
Comita as alterações
```
git commit -m "<mensagem_commit>"
```
### Ramos (Branches)
Cria um Ramo
```
git branch <nome_ramo>
```
Troca para outro ramo
```
git checkout <nome_ramo>
```
### Informações
Imprime o estado dos arquivos (untracked, staged, modified, unmodified)
```
git status
```
Lista todos os commits de um ramo (branch)
```
git log
```
Lista a referência de cada commit (usado nos resets)
```
git reflog
```
Lista todos os ramos (branches)
```
git branch
```
Lista configurações do git
```
git config --list
```
Lista origens dos repositórios remotos
```
git remote -v
```
### Reset
Reseta os arquivos para determinado commit (deleta arquivos)
```
git reset --hard <commit_ID>
```
Reseta os arquivos para um estado ainda não staged (antes do add) de determinado commit
```
git reset --mixed <commit_ID>
```
Reseta os arquivos para o estado staged de determinado commit
```
git reset --soft <commit_ID>
```
*Utilizar restore para restaurar arquivos alterados após reset.*
### Push
Adiciona a origem do repositório remoto
```
git remote add <nome_repositório_remoto> <endereço_https_repositório>
```
Exemplo:
```
git remote add origin https://github.com/victorhfsilva/Comandos-Terminal
```
Exemplo utilizando Access Token:
```
git remote add origin https://<token>@github.com/victorhfsilva/Comandos-Terminal.git
```
Deleta repositório remoto
```
git remote remove <nome_repositório_remoto>
```
Exemplo:
```
git remote remove origin
```
Empurra ramo ao repositório remoto
```
git push <nome_repositório_remoto> <ramo>
```
Exemplo:
```
git push origin master
```
## Pull
Puxa um ramo do repositório remoto
```
git pull <nome_repositório_remoto> <ramo>
```
Exemplo:
```
git pull origin master
```
