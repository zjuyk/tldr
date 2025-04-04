# zip

> Empaqueta y comprime archivos en un archivo Zip.
> Vea también: `unzip`.
> Más información: <https://manned.org/zip>.

- Agrega archivos/directorios a un archivo específico:

`zip {{[-r|--recurse-paths}} {{ruta/a/comprimido.zip}} {{ruta/al/archivo_o_directorio1 ruta/al/archivo_o_directorio2 ...}}`

- Elimina archivos/directorios de un archivo específico:

`zip {{[-d|--delete]}} {{ruta/a/comprimido.zip}} {{ruta/al/archivo_o_directorio1 ruta/al/archivo_o_directorio2 ...}}`

- Archiva archivos/directorios e[x]cluyendo especificados:

`zip {{ruta/a/comprimido.zip}} {{ruta/al/archivo_o_directorio1 ruta/al/archivo_o_directorio2 ...}} {{-x|--exclude}} {{ruta/a/archivos_o_directorios_excluidos}}`

- Archiva archivos/directorios con un nivel de compresión específico (`0` - el más bajo, `9` - el más alto):

`zip {{[-r|--recurse-paths}} -{{0..9}} {{ruta/a/comprimido.zip}} {{ruta/al/archivo_o_directorio1 ruta/al/archivo_o_directorio2 ...}}`

- Crea un archivo cifrado con una contraseña específica:

`zip {{[-r|--recurse-paths}} {{[-e|--encrypt]}} {{ruta/a/comprimido.zip}} {{ruta/al/archivo_o_directorio1 ruta/al/archivo_o_directorio2 ...}}`

- Archivo de archivos/directorios a un archivo multiparte[s] (por ejemplo, en partes de 3 GB):

`zip {{[-r|--recurse-paths}} {{[-s|--split-size]}} {{3g}} {{ruta/a/comprimido.zip}} {{ruta/al/archivo_o_directorio1 ruta/al/archivo_o_directorio2 ...}}`

- Imprime un contenido específico de archivo:

`zip {{[-sf|--split-size --freshen]}} {{ruta/a/comprimido.zip}}`
