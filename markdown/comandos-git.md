## Lista de comandos Git:

1. git reset: Esto hace que si tenemos un archivo o carpeta en la area de staged( efectuado, es decir que le hicimos add ), esto hará que quite de esa área al archivo o carpeta. EJEMPLO:

~~~
git status (para que archivos estan en el área de staged)

// reset: lo quitará del area de staged
git reset (nombre del archivo)
~~~


> En resumen el archivo que está en un estado staged, lo pasa al estado unstaged.