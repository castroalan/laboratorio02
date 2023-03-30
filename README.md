# COMANDOS APRENDIDOS#

## GIT
Sistema de contro de control de versiones, es una herramienta fundamental para el desarrollo de cualquier proyecto.
Permite mantener un historial de cambios en los archivos, evitar la pérdida de datos, facilitar la colaboración en equipo y mejorar la gestión de cambios en el proyecto.

## ARCHIVOS BINARIOS Y ARCHIVOS DE TEXTO
No es necesario hacer commit de archivos binarios debido a que pesan mucho.

## GIT INIT
`git init`: iniciará un nuevo repositorio, git en el directorio actual.

## GIT ADD
`git add`: agrega los cambios de un archivo especifico

## GIT ADD.
`git add .`: agrega todos los cambios de los archivos.

## GIT STATUS
`git status`: ver los cambios que se han agregado

## GIT BRANCH
`git branch`: visualizar las diferentes ramas o variaciones de la historia del producto.

## GIT CHECKOUT
`git checkout`: sirve para cambiar la nueva rama, navegar en las diferentes ramas y al commit que deseo ir.
`git checkout -b`: desde el punto donde yo estoy crea una rama y se pasa a la siguiente.

## GIT MERGE
`git merge`: sirve para fusionar la nueva rama con la rama principal del repositorio. Unir dos archivos de diferentes ramas.

## STAGING
`staging`: carpeta local donde hacemos las modificaciones en el ambiente de desarrollo 

## MERGE
cambiar a la rama de destino: primero se debe cambiar la rama del destino en la que se desean fusionar los cambios utilizando el comando git checkout y la rama del destino.

## MERGE RESOLUCION DE CONFLICTOS
El merge se puede hacer de forma automática o manual, si git detecta que no interfieren entre si el merge se realiará automáticamente.


## PARA REGRESAR AL TIEMPO
`git checkout <ID del commit>` para crear una rama desde una version anterior git branch <nombre de la nueva rama><ID del commit>

## REPOSITORIO REMOTO
`git remoto add <nombre del repositorio> <URL del repositorio>`

REPOSITORIO REMOTO: es una version de tu proyecto que se encuentra alojada en un servidor remoto, en lugar de en tu computadora local.
REPOSITORIO PUBLICO: ACCESO PARA CUALQUIERA.
REPOSITORIO PRIVADO: ACCESO PARA LAS PERSONAS QUE YO DESEE.
Se pueden tener muchos repositorio de manera remota.

## PETICION DE CAMBIOS (PULL REQUEST)
Es una forma de solicitar que un colaborador revise y apruebe tus cambios, antes de fusionarlos con la rama principal del proyecto. 


## REVERTIR LOS CAMBIOS 
`git revert`: <ID del commit> esto creará un nuevo commit que deshace los cambios realizados en el commit anterior.

Se trabaja en la misma rama, se regresan los cambios, lo que hay por delante queda en staging area para consolidar.

`git reset --soft`: suponiendo que deja de existir la ultima version.

`git reset`: permite deshacer cambios sin crear un nuevo commit. Esto es útil si deseas deshacer varios cambios en un solo comando.

`git hard reset`: los cambios se eliminan y es como si no existieron.


## GIT LOG
`git log`: sirve para ver todos los commit realizados.

## GIT COMMIT -M
`git commit -m`: funciona para realizar los comentarios de los cambios realizados, documentar cada uno de ellos.

## GIT DIFF
`git diff <archivo>`: mostrará las diferencias entre el archivo actual y su última versión guardada.


`git diff <hash>`: verificar una version especifica del archivo con la version actual.
<hash> es el numero de identificacion del commit que contiene la version del archivo que se desea comparar.

## GESTION DE MASTER
Es la posibilidad de gestionar en una rama una linea independiente de desarrollo que se deriva de otra rama, normalmente la rama principal (también llamada "master" o "main").


## GIT PUSH ORIGIN MASTER
`git push origin master`: sincronizar nuestros cambios en el local con el repositorio remoto

## GIT PULL
`git pull`: cuando hagamos cambios en nuestro repositorio remoto y para que se sincronice en el local.


## ¿Que son los tags?
- Los tags o etiquetas se parecen al mensaje del commit.
- Son identificadores asociados a versiones especificas de un repositorio.
- Debemos usarlas para versionamiento productivo.
- Estos versionamientos pueden ser lanzamiento de software o marcar hitos importantes.
> version Alpha: Es el punto mas bajo del sistema.

> version Beta: Es el punto intermedio del producto (version semiestable).

> version release: de ellas se espera que esten mas cerca a produccion.

> version 1.0: es la mas estable que se logra conseguir.

> con **git tag** tenemos un identificador estatico.

> podemos usar **git checkout tag** para llegar a un identificador del punto de la historia.

## Comandos para la creacion de un tag
- **git tag v1.0** para asignar el tag.
- **git tag -s v1.0** envia un parametro al comando para firmar los tags.
- **git push -tags** para publicar los tags
- **git show v1.0** para mostrar informacion de un tag como si fuera un git log.

## Comandos para GIT fetch, pull y push
- **git fetch** descarga los cambios de un repositorio remoto a local.
- **git pull** combina automaticamente los cambios del repositorio remoto con la rama actual en tu repositorio actual.
- **git push** se usa para enviar cambios en la rama actual de tu repositorio local al repositorio remoto.
