## configurar
```c
git config --list --show-origin
git config --global user.name "tbrzc"
git config --global user.email javillabonmo@gmail.com
git config --global core.editor "'C:/Program Files/Neovim/bin/nvim.exe'"
git config --global init.defaultBranch main
```
```
git init
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
```