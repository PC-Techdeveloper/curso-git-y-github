### GIT:

REPOSITORIO REMOTO EN GITHUB DESDE GIT

https://docs.github.com/es/get-started/getting-started-with-git/managing-remote-repositories <-- Enlace Github Docs

COMANDOS BÁSICOS EN GIT:

-- ls: Muestra una lista de archivos.

-- git add <archivo>: Incluir los cambios del o de los archivos en el commit, añade un nuevo archivo. Atajo: git add -A o git add . (Añade todos los archivos), tres estados (área de trabajo, área de preparación y área de confirmación).

-- git status: Ver el estado de los archivos sobre las ramas actuales.

-- git commit -m "descripción del código": Establece un punto de control en el proceso de desarrollo el cual permite volver más tarde si es necesario.

-- git push <nombre-remoto> <nombre-de-la-rama>: Envía los commits al repositorio remoto después de confirmar los cambios. Para cargar y subir la rama se usa el comando git push --set-upstream <nombre-remoto> <nombre-de-la-rama> o git push -u origin <nombre-de-la-rama>

-- git pull <nombre-remoto>: Recibe actualizaciones del repositorio remoto.

-- git revert: Deshacer los cambios que se han realizado.

-- git log: Muestra información de los commit realizados.

-- git clone <https://link-con-nombre-del-repositorio>: Descargar el código fuente existente desde un repositorio remoto (Github), ya que realiza una copia idéntica de la última versión de un proyecto en un repositorio y la guarda en el ordenador.

RAMAS EN GIT:
Una rama (Branch - Branches) en Git es una línea independiente de desarrollo en el repositorio, la línea de tiempo en el branch son: En vivo, Rama main (Rama principal).

Crear una rama en Git:
-- git branch <nombre-de-la-rama>: Creará una rama en local. Para envíar (push) la nueva rama al repositorio remoto se utiliza el comando git push <nombre-remoto> <nombre-de-la-rama>

Visualización de ramas:
-- git branch
-- git branch --list

Eliminar una rama: Aplica para las ramas locales en Git, NO en las ramas que ya están en GitHub
-- git branch -d <nombre-de-la-rama>

-- git checkout <nombre-de-la-rama>: Permite cambiar de una rama a otra, también se usa para chequear archivos y commits.

- Pasos para cambiar exitosamente de ramas:

1. Los cambios en la rama actual tienen que ser confirmados o almacenados en el guardado rápido (Stash) antes de que cambie de rama.

2. La rama a la que se quiera cambiar debe existir en local.

- Comando de acceso directo que permite crear y cambiar esa rama al mismo tiempo:

-- git checkout -b <nombre-de-la-rama>: Este comando crea una nueva rama en local (-b cambia a la rama que acabas de crear).

Cambiar el nombre de una rama en Git:
1 Método: Estar en la rama que quieres al cual le cambiarás el nombre y utilizar el comando git branch -m <nombre-de-la-nueva-rama>

2 Método: No es necesario estar en la rama a la cual se modificará, usa el comando git checkout <nombre-de-la-rama-principal> <nombre-de-la-nueva-rama> y los cambios se verán afectados de una manera más rápida.

CREAR COMMITS EN LAS RAMAS (NO EN LA RAMA MAIN):

-- git checkout <nombre-de-la-rama>: Usar el comando git branch para ver el historial de las ramas creadas, luego git checkout <nombre-de-la-rama> para cambiar de rama y realizar la modificación, por último realizar el commit guardando los cambios. Regresar a la versión anterior y notarás que tienes dos versiones diferentes por arte de magia.

GIT LOG PARA LAS RAMAS: Permite ver el historial del proyecto, filtrarlo y buscar cambios concretos. Mientras que el `git status` permite examinar el directorio de trabajo y el entorno de esanyo, git log solo muessra el historial confirmado.

# FUSIONAR RAMAS (MERGE):
Es un proceso que permite combinar varias líneas independientes de desarrollo en una sola rama (Para fusionar dos ramas, debes estar en la rama que RECIBIRÁ la fusión).

-- Fusionar una rama con la rama main:


