# FILTRO WEB v1.0.1
Es un filtro que nos permite buscar en un listado por cadena de texto o filtrando su tipo de archivo.

## RECOMENDACIONES -- USUARIOS SIN CONOCIMIENTO JAVASCRIPT
Si no conoces sobre desarrollo en Javascript te recomiendo utilizar el archivo que está dentro de la carpeta compressed.

Para utilizarlo necesitaras en tu documento HTML los siguientes elementos:
- Un DIV con ID = "publicaciones", que contendrá solo los enlaces a los archivos (sólo elementos a)
		Este DIV no deberá ser visible en el documento (ya que es el que contiene todos los enlaces)

```diff
- Se ha encontrado un error: si se diseña sobre HTML y no está minificado (es decir, contiene espacios y saltos de linea) el plugin no funciona como debería, se recomienda que en este DIV no haya espacios ni saltos de linea.
```

- Un DIV con ID = "listado", es el que se actualizará constantemente con el filtro.
	Puede estar vacío o no, de igual manera se limpia al cargar la página y se colocan todos los elementos de #publicaciones.

- La cantidad de CheckBox que sea necesaria en tu proyecto, deben incluir la CLASE ".input__filtro" y el ID debe ser exactamente el tipo de archivo que se quiere filtrar, por ejemplo "mp3, doc, pdf".

- Un elemento 'a' con el ID = "btn_filtrar", simulará ser un boton de filtrado.

- El tipo de datos de cada archivo se especifica en cada elemento 'a' de #publicaciones, con el atributo 'data-type', por ejemplo &lt;a href="archivos/archivo.extension" data-type="extension">Texto a Mostrar&lt;/a>.
	Este tipo de datos es el que se filtra, y se filtra de acuerdo al ID de los checkbox.

- Un INPUT de tipo texto con el ID = "text_filter", se va a encargar de buscar sobre el texto de la etiqueta de enlace.

## USUARIOS CON CONOCIMIENTO EN JAVASCRIPT
Dentro de la carpeta dev se encuentra el archivo desarrollado por mí, está creado para que puedan modificar el nombre de las variables utilizadas, por si en algún caso los nombres colocados por defecto impactan sobre su proyecto.

### VISITA NUESTRA WEB
http://basicsproject.tk/

### SOPORTE y CONSULTAS
Se reciben mails sólo con asunto sobre reportes de mal funcionamiento de mi contenido en: basicswebproject@gmail.com