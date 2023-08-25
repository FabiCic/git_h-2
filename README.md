# git_h-2
<h2> H-2 (ENVIAR UN DIRECTORIO VACIO AL REPOSITORIO REMOTO) 👀👀👀 </h2>

1.Crear un nuevo repositorio en github nombre: git_h-2

2.Crear un repositorio local

>git init

3.Registrar el repositorio remoto con tú repositorio local

>git remote add origin (pegar_la_ruta_del_repositorio_local)

4.Verificamos la ruta remota

>git remote -v

5.Crear 1 carpeta ó directorio con el nombre de "usuarios" esto crea directamente el directorio

>mkdir usuarios

6.Verificar la creación del directorio

>ls -l

7.Ahora si haces un status del stage

>git status

<h3> NOTA IMPORTANTE </h3>
La carpeta no aparece en el stage, es decir la vez creada, pero en git es como que no la reconoce, esto es debido a que git no hace seguimiento a directorios vacios.

En este momento es necesario elaborar un archivo interno en el directorio "usuarios", pero si por los momentos no queremos agregar nada en ella, pero si tenerla en nuestro repositorio debemos crear un archivo oculto dentro del directorio.

>cd usuarios

>touch .gitkeep

>cd ..

>ls -l

8.Examinamos el stage y debemos ver la carpeta ó directorio usuarios disponible para el tracking

>git status

9.Agregamos el directorio al stage

>git add .

10.Se realiza el commit

>git commit -m "feat: add directory usuarios"

11.Verificamos el commit

>git log --oneline

12.Hacer push

>git push -u origin master

13.Toca ir al repositorio remoto y ver la carpeta en nuestro repositorio
