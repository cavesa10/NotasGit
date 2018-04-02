### git log
Muestra todo el historial de commits del repositorio

`git log --pretty=format:"%h - %an, %ar : %s"`

Muestra el historial con el formato que indicamos.
#### Limitar la salida del historial

`git log -h`: Cambiamos la n por cualquieres numero entero, por ejemplo: `git log-2` nos mostrara los 2 commits mas recientes.

`git log --after="2016-04-07 00:00:00"`: muestra los commits realizados despues de la fecha especificada