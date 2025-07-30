## configurar
```c
git config --list --show-origin
git config --global user.name "tbrzc"
git config --global user.email javillabonmo@gmail.com
git config --global core.editor "'C:/Program Files/Neovim/bin/nvim.exe'"
git config --global init.defaultBranch main
git config --global core.eol lf
git add --renormalize . // si se cambia a lf
```
```sh
git init
git remote -v 
git checkout -b main # -b → Crea una nueva rama antes de cambiar a ella.
git remote add origin https://github.com/tu-usuario/NOMBRE_REPO.git
```
- Clonar con otro nombre, un proyecto
```
git clone https://github.com/libgit2/libgit2 mylibgit
```
- Rastrear archivos
El comando `git add` puede recibir tanto una ruta de archivo como de un directorio; si es de un directorio, el comando añade recursivamente los archivos que están dentro de él.
```
git add README
```
```
git commit -m "soy un commit"
git commit --allow-empty-message -m ""
```

## SSH
```sh
ssh-keygen -t ed25519 -C "javillabonmo@gmail.com"
cat .ssh/ed25519.pub
git clone git@github.com:tbrzc/REPOSITORY.git
ssh -T git@github.com #comprueba el usuario
```

## CLI
```sh
gh auth login
gh repo create tbrzc-notes/NOMBRE_REPO --private --add-readme
gh repo clone ORGANIZACION/NOMBRE_REPO
gh repo list tbrzc-notes # listar los repos de la organizacion
```

## delta
```sh
git config --global core.pager delta
git config --global interactive.diffFilter 'delta --color-only'
git config --global delta.navigate true
git config --global merge.conflictStyle zdiff3
```


```c
git add .
git add file.txt

git commit -m ""
git log // ver todo el historial de commits
```

```c
# Hiciste cambios en varios archivos, aún sin commit
git status
# output: modified: archivo1.cs, new file: archivo2.txt

# Guardar los cambios sin commit
git stash -u  // incluye archivos sin agregar (untracked)

# Cambiar de rama para arreglar un bug urgente
git checkout main
# Arreglas y haces commit en otra rama...

# Volver a tu rama de trabajo
git checkout feature/nueva-funcionalidad

# Recuperar los cambios
git stash pop

```