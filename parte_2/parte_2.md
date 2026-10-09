## Flujo colaborativo

1. Fork: Se debe entrar al repositorio remoto o GitHub del dueño del proyecto y generar un Fork en donde, se creará una "Copia" en GitHub del repositorio del dueño del proyecto principal.

2. Clone: Una vez creado el Fork, es necesario entrar al Fork creado de nuestra cuenta de GitHub y copiar el URL de ese repositorio. Nos dirigimos a VSC y nos colocamos en la terminal en el lugar donde queremos hacer la copia del repositorio, una vez elegido el lugar se utliza el comando: git clone URL y se pega el URL del Fork.

3. Modificar archivos: Una vez que entres al clone creado, podrás modificarlo activando el entorno virtual, descargando las dependencias y creando y modificando los demás archivos sin olvidar asegurarse que el entrono virtual no está dentro del repositorio.

4. Branch: Una vez hecho los cambios, lo suiguiente es crear una nueva rama para subir esos cambios, para ello es necesario usar el comando: "git switch -c Nueva rama", esto generará una nueva rama en tu repositorio, puedes confirmar que se haya generado con el comando "git branch".

5. Commit: Si la rama ya está lista, puedes revisar el estatus de tu repositorio con el comando "git status", si todo está listo puedes hacer "git add ." y finalemente el commit con el comando "git commit -m "Cambios"".

6. Push: Al estar el commit ya creado es necesario subir el cambio a GitHub, para ello se utiliza el comando de Push de la siguiente manera: "git push -u origin Nueva rama", en donde el nombre es el nombre de la rama que se creó, una vez ingresado el comando se subirá a GitHub la rama seleccionada.

7. Pull Request: En GitHub, el colaborador debe identificar que su rama se haya subido correctamente, de ser así, debe generar un Pull Request en su propio repositorio, solicitando una aceptaación al Dueño del proyecto donde se compara su rama Master con la rama que creó el colaborador.

8. Review: Por otro lado, el Dueño del proyecto verá que en su repositorio se generó un Fork y además, aparecerá que recibió un Pull Request, al entrar a los Pull Request recibidos podrá ver los cambios que está solicitando el colaborador. Puede aceptar los cambios o solicitar un ajuste o cambio con Request Changes y esperar a que el colaborador genere los cambios.

9. Merge: Finalmente si el proyecto cumple con lo que se desea, se genera un Merch en GitHub lo que fuciona el proyecto del colaborador con el del Dueño y se pueden sincronizar los repositorios cons Sync Fork y hacer un Pull para generar los cambios


## Fork y Clone

- "Clone crea una copia del proyecto dentro de mi cuenta de GitHub"

No la afirmación no es correcta, la funcionalidad del comando Clone se genera dentro de VSC, es decir, dentro de un repositorio local, por lo que al usar este comando la copia no se genera en nuestro GitHub se genera en nuestro equipo, por otro lado, Fork genera una "copia" del repositorio en GitHub que únicamente se encuentra ahí, por lo que es necesario hacer un Clone para tenerlo en nuestro repositorio local.

## Pull Request

- Supón que realizaste Fork, Clone, Branch, Modificar, Commit y Push. Responde: ¿los cambios ya forman parte
del repositorio original? ¿Qué debe ocurrir para incorporarlos?

No, con los pasos realizados aún los cambios no pertenecen al repositorio origianl, para que ocurra esto es necesario solicitar un Pull Request al Dueño del proyecto original y estos cambios deben ser aceptados y generar un Merge para poder ser unidors con el reopsitorio original.

## Request Changes

- El propietario revisa tu Pull Request y selecciona Request Changes. Explica qué debes hacer, si necesitas crear
otro Pull Request y qué ocurre cuando realizas nuevamente push.

Se deben generar los cambios solicitados por el Dueño, una vez hechos se puede generar un git push de la rama que se hicieron los cambios y no es necesario crear un Pull Request ya que el anterior generado registrará el nuevo repositorio subido por el colaborador que incluye los cambios.

## Merge y repositorio local

- Un Pull Request fue aceptado y se realizó Merge en GitHub. Sin embargo, el repositorio local del propietario no
contiene los cambios. Explica por qué sucede y qué operación debe realizarse.

Esto sucede ya que, aunque se sincronizaran los cambios al repositorio del Dueño, estos cambios se encuentran en GitHub, no en su repositorio local, para ver reflejado estos cambios es necesario utilizar un git pull en VSC para jalar los cambios realizados de GitHub.

## Sync Fork

- Tu Fork fue creado varios días atrás y el repositorio original recibió nuevos commits. Explica qué herramienta
utilizarías, qué repositorio se actualiza y qué diferencia existe entre Sync Fork y git pull.

Es necesario realizar un Sync Fork para sincronizar los cambios que se estén generando en el proyecto desde el último Fork creado ya que el repositorio que se actualiza ese el del Dueño, no el del colaborador, para que este vea los cambios es necesario sincronizarlos con Sync Fork y, una vez generados utilizar git pull para tomar los cambios.
La diferencia que existe es que Sync Fork actualiza el repositorio sincronizando los cambios hechos en GitHub, mientras que git pull jala los cambios del repositorio de GitHub a tu repositorio loca.