\# Práctica de Git y GitHub











\#### Nombre: Arnoldo René Gudiño Ponce



\#### Matrícula: 2630202



\#### Práctica: Creación y sincronización de un repositorio local con GitHub



\## 



\## 



\## Objetivo



Saber cómo usar Git y GitHub para hacer un repositorio local, seguir los cambios con commits y sincronizar los archivos entre un repositorio local y un repositorio remoto en GitHub



\## 



\## Procedimiento







1\. ### Creación del repositorio local



|primero se crea una carpeta|practica-git-arnoldo-gudino|

|-|-|

|se inicializa git|git init|

|luego se estableció la rama principal|git branch -M main|

|creamos dos archivos|README.md y datos.txt|

|revisamos el estado del repositorio cada que queramos|git status|

|agregamos los archivos al área de staging|git add -A|

|hicimos primer commit|git commit -m "Primer commit"|











2\. ### Creación del repositorio en GitHub











|se crea un repositorio en GitHub con el mismo nombre|practica-git-arnoldo-gudino|

|-|-|

|el repositorio se crea vacío|sin README o .gitignore|



\### 



3\. ### Vinculación del repositorio local con GitHub



|Para conectar el repositorio local con GitHub se utilizó|git remote add origin https://github.com/arnoldorgp/practica-git-arnoldo-gudino.git|

|-|-|

|Después se verificó la conexión|git remote -v|

|se enviaron los archivos del repositorio local a GitHub|git push -u origin main|



\### 



4\. ### Sincronización Local --> GitHub







Se modificó el archivo datos.txt desde el repositorio local escribiendo: Este archivo fue modificado desde el repositorio local.



Después se usaron:



\* git status

\* git add .

\* git commit -m "Actualización desde repositorio local"

\* git push



El cambio se envió correctamente a GitHub.







5\. ### Sincronización GitHub --> Local







Se modificó datos.txt en GitHub escribiendo: Este archivo fue modificado desde GitHub.



Después se usó: git pull origin main



Este comando descargó el cambio de GitHub y lo agregó al repositorio local.



El flujo fue: GitHub --> Commit --> git pull --> Repositorio local











6\. ### Sincronización final







Al terminar se ejecutó: git status



La respuesta de la terminal fue: Your branch is up to date with 'origin/main'.

nothing to commit, working tree clean



Esto significa que el repositorio local y GitHub están sincronizados.







\## Comandos utilizados



|git init| Inicializa un repositorio de Git en la carpeta que estemos|

|-|-|

|git branch -M main| Cambia el nombre de la rama actual a main|

|git status|muestra el estado actual del repositorio|

|git add -A| Agrega todos los archivos que estaban en untrackefiles a la zona de staging|

|git commit -m ""| Crea un commit|

|git remote add origin URL| Conecta repositorio local con repositorio remoto|

|git remote -v| Muestra las URL de los repositorios remotos configurados|

|git push| Envía los cambios del repositorio local a GitHub|

|git push -u origin main| Envía la rama main a GitHub y establece su seguimiento remoto|

|git pull origin main| Aplica los cambios de GitHub al repositorio local|



\## Archivos utilizados







README.md: Contiene la información y documentación de la práctica.



datos.txt: Se utilizó para comprobar la sincronización de cambios entre GitHub y el repositorio local.







\## Conclusión



con esta practica aprendí a sincronizar un repositorio local con uno remoto y como trabajar con los archivos dentro de este repositorio, poder modificarlos tanto de forma local así como en la nube y como guardar los cambios en ambos lados





