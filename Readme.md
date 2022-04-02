Data de criação: 02.04.2022

### Treino de git baseado na apostila:
`documentos/apostilas.manuais.documentacao.etc/git/Guia_de_Utilizacao_do_Git.pdf`

E também no site:
(https://programadorviking.com.br/git-commit/)

### Comandos já usados/testados:

```git
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
```
