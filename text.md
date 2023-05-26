En el caso de queramos resetear todo, borramos la carpeta .git que está oculta en la carpeta raiz del proyecto de React (Este paso es solo si tenemos problemas)
Ahora comenzamos con git init que inicializa todo lo referente a git en nuestro proyecto
Luego se agrega todo los archivos de seguimiento al stage, o lugar intermedio para poder hacer commit, con el git add .  o si se quiere agregar solo ciertos archivos agregamos los archivo que queramos
Luego hace el commit de nuestros elementos del stage con git commit -m 'nombre del commit'
Finalmente deseamos vincular nuestro proyecto a un repositorio de github, por lo que, tenemos que crear un nuevo repositorio o buscar uno creado que no esté vinculado a ningún otro proyecto.
Para vincular, se tienen los siguiente pasos
git remote add origin https://github.com/{cuenta_de_github}/{nombre_del_repositorio}.git  Esto nos sirve para vincular nuestro proyecto al repositorio
git branch -M main  esto nos sirve para cambiar el nombre de nuestra rama actual a main
git push -u origin main  esto nos sirve para subir la rama main al repositorio
Listo, ya esta todo listo
Como actualizar la información de una repositorio ya existente
En caso de estar en otra computadora tenemos que clonar el repositorio con git clone {url del repositorio}
En caso de estar trabajando con otro compañeros o programador, antes de hacer algún cambio, debemos traernos la información nueva a nuestro proyecto en local con git pull
Ahora lo que hacemos son los cambios que necesitamos en nuestro proyecto
Luego, como ya está vinculado nuestro proyecto al repositorio simplemente hacemos los pasos 3, 4 de la parte “Como subir un proyecto….”
Y luego simplemente hacemos, git push , automáticamente se suben los cambios
En caso de tener mas ramas y queremos subir esa rama, entonces tenemos que indicar git push -u origin {nombre de la rama}