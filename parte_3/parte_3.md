## Analiza

git status: Muestra el estado del repositorio local en color rojo o verde.
git add README.md: Añade el archivo README.md a la zona de Stage del repositorio, únicamente este archivo es el que se envía a esta zona
git commit -m "Actualiza documentación": Se crea el commit en el repositorio local con los archivos que se encontraban en la zona de Stage
git push: Los commit realizados en el repositorio local son subidos a GitHub.

## Identifica qué falta

- Caso A

Modificar archivo
↓
git add .
↓
¿?
↓
git push

Hace falta el comando: git commit -m "" para generar el guardado al repositorio de los archivos que se encuentran en la zona de Stage y sean subidos con git push.

- Caso B:

Repositorio GitHub
↓
¿?
↓
Repositorio local

Se puede utilizar el Sync Fork en caso de que el colaborador no tenga una versión actual, de ser así, se utilizar el comando "git pull" para jalar los cambios de GitHub a tu repositorio local.

- Caso C:

Repositorio remoto actualizado
↓
¿?
↓
Repositorio local actualizado

Se utilza la función de Sync Fork para sincronizar los cambios del repositorio remoto y hacer un git pull para actualizar tu repositorio local.