# Como recuperar datos con git:

## Proceso de como recuperar todo la informacion de un commit:

1. Primero debemos de identificar que commit queremos cargar. Sería de la siguiente manera para poder hacerlo:
~~~
// Escribirlo en la terminal

git log --oneline
~~~

2. Segundo paso entrar en el commit. Esto se podrá hacerlo con el siguiente comando:
~~~
git checkout (Los caracteres SHA del commit)
~~~

3. Tercer paso: Importante esto solo hace que cargue ese commit en visual recuperando todos los datos de ese commit. Pero hay mas formas de hacerlo segun, la necesidad que se necesite.

~~~
git reset --hard
~~~

> Esto hace que recuperemos todo lo que teniamos en el commit en el que nos enconstramos.

4. Paso extra: si queres borrar un archivo o carpeta del repositorio, pero no de manera local, es de la siguiente manera:

~~~
git rm --cached (mi archivo) // esto es solo con archivos
git rm -r --cached (mi carpeta) // borra la carpeta
~~~

> Y listo esto esto hace que borremos en nuestro repositorio remoto (gitHub) la carpeta o archivo, pero no lo borra en nuestro nivel local.

---

**Fun fact:** si queremos borrarlos en mi repositorio remoto, y en mi area local (osea en visual code), es de la siguiente manera:

~~~
git rm (archivo)

git rm -r (carpeta)
~~~

**Plus Fun fact:** al hacer el ultimo ejemplo de arriba y el penultimo, tenemos que guardarlo en la parte local(add .) y en la de git (commit), despues mandarlo a nuestro repositorio remoto (push).

~~~
git add .

git commit

git push
~~~

