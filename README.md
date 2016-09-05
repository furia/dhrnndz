# hackatones

Este proyecto está pensado para ofrecer una opción no difícil de implementar y accesible para gestionar información relacionada a un hackatón o datatón.

La información está distribuida en bloques por lo que cada uno de ellos tiene un archivo independiente que puedes editar para incluir la tuya.

Este tema está pensado para usar dos escenarios: uno antes/durante y uno posterior o al cierre del evento.

El antes/durante, inicia desde que ya se han decidido y logrado concretar los aspectos operativos de un hackatón o datatón. Aquí la información debe ser clara, puntual y se tiene que adelantar a responder a las preguntas más comunes que puedan tener los interesados.

El escenario posterior, comienza a ser útil una vez que el hackatón a llegado a su término. Es ideal hacer saber de manera pública cuáles fueron los logros que se obtuvieron, así como quienes fueron los ganadores.

Hacer el cambio de escenario implica modificar algunos datos.

Cabe mencionar que la apariencia del contenido es responsivo y editable. Funciona utilizando plataformas como [http://jekyllrb.com/](http://jekyllrb.com/) y los servicios de [https://pages.github.com/](https://pages.github.com/), entre otros.

## Instalación

Para tener una copia del tema en tu cuenta de GitHub, debes localizar el botón de `fork` en la esquina superior derecha y darle click.

Si tienes más experiencia, puedes hacer una copia local y gestionarlo desde uno de tus repositorios. Si necesitas información al respecto consulta la documentación en [https://github.com/](https://github.com/) y [http://jekyllrb.com/docs/quickstart/](http://jekyllrb.com/docs/quickstart/).

En caso de usar [https://pages.github.com/](https://pages.github.com/) para publicar tu sitio, deberás cambiar el nombre del repositorio por el nombre que usas como usuario (es ideal que el nombre haga referencia al nombre del hackatón).

Para más información al respecto consulta [https://pages.github.com/](https://pages.github.com/).

## Uso

En caso de usar el tema desde local, se debe utilizar la línea `jekyll server` para correr el servidor.

### Cambiar contenido

No olvides que una vez localizada la sección para editar contenido, el cambio debe ser guardado por medio de cuadro de diálogo Commit changes con la opción Commit directly to the gh-pages branch seleccionada.

La información para la página de inicio se puede modificar en `_data` y en `_config.yml`

Para cambiar el texto al inicio del proyecto: `Título para el hackatón`, deberás cambiar `title:` en `_config.yml`.

Para cambiar la imagen de fondo que aparece en la página de inicio deberás reemplazar `img/background.jpg` por la que tu desees, las dimensiones de esta son: 1100 x 733 px.

En el caso de la sección Objetivo debes ir a `_data/objetivo.yml`.

Si deseas agregar fechas para la Agenda sólo debes seguir el formato en `_data/agenda.yml`

Para el mapa, sólo necesitas cambiar el iframe que te proporciona google maps en `_data/mapa.yml` o incluir la estructura similar de otro servicio

Para agregar jueces debes incluir las imágenes en `/img/jueces` y para cambiar la información tendrás que ir a `_data/jueces.yml`

Para agregar mentores debes incluir las imágenes en `/img/mentores` y para cambiar la información tendrás que ir a `_data/mentores.yml`

Los Premios manejan la misma lógica que Agenda, esta información se encuentra en `_data/premios.yml`

La sección de Resultados está pensada para incluir un texto que describa lo que se logró con el evento en términos cualitativos y cuantitativos, esto se debe cambiar en `_data/resultados.yml`

Para Ganadores se usa la misma distribución que en Jueces, imágenes en `/img/ganadores` e información en `_data/ganadores.yml`

### Agregar publicaciones

Para generar un nueva publicación en la sección de Noticias, sólo necesitas almacenar el archivo `.markdown` en el directorio `_posts/`

Te recomendamos guardarlos con el siguiente formato `año-mes-dia-Nombre-del-archivo.markdown`

Las imágenes de los post deben estár en el directorio `/post-images` y el vínculo en el archivo almacenado en `_posts/` debe coincidir

Este tema esta pensado para manejar una gama cromática específica, si deseas modificar los colores debes ir a `_sass/_site.scss` y ubicar el bloque `// Variables de color para el tema`

Como se mencionó este tema está pensado para manejar 2 escenarios, uno previo/durante y otro posterior al evento. En `_config.yml`, encontrarás las `// Variables de contenido`, los valores definidos son para el escenario previo. Para el posterior, deberás invertir el valor de éstas variables.

### Cambiar escenarios

Como se mencionó el tema está pensado para manejar 2 escenarios, uno previo/durante y otro posterior al evento. En `_config.yml`, se encuentran las `// Variables de contenido`, estos valores definen la visualización de contenido. Para cambiar de un escenario al otro, sólo se debe invertir el valor de las variables, es decir, pasar de true a false y de false a true.

### Cambio de esquema de color

El tema, también están implementado para manejar una gama cromática específica, si deseas modificar los colores debes ir a la carpeta `_sass/_site.scss` y ubicar el bloque `// Variables de color para el tema`.

Los colores están expresados en variables hexadecimales, para elegir colores puedes utilizar http://paletton.com/.

De manera paralela, se incluyen dos opciones que se pueden utilizar, copiando y pegando los hexadecimales de las opciones presentadas en el lugar de las colores del bloque activo.

### Google Analytics

También se puede usar [Google Analytics](https://www.google.com.mx/analytics/) para hacer seguimiento de quién visita el sitio, para ello deberás cambiar en `_config.yml` el `tracking_id` por tu número de idenfiticación del servicio. Para que funciones esta variable debe estár definida como `true`.


### Facebook Comments

Para tener comentarios en los publicaciones, se deberá utilizar Facebook comments.

En caso de no querer utilizarlos se tiene que localizar en `_config.yml` el bloque `# Facebook comments` y cambiar a false la variable `fbcomments`.

Para utilizarlos, es necesario tener validada la cuenta en Facebook (número telefónico) y estar registrado como desarrollador en https://developers.facebook.com/.

Una vez que se tenga lo anterior, se tiene que seleccionar la opción `Agregar una nueva aplicación` dentro de la opción `Mis aplicaciones`, seleccionando como plataforma `Sitio web` para obtener tu número de identificación o `App Id`.

El `App Id` y el `Api version`, deben ser reemplazados en `_config.yml`.

Después, en https://developers.facebook.com/docs/plugins/comments debes agregar en Comments Plugin Code Generator el url que se utilizará para el sitio, por último debes dar click en el botón `Get code`. Sólo necesitas generar el código desde la página para que la información que ya agregaste en `_config.yml` funcione.

## Licencia
MIT. Copyright (c) [Nombre del proveedor ](http://sitiodelproveedor.com)
