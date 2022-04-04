Data de criação: 02.04.2022

### Treino de git baseado nas apostilas:
`documentos/apostilas.manuais.documentacao.etc/git/Guia_de_Utilizacao_do_Git.pdf`
`documentos/apostilas.manuais.documentacao.etc/git/tutorial_git_github.pdf`

E também no site:
(https://programadorviking.com.br/git-commit/)

### Comandos já usados/testados:

```git
# Configuracao
# Para o projeto
git config --local
# Configuracao global
git config --global
# Mudar apenas o nome no projeto
git config --local user.name "Meu Nome"
# Visualizar o nome/email
git config user.name
git config user.email

# Comandos basicos
git init
git add .
git commit -m "Primeiro commit."
git remote add origin https://github.com/dorensbach/reaprendendo-git-2022.git
git push origin master
git add arquivo-02
git status

# Adicionar um branch (ramo)
git checkout -b ramo2
git checkout master
git checkout ramo2
git push origin ramo2

# Remover um branch
git checkout -b ramo3
git add arquivo-ramo3
git branch -d ramo3
git branch -D ramo3

# Merge
git checkout master
git status
git merge ramo2
git push origin master

# Ver diferenca entre 2 branch
git diff master ramo2

# Listar os remotes existenes
git remote -v

# Clonar um repositorio (SSH)
git clone git@github.com:dorensbach/reaprendendo-git-2022.git
#Tambem pode ser (HTTPS):
git clone https://github.com/dorensbach/reaprendendo-git-2022.git

# Buscar por alteracoes no servidor remoto
git pull origin master

# Mostra o historico de commits
git log
git log --oneline
git log -p

# Desfazer um commit
# Pegar o codigo do commit com o git log
git revert codigo
# Usar o push para enviar o revert pro remote
git push origin master

# Para mostrar para o git quais arquivos ele não deve monitorar, criar um arquivo
# com o nome .gitignore e incluir nele o nome dos arquivos que deverão ser ignorados.
```
### SSH
#### Criar chave e adicionar ao ssh-agent
(https://docs.github.com/pt/get-started/getting-started-with-git/managing-remote-repositories#switching-remote-urls-from-https-to-ssh)
Importante usar o comando `eval "$(ssh-agent -s)"`
#### Adicionar chave à conta
(https://docs.github.com/pt/authentication/connecting-to-github-with-ssh/adding-a-new-ssh-key-to-your-github-account)
#### Mudar a url remota de HHTP para SSH
https://docs.github.com/pt/get-started/getting-started-with-git/managing-remote-repositories#switching-remote-urls-from-https-to-ssh
