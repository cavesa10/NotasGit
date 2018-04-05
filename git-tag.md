### git tag

Lista las etiquetas en orden alfabético.

### git tag -a nombre_etiqueta - "Mensaje de la etiqueta"
Etiqueta anotada. Se guarda en la base de datos de Git como un objeto entero. Tiene un checksum; contiene el nombre del etiquetador, correo electrónico y fecha; y tienen un mensaje asociado.

### git tag -l [patro o filtro]

```
git tag -l "v1.*"
```
Lista las etiquetas que coinciden con el patrón especificado.