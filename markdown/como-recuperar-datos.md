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
