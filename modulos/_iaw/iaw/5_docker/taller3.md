---
title: "Taller 3: Creación de imágenes Docker"
---

Para la realización de este taller es necesario tener una cuenta en Docker Hub.

## Creación de una imagen a partir de un Dockerfile 

1. Crea una página web estática (por ejemplo busca una plantilla HTML5). O simplemente crea un `index.html`.
2. Crea un fichero `Dockerfile` que permita crear una imagen con un servidor web sirviendo la página. Puedes usar una imagen base debian o ubuntu, o una imagen que tenga ya un servicio web, como hemos visto en el apartado [**Ejemplo 1: Construcción de imágenes con una página estática**](https://github.com/josedom24/curso_docker_ies/blob/main/modulo5/ejemplo1.md).
3. Ejecuta el comando docker que crea la nueva imagen. La imagen se debe llamar `<tu_usuario_docker_hub>/mi_servidor_web:v1`.
4. Conéctate a Docker Hub y sube la imagen que acabas de crear.
5. Descarga la imagen en otro ordenador donde tengas docker instalado, y crea un contenedor a partir de ella. (Si no tienes otro ordenador con docker instalado, borra la imagen en tu ordenador y bájala de Docker Hub).
6. Vamos a hacer una modificación de la página web: haz una modificación al fichero `index.html`.
7. Vuelve a crear una nueva imagen, en esta caso pon ta etiqueta `v2`. Súbela a Docker Hub.
8. Por último, baja la nueva imagen en el ordenador donde está corriendo el contenedor. Para hacer la implantación de la nueva versión debes borrar el contenedor y crear uno nuevo desde la nueva versión de la imagen.

{% capture notice-text %}
## ¿Qué tienes que entregar?

1. Pantallazo donde se vea el contenido del fichero Dockerfile.
2. Pantallazo donde se vea el comando que crea la nueva imagen.
3. Pantallazo donde se vea el acceso a la página web primera versión.
4. Pantallazo donde se vean las dos imágenes subidas a tu cuenta de Docker Hub.
5. Pantallazo donde se vea el acceso a la página web segunda versión.

{% endcapture %}<div class="notice--info">{{ notice-text | markdownify }}</div>
