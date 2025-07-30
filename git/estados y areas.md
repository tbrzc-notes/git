# Estados principales en los que se puede encontrar un archivo
- **modified**: cualquier archivo modificado que no haya sido commited
- **staged**: area de preparacion, marca los archivos modificados en su version actual para que sean guardados en la db de git
- **commited**: significa que la informacion fue guardada correctamente en la base de datos local
- **tracked**: todos aquellos archivos, que son la instantanea mas reciente, pueden ser archivos modificados o no, o preparados
- **untracked-files**: cualquier archivo que no esta en la ultima instantanea y que no esta en el area de preparacion (al clonar todos los archivos estaran rastreados pues no se han modificado)
## Secciones principales de un proyecto en git
- <mark style="background: #CACFD9A6;">git directory</mark>: se almacenan los metadatos y la base de datos de objetos, es lo que se copia cuando se clona un repo
- <mark style="background: #FF5582A6;">working directory</mark>: es una copia de una version del projecto, los archivos se sacan de la base de datos comprimida en el directorio .git
- <mark style="background: #ADCCFFA6;">staging area</mark>: se encuentra en el directorio .git

![[Pasted image 20240518131119.webp|543x309]]