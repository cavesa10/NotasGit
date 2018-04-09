# Aprendiendo a usar Git desde Cero
Sistemas de control de versiones para el mantenimiento eficiente y confiable de archivos.

## Zonas de Git
1. Directorio de trabajo
2. Área de preparación
3. Directorio Git

## Flujo de trabajo básico en GIT
1. Modificas una serie de archivos en tu directorio de trabajo.
2. Preparas los archivos, añadiendolos a tu área de preparación.
3. Confirmas los cambios, lo que toma los archivos tal y como están en el área de preparación y almacena esa copia instantánea de manera permanente en tu directorio de Git.

## Configurando Git por primera vez
```
git config --global user.name "Carlos Vesga"
git config --global user.email cavesa10@gmail.com
git config --global core.editor Code
git config --list
```

## Configuración SSH en Windows
Usando git bash seguimos los siguientes pasos:

1. Creamos  una carpeta llamada "llaves-ssh" en el disco "C" para evitar problemas de rutas.
2. Ejecutamos el comando `ssh-keygen -t rsa -C "cavesa10@gmail.com"` El correo debe ser el mismo con el que nos registramos en Github para evitar posibles problemas. Dejamos el passphrase vacion y damos enter. Cuando nos pida la ruta escribimos `/c/llaves-ssh/github_rsa`.
3. Iniciamos ssh-agent en backgraound ejecutando el comando ´eval "$(ssh-agent -s)"´.
4. Agregamos la llave ssh generada a ssh-agent ejecutando el comando `ssh-add /c/llaves-ssh/github_rsa`.
5. Desde ahora podemos hacer pull y push sin autenticacion.
