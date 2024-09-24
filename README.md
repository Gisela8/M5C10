# M5C10-CHECKPOINT_10


# _**¿Qué es Git? para qué se usa, que beneficios tiene. ¿para tí sería obligatorio el uso?**_

Git es un software de control de versiones. Su finalidad es llevar el registro de los cambios  de archivos de proyectos, además de ayudar a  coordinar el trabajo entre los diferentes participantes de dichos proyectos como repositorio del código.

Algunas características importantes son:

- Fuerte apoyo al desarrollo no lineal,  rapidez en la gestión de ramas y mezclado de diferentes versiones. 
      
- Git  da a cada programador/desarrollador una copia local del historial del desarrollo entero, y los cambios se propagan entre los repositorios locales. Los cambios se importan como ramas adicionales y pueden ser fusionados en la misma manera que se hace con la rama local.
      
- Los almacenes de información pueden publicarse por HTTP, FTP, rsync o mediante un protocolo nativo, ya sea a través de una conexión TCP/IP simple o a través de cifrado SSH.  - Gestión eficiente de proyectos grandes,  optimización de velocidad de ejecución.

- Un flujo de trabajo de Git es una fórmula que permite realizar un trabajo de forma productiva.


Órdenes básicas:

- gt init: Esto crea un subdirectorio nuevo llamado .git, el cual contiene todos los archivos necesarios del repositorio 

- git fetch: Descarga los cambios realizados en el repositorio remoto.
     
- git merge <nombre_rama>: recoge los cambios realizados en la rama “nombre_rama”.
      
- git pull: Unifica los comandos fetch y merge en un único comando.
      
- git commit -m <mensaje>: Confirma los cambios realizados. 

- git push origin<nombre_rama>: Sube la rama “nombre_rama” al servidor remoto.

- git status: Muestra el estado actual de la rama.
      
- git add <name_archivo>: Comienza a trackear el archivo “name_archivo”.
      
- git branch: Lista todas las ramas locales.

- git brach -a  Lista todas las ramas locales y remotas.
      
      
# _**¿Qué es Github? para qué se usa, que beneficios tiene. ¿para tí sería obligatorio el uso?**_ 

GitHub es una plataforma de desarrollo colaborativo que permite alojar poyectos en la nube utilizando el sistema de control de versiones llamado Git. 
Ayuda a los desarrolladores a almacenar el código llevando un registro de cambios. 

Ofrece integración con herramientas com Travis CI, CircleCI que permiten la ejecución automática de pruebas, cuando se envían nuevos cambios al repositorio.
El código es abierto generalmetne y permite realizar proyectos en común y mantener el seguimiento detallado de su progreso.

La plataforma GitHub también funciona como red social conectando a los desarrolladores con los usuarios. 
Proporciona herramientas para mantener documentación y wikis.
Acepta cualquier lenguaje de programación.

 # _**¿Existen otras opciones? en caso de que sea afirmativo ¿por qué utilizarías github?**_
 
GitLab, Bitbucket, Sourceforge.

Github está  compuesto por una comunidad de colaboradores y desarrolladores muy amplia. 
además de su apoyo a un código abierto. Es la más antigua del mercado se creo en 2008.


# _**¿Qué hace un archivo .gitignore? para qué se usa, que beneficios tiene. ¿para tí sería obligatorio el uso?**_

- Los archivos . gitignore contienen patrones que establecen coincidencias con los nombres de archivo del repositorio para determinar si deberían ignorarse o no. 
  Es un archivo de texto que le dice a Git qué archivos o carpetas ignorar en un proyecto.

- Un archivo local .gitignore generalmente se coloca en el directorio raíz de un proyecto. 
  También se puede crear un archivo global .gitignore, y cualquier entrada en ese archivo se ignorará en todos los  repositorios de Git.

- Para crear un archivo .gitignore local, se crea un archivo de texto y se asigna el nombre ".gitignore" 
  Cada nueva línea se debe incluir un archivo o carpeta adicional que se quiere que Git  ignore.
  
   * se utiliza como una coincidencia comodín.
      
   / se usa para ignorar las rutas relativas al archivo .gitignore.

   # es usado para agregar comentarios
      
   Ejemplo  .gitignore : # Ignora la carpeta naia_exercises


- Para agregar o cambiar  .gitignore global, se ejecuta el siguiente comando en la terminal:

  git config --global core.excludesfile ~/.gitignore_global

  Esto creará el archivo ~/.gitignore_global. Ahora se puede editar ese archivo de la misma manera que un archivo .gitignore local. 
  Todos los repositorios Git ignorarán los archivos y carpetas listadas en el .gitignore global.

- Para evitar el rastreo de un solo archivo, detener el rastreo del archivo, pero no borrarlo del sistema;
  se utiliza: git rm --cached <nombre-del-archivo>

- Para evitar el rastreo de todos los archivos en .gitignore:
  se ejecuta: git rm -r --cached. Esto elimina los archivos modificados del índice, y luego se ejecuta: git add
  

