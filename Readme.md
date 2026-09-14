#### Nombre del estudiante: Raúl Alejandro Hernández Quilantán
#### Matricula: 2630268
## Creación y sincronización de repositorios con Git y GitHub

### Objetivo de la práctica:

#### El objetivo de esta práctica fue aprender a crear y administrar un repositorio local utilizando Git, vincularlo con un repositorio remoto en GitHub y comprobar la sincronización de información desde el repositorio local hacia GitHub y viceversa

### Descripción del procedimiento realizado:

#### Primero hice una carpeta llamada: practica-git-RaúlAlejandro-HernandezQuilantan, dentro de ella inicialize el repositorio de Git y estableci main como la rama principal, despues hice los archivos Readme y datos.txt, verifique el estado del repositorio, agregue los archivos al area de preparacion y realize el primer commit. Hice un repositorio en GitHub con el mismo nombre y lo vincule con el repositorio local, realize un push para enviar los archivos locales a GitHub, modifique datos desde la aplicacion y el cambio se transfirio al repositorio local por git pull origin main luego realize otra modificación en datos desde la carpeta. El cambio lo agregue a staging, lo registre por un commit y lo envie otra vez a GitHub por git push


|Comandos utilizados|Explicación breve de la función de cada comando|
|-------------------|-----------------------------------------------|
git init|Inicializa un repositorio de Git dentro de una carpeta
git branch -M main|Cambia el nombre de la rama actual a main
git status|Muestra el estado actual del repositorio y los archivos que tienen cambios
git add .|Agrega los archivos modificados al área de preparación 
git commit -m "Primer commit"|Registra los cambios preparados en el historial del repositorio
git remote add origin URL_DEL_REPOSITORIO|Agrega un repositorio remoto y lo identifica con el nombre origin
git remote set-url origin URL_DEL_REPOSITORIO|Cambia la dirección del repositorio remoto asociado a origin
git remote -v|Muestra las direcciones de los repositorios remotos configurados.
git push -u origin main|Envía la rama main y sus commits desde el repositorio local hacia GitHub
git pull origin main|Descarga los cambios de la rama main de GitHub y los integra en el repositorio local
git push|Envía al repositorio remoto los commits locales que todavía no se encuentran en GitHub

### Explicación de cómo se creó el repositorio local

#### Primero hice  una carpeta para almacenar los archivos de la práctica. Despues abri la PowerShell dentro de dicha carpeta y se ejecuto:
~~~
git init
~~~
#### Este comando convirtio la carpeta en un repositorio local de Git y estableci la rama principal con el nombre main mediante:
~~~
git branch -M main
~~~
#### Despues hice readme.md y datos.txt, los agregue al area de preparación por git add . y tambien hice el primer registro en el historial utilizando:
~~~
git commit -m "Primer commit"
~~~

### Explicación de cómo se vinculó el repositorio local con GitHub

#### Primero hice un repositorio público y vacío en GitHub. Después use la URL del repositorio para establecer la conexión entre el repositorio local y el remoto

~~~
git remote add origin URL_DEL_REPOSITORIO
~~~

#### Comprobe la configuración con el comando:

~~~
git remote -v
~~~

#### Durante el proceso corregi la URL del repositorio remoto, por lo que utilize git remote set-url origin para establecer la dirección correcta. Finalmente ejecute:

~~~
git push -u origin main
~~~

#### para enviar por primera vez el contenido del repositorio local a GitHub


### Explicación de la sincronización Local → GitHub

####  Para comprobar la sincronización desde el repositorio local hacia GitHub, primero realize unos cambios en datos.txt desde la computadora. Despues utilize:

~~~
git add .
git commit -m "Actualización desde repositorio local"
git push
~~~

### Explicación de la sincronización GitHub → Local

#### Para comprobar el flujo contrario, primero modifique datos.txt directamente desde GitHub. Después regrese al repositorio local y se ejecutó:

~~~
git pull origin main
~~~
#### El comando descargo los cambios en GitHub y los integró en el repositorio local. Al abrir nuevamente datos.txt, comprobe que el cambio realizado desde GitHub también estaba disponible en la computadora

### Descripción de los archivos contenidos en el repositorio

#### Readme.md: Es el archivo utilizado para documentar la práctica. Contiene información sobre el objetivo, procedimiento, comandos utilizados, sincronización entre Git y GitHub y las conclusiones obtenidas

#### Datos.txt: Es un archivo de texto utilizado para comprobar el intercambio de cambios entre el repositorio local y GitHub. Durante la práctica fue modificado desde GitHub y posteriormente desde el repositorio local

### Conclusión personal sobre lo aprendido

#### En esta práctica aprendi a crear un repositorio local utilizando PowerShell y a conectarlo con un repositorio remoto en GitHub ademas aprendi la funcion de los comandos git add, git commit, git push y git pull.Con esta practica comprobe que los  cambios se podian enviar desde la laptop hacia GitHub por push o descargarse desde ahi por pull