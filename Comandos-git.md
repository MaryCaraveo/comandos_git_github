# Comandos básicos de git

### Para abrir el editor de codigo VS Code.

- > `$ code`

### Para abrir el archivo en VS Code.

- > `$ code archivo.txt`

### Para visualizar la versión de git

- > `$ git --version`

### Para visualizar toda la configuración actual de git.

- > `$ git config`

### Para ver la configuración por defecto de git.

- > `$ git config --list`

### Para ver donde esta la configuración guardada (Solo para casos avanzados).

- > `$ git config --list --show-origin`

### Para cambiar la configuración del usuario de git.

- > `$ git config --global user.name "Guadalupe Caraveo"`

### Para cambiar la configuración del correo de git.

- > `$ git config --global user.email "correo@gmail.com"`

### Para inicializar el repositorio de git en la carpeta del proyecto.

- > `$ git init`

### Muestra el estado del proyecto (Para ver si hay cambio o no).

- > `$ git status`

### Para agrega un archivo editado a Staging donde se guarda temporalmente antes de ser enviado al repositorio.

- > `$ git add archivo.txt`

### Para agregar todos los archivos editados a staging donde se guarda temporalmente antes de ser enviado al repositorio.

- > `$ git add .`

### Sirve para eliminar archivos que ya no necesitemos mantener en nuestro repositorio.

- > `git rm`

### Para borrar el archivo del staging cuando se haya agregado con el comando `$ git add`.

- > `git rm --cached archivo.txt`

### Para enviar los cambios al repositorio, esto se realiza despues de haber agregado los cambios con `$ git add`.

- > `$ git commit -m "Mensaje del commit"`

### Para visualizar el historial de un archivo en especifico (commits).

- > `$ git log archivo.txt`

### Para mostrar el historial de los registros (commits) del proyecto.

- > `$ git log`

### para visualizar los cambios especificos en los archivos a partir del commit.

- > `git log --stat`

### Muestra los cambios que han existido sobre un archivo.

- > `$ git show`

### Para ver la diferencia entre una versión y otra.

- > `git diff commitA commitB.`

### Para volver a cualquier versión anterior de un archivo en específico o incluso del proyecto entero (ejemplo `git checkout + master + nombre archivo`).

- > `git checkout + ID del commit`

### Esta también es la forma de crear ramas y movernos entre ellas.

- > `git checkout + Nombre_branch`

### Permite regresar a una versión anterior y sobreescribir toda la historia. Se borraran los cambios que se hicieron despues de este commit (Ejemplo `git reset <ID commit>`).

- > `$ git reset`

### Borra toda la información que tengamos en el área de staging (Se borra todo definitivamente).

- > `--hard`

### Mantiene los archivos en el área de staging para poder aplicar los últimos cambios pero desde un commit anterior.

- > `--soft`

### Sirve para mover los archivos que no quisieramos incluir en el commit que realizaremos. De esta manera mantenemos los cambios, pero no lo registramos en el commit. Hasta que estemos seguros de incluirlo.

- > `git reset HEAD`

### Para borrar commits.

- > `git branch -d`

### Nos permite descargar los archivos de la última versión de la rama principal y todo el historial de cambios en la carpeta .git.

- > ` git clone url_del_servidor_remoto`

### Luego de hacer git add y git commit debemos ejecutar este comando para enviar los cambios al servidor remoto.

- > `$ git push`
- > `$ git push origin master`

### Se usa para traer actualizaciones del servidor remoto y guardarlas en nuestro repositorio local. También usamos el comando `git fetch` con servidores remotos.

- > `$ git fetch`

### Se utiliza para combinar los últimos cambios del servidor remoto y nuestro directorio de trabajo (ejemplo `git merge "nombre de la rama"`).

- > `git merge`

### Básicamente, git fetch y git merge al mismo tiempo.

- > `$ git pull`

### Para actualizar la información del repositorio master al local.

- > `$ git pull origin master`

### Para agregar un origin remoto de los archivos.

- > `git remote add origin "link del repositorio en git"`

### Para mostrar el repositorio remoto.

- > `git remote`

### Comando para verificar que la URL se haya guardado corretamente, nos deberia traer la url donde hariamos el fecht y el push.

- > `git remote -v`

### Para forzar los cambios cuando existen historias o commit diferentes.

- > `git pull origin master --allow-unrelated-histories`
