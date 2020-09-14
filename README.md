# git-github 💚
Este repositorio lo hice por un curso de [Git](https://git-scm.com/ "Git") y [GitHub](https://github.com/matiasnnr "GitHub") que hice, en el cual aprendí a trabajar con la línea de comandos y también con las funciones que entrega GitHub en su página web

*No soy un experto en git ni github, pero me sé manejar sin mayores problemas*

**Algunas cosas que vimos en el curso:**
- Todos los comandos de Git
- El flujo de trabajo en GitHub
- Buenas prácticas
- Algunos truquillos 😆


**A continuación, una lista de comandos que podrían ser de ayuda 🙂**

Git Commands and Terminal / Comandos de GIT y Terminal
============

_A list of commonly used Git and Terminal commands_

*Una lista de los comandos más utilizados en Git y la Terminal*

--

### Terminal Commands / Comandos de la Terminal

| Command | Description | Descripción |
| ------- | ----------- | ------------ |
| `cd [rute]` | To change directory | Cambia el directorio |
| `mkdir [name]` | Make directory | Crea una nueva carpeta |
| `ls -a` | List information about the files | Lista los archivos del directorio |
| `clear` | clear the terminal screen | Limpia la Terminal |
| `Touch [name.txt]` | create a empty file | Crea un archivo vacio |
| `rm [file]` | remove files | Elimina un archivo |
| `rm -rf [dir]` | remove directories | Elimina una carpeta |
| `pwd` | Print name of current/working directory | Muestra el directorio donde nos encontramos |
| `mv` | move (rename) files | Mueve o renombra archivos |
| `cat [name.txt]` | Concatenate files and print on the standard output | Vista previa del contenido del archivo |
| `sudo` | execute a command as another user | Ejecuta un commando como administrador |

### Config Git / Configuración de Git

| Command | Description | Descripción |
| ------- | ----------- | ------------ |
| `git config --global user.name "name-example"` | Add a user name | Añade un nombre de usuario |
| `git config --global user.email user@example.com` | Add a email for user | Añade un correo del usuario |
| `git config --list` | List all setings | Muestra todas las configuraciones |

### Config SSH Keys / Configuración de Credenciales SSH

| Command | Description | Descripción |
| ------- | ----------- | ------------ |
| `ssh-keygen -t rsa -b 4096 -C "Email"` | Generate SSH key | Generar credencial SSH |
| `eval $(ssh-agent -s)` | Verify ssh agent | Verifica la existencia del servidor de credenciales SSH |
| `ssh-add [rute]` | Add SSH key to your workspace | Agrega la credencial SSH al entorno de trabajo |

### Creating Projects / Creación de proyectos

| Command | Description | Descripción |
| ------- | ----------- | ------------ |
| `git init` | Initialize a local Git repository | Inicia un repositorio local de Git |
| `git clone [url]` | Create a local copy of a remote repository | Crea una copia local de un repositorio remoto |

### Basic Snapshotting / Snapshooting Básico

| Command | Description | Descripción |
| ------- | ----------- | ----------- |
| `git status` | Check status | Verifica el estatus del repositorio |
| `git add [file-name.txt]` | Add a file to the staging area | Añade un archivo al area de preparación |
| `git add .` | Add all new and changed files to the staging area | Añade todos los archivos al area de preparación |
| `git commit -m "[commit message]"` | Commit changes | Añade los archivos al repositorio |
| `git commit -am "[commit message]"` |Add changed files and commit | Añande los cambios y hace commit |
| `git rm -r [file-name.txt]` | Remove a file (or folder) | Elimina archivos o carpetas |
| `git commit --ammend` | Ammend the last commit | Agrega los cambios al último commit en caso de error |

### Branching & Merging / Ramas y fusionar

| Command | Description | Descripción |
| ------- | ----------- | ----------- |
| `git branch` | List branches (the asterisk denotes the current branch) | Lista todas las ramas |
| `git branch -a` | List all branches (local and remote) | Lista todas las ramas locales y remotas |
| `git branch [branch name]` | Create a new branch | Crea una nueva rama |
| `git branch -d [branch name]` | Delete a branch | Elimina una rama |
| `git show-branch --all` | List all branches local | Lista todas las ramas en local |
| `git push origin --delete [branch name]` | Delete a remote branch | Elimina una rama remota |
| `git checkout -b [branch name]` | Create a new branch and switch to it | Crea una nueva rama y cambia a ella |
| `git checkout -b [branch name] origin/[branch name]` | Clone a remote branch and switch to it | Clona una rama remota y cambia a ella |
| `git checkout [branch name]` | Switch to a branch | Cambiar a una rama determinada |
| `git checkout -` | Switch to the branch last checked out | Cambia a la ultima rama seleccionada |
| `git checkout -- [file-name.txt]` | Discard changes to a file | Descarta los cambios de un archivo |
| `git merge [branch name]` | Merge a branch into the active branch | Fusiona una rama a la rama activa
| `git merge [source branch] [target branch]` | Merge a branch into a target branch | Fusiona una rama a una rama determinada |
| `git stash` | Stash changes in a dirty working directory |
| `git stash clear` | Remove all stashed entries |

### Sharing & Updating Projects / Compartiendo y Repositorios Remotos

| Command | Description | Descripción |
| ------- | ----------- | ----------- |
| `git push origin [branch name]` | Push a branch to your remote repository | Envia el repositorio local a remoto |
| `git push origin --delete [branch name]` | Delete a remote branch | Elimina un repositorio remoto |
| `git pull` | Update local repository to the newest commit |
| `git pull origin [branch name]` | Pull changes from remote repository | Hace un feth y fusiona
| `git remote add origin ssh://git@github.com/[username]/[repository-name].git` | Add a remote repository | Crea un repositorio remoto |
| `fork` | Copy a external repository | Copa un repositorio externo |
| `git remote -v` | list remote connections | Lista las conexiones remotas |
| `git remote set-url [branch name] [url]` | Change the url | Cambia la url del repositorio |

### Inspection & Comparison / Inspección y Comparación

| Command | Description | Descripción |
| ------- | ----------- | ----------- |
| `git log` | View changes | Muestra los cambios en el repositorio |
| `git log --summary` | View changes (detailed) | Muestra los cambios en el repositorio detalladamente |
| `git log -all --graph --decorate --oneline` | View changes (Max-detailed) | Muestra todos los cambios del repositorio detallada y gráficamente |
| `git diff [source branch] [target branch]` | Preview changes before merging | Compara los diferentes cambios |


### Others / Otros

| Command | Description | Descripción |
| ------- | ----------- | ----------- |
| `alias [name=] "command"` | Create a shorcut for a command | Crea un alias para llamar a un comando |
| `git tag -a [name] -m "message" [id/hashtag]` | Create a tag for a commit | Crea un tag de un commit en especifico |
| `git show-ref --tags` | List all tags | Lista los tags existentes |
| `git push --tags` | Push tags to your repository | Envia los tags al repositorio remoto |
| `git tag -d [name]` | Delete a tag | Elimina un tag en especifico |
| `git push origin :refs/tags/[name]` | Delete a tag from GitHub | Elimina un tag dentro de GitHub |
| `gitk` | Open GUI | Abre una interfaz grafica |
| `git cherry.pick [id]` | Take commit from other branches | Trae un commit especifico desde otra rama |
| `git grep -n [word]` | Search words in the proyect | Busca la palabra especificada en todo el proyecto |
