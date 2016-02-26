# hackatones

## Instalación
Para una instalación fácil, deberás tener presente ciertos requerimientos y comandos, para ello consulta `http://jekyllrb.com/docs/quickstart/`

Antes de subir tu sitio, realiza los cambios necesarios en `_config.yml`

1. Si estás almacenando tu sitio en GitHub tu `url` debería ser `http://nombre-de-usuario.github.io` si necesitas información al respecto consulta `https://pages.github.com/`

2. En `baseurl` se encuentra la sub-ruta para tu sitio. Si el repositorio se llama `hackatones`, este debería estar en `/hackatones`

3. En `tracking_id` puedes establecer tu identificador para google analytics. Para que funciones esta variable debe estár definida como `true`

## Uso

- Para hacer funcionar el servidor debes utilizar la línea `jekyll server --baseurl`

- La información para la página de inicio se puede modificar en `_data` y en `_config.yml`
  Para cambiar el texto al inicio del proyecto: `Título para el hackatón`, deberás cambiar `title:` en `_config.yml`
  En el caso de la sección Objetivo debes ir a `_data/goal.yml`
  Si deseas agregar fechas para la Agenda sólo debes seguir el formato en `_data/agenda/agenda.yml`
  Para el mapa, sólo necesitas cambiar el iframe que te proporciona google maps en `_data/map.yml` o incluir la estructura similar de otro servicio
  Para agregar jueces debes incluir las imágenes en `/img/judges` y cambiar la información tendrás que ir a `_data/judges/judges.yml`
  Los Premios manejan la misma lógica que Agenda, esta información se encuentra en `_data/awards/awards.yml`
  La sección de Resultados está pensada para incluir un texto que describa lo que se logró con el evento en términos cualitativos y cuantitativos, esto se debe cambiar en `_data/results.yml`
  Para Ganadores se usa la misma distribución que en Jueces, imágenes en `/img/winners` e información en `_data/winners/winners.yml`

  Esta tema está pensado para manejar 2 escenarios, uno previo/durante y otro posterior al evento. En `_config.yml`, encontrarás las Variables de contenido, los valores definidos son para el escenario previo. Para el posterior, deberás invertir el valor de éstas variables.

- Para generar un nuevo post, sólo necesitas almacenar el archivo `.markdown` en el directorio `_posts/`

  Te recomendamos guardarlos con el siguiente formato `año-mes-día-Nombre-del-archivo.markdown`

  Las imágenes de los post deben estár en el directorio `/post-images` y el vínculo en el archivo almacenado en `_posts/` debe coincidir

- Este tema esta pensado para manejar una gama cromática específica, si deseas modificar los colores debes ir a `_sass/_site.scss` y ubicar el bloque `// Variables de color para el tema`

- Para cambiar la imagen de fondo que aparece en la página de inicio deberás reemplazar `img/background.jpg`por la que tu desees, las dimensiones de esta son: 1100 x 733 px

- Para generar comentarios en los publicaciones, deberás utilizar Facebook comments.

  Crear una nueva aplicación en `My Apps` para obtener tu número de identificación

## Licencia
MIT. Copyright (c) [Nombre del proveedor ](http://sitiodelproveedor.com)
