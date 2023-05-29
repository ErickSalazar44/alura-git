# alura-git
Lista de cursos para controlar con Git

1) En el caso de queramos resetear todo, borramos la carpeta .git que está oculta en la carpeta raiz del proyecto de React (Este paso es solo si tenemos problemas)
2) Ahora comenzamos con git init que inicializa todo lo referente a git en nuestro proyecto
3) Luego se agrega todo los archivos de seguimiento al stage, o lugar intermedio para poder hacer commit, con el git add .  o si se quiere agregar solo ciertos archivos agregamos los archivo que queramos
4) Luego hace el commit de nuestros elementos del stage con git commit -m 'nombre del commit'
5) Finalmente deseamos vincular nuestro proyecto a un repositorio de github, por lo que, tenemos que crear un nuevo repositorio o buscar uno creado que no esté vinculado a ningún otro proyecto.
6) Para vincular, se tienen los siguiente pasos
  a) git remote add origin https://github.com/{cuenta_de_github}/{nombre_del_repositorio}.git  Esto nos sirve para vincular nuestro proyecto al repositorio
  b) git branch -M main  esto nos sirve para cambiar el nombre de nuestra rama actual a main
  c) git push -u origin main  esto nos sirve para subir la rama main al repositorio
7) Listo, ya esta todo listo

"Como actualizar la información de una repositorio ya existente"
1) En caso de estar en otra computadora tenemos que clonar el repositorio con git clone {url del repositorio}
2) En caso de estar trabajando con otro compañeros o programador, antes de hacer algún cambio, debemos traernos la información nueva a nuestro proyecto en local con git pull
3) Ahora lo que hacemos son los cambios que necesitamos en nuestro proyecto
4) Luego, como ya está vinculado nuestro proyecto al repositorio simplemente hacemos los pasos 3, 4 de la parte “Como subir un proyecto….”
5) Y luego simplemente hacemos, git push , automáticamente se suben los cambios
6) En caso de tener mas ramas y queremos subir esa rama, entonces tenemos que indicar git push -u origin {nombre de la rama}
