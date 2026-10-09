## Coneptos

1. Explica la diferencia entre Git y GitHub.

Git representa un repositorio local que se encuentra dentro de nuestro equipo, mientras que GitHub es un repositorio remoto en la nube donde podemos almacenar nuestro repositorio local.

2. Explica para qué sirve .gitignore.

El archivo .gitignore sirve para colocar los arhcivos que no deseamos que sean subidos al repositorio remoto de GitHub y no sean visbles o funcionales.

3. Explica por qué .venv no debe almacenarse normalmente en GitHub.

.venv no debe ser almacenado ya que contiene demasiados archivos que podrían saturar el repositorio remoto y no es necesario subirlo ya que puede ser descargado por el colaborador en su equipo local.

4. Explica para qué sirve requirements.txt.

El archivo requirements.txt sirve para colocar las dependencias del proyecto con el que se trabaja, al decir dependencias son las librerías descargadas y que son necesarias para que funcione el programa.

5. Explica la diferencia entre Stage, Commit y Push.

Stage es la zona donde se colocan los archivos que se encuentran listos para hacer commit y subirse el repositorio local con sus cambios.
Commit es el guardado y actualización del repositorio local con los arhcivos que se encontraban en la zona de Stage
Push es el comando necesario para subir el repositorio local al repositorio remoto o en la nube de GitHub.

6. Explica por qué un repositorio puede tener varios commits antes de realizar un push.

Se pueden generar varios cambios dentro del proyecto, una vez generado un commit y se haga un cambio este debe ser registrado y actualizado en el repositorio local, por ello, se pueden generar varios commits, además, generas un historial de cambios dentro de tu repositorio local, lo que permite crear cambios y, de ser necesario, regresar a una versión anterior de tu proyecto para corregir o generar otro cambio y finalemtne hacer un push para guardar esos cambios a GitHub.