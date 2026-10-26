# Portal Interdimensional — proyecto-web-ia

Explorador interactivo de personajes de Rick and Morty. Consulta datos reales de la API pública y permite buscar, filtrar, ordenar y guardar favoritos.

## Integrantes

- Diana Guadalupe Bojórquez Cetina
- Agregar aquí los nombres de los demás integrantes del equipo, si aplica.

## Aplicación

- Repositorio: https://github.com/dianabojorquezcetina-max/proyecto-web-ia
- GitHub Pages: https://dianabojorquezcetina-max.github.io/proyecto-web-ia/ (activar Pages en Settings → Pages para publicar)

## Uso

1. Abre la aplicación publicada o sirve los archivos con un servidor web estático.
2. La página consulta personajes en Rick and Morty API al cargar.
3. Escribe un nombre para buscar; usa los filtros de estado y especie para acotar resultados.
4. Selecciona Cargar más personajes para recorrer las páginas siguientes.
5. Usa el corazón para guardar o quitar favoritos. Se conservan en el almacenamiento local del navegador.
6. Usa A–Z para ordenar y el botón Modo para alternar entre tema oscuro y claro.

## Tecnologías y funcionamiento

- HTML define las secciones y controles accesibles de la página.
- CSS crea el diseño adaptable y los temas de color.
- JavaScript consulta la API Rick and Morty con fetch(), procesa el JSON, filtra resultados y actualiza la interfaz.
- localStorage guarda favoritos y la preferencia de tema en el dispositivo actual.
- Si la API falla o no encuentra coincidencias, la aplicación muestra un mensaje en pantalla.

## Prompts importantes usados

1. «Analiza los requisitos de la tarea y conviértelos en una aplicación web de personajes que consuma Rick and Morty API.»
2. «Implementa búsqueda, filtros de estado y especie, paginación y favoritos persistidos con localStorage.»
3. «Añade una funcionalidad extra que podamos explicar: modo claro/oscuro y orden alfabético; mantén el diseño adaptable.»

## Respuesta de IA que requirió correcciones

La primera propuesta de JavaScript usaba plantillas literales dentro del contenido que se pegaba en el editor. Al preparar el texto para GitHub, las comillas invertidas entraron en conflicto con el formato de entrada y el código no se pudo insertar. Se corrigió usando concatenación de cadenas en la plantilla de las tarjetas, y se verificó que el contenido apareciera en el editor antes de guardarlo.

## Error y resolución

La API devuelve una respuesta HTTP de error cuando una búsqueda no tiene coincidencias. La consulta comprueba response.ok, captura el error y presenta un mensaje de búsqueda sin resultados o de conexión fallida; el usuario puede cambiar el término o limpiar los filtros.

## Modificación extra que podemos explicar

Se agregó el orden alfabético como reto adicional. El botón alterna el orden ascendente y descendente del arreglo visible con localeCompare() en español; render() vuelve a dibujar las tarjetas sin cambiar los datos de la API. También se añadió el cambio de tema, que guarda la preferencia en localStorage.

## Reflexión del equipo

Completar después de probar y conversar en equipo: escriban qué aprendieron al usar IA, qué partes verificaron por su cuenta y qué cambiarían en una siguiente versión. Cada integrante debe poder explicar cómo fetch(), los filtros y localStorage funcionan.

## Trabajo colaborativo y presentación

Para completar la consigna del curso, el equipo debe documentar aquí las contribuciones de cada integrante y realizar los Issues, commits y Pull Request de acuerdo con el proceso solicitado. Presenten el funcionamiento y expliquen qué código generó la IA y qué ajustes hizo el equipo.

## Fuente de datos

[The Rick and Morty API](https://rickandmortyapi.com/documentation)


## Guía rápida para la presentación

- fetch() solicita los datos a una URL; response.json() convierte la respuesta para que JavaScript pueda recorrerla.
- HTML organiza el contenido, CSS controla su apariencia y JavaScript responde a las acciones y procesa los datos.
- El buscador espera 350 ms después de escribir y consulta el endpoint de búsqueda por nombre.
- Si la API responde con error o falla la conexión, catch muestra un mensaje para que la persona pueda reintentar.
- Los favoritos se serializan en JSON dentro de localStorage y se recuperan al cargar la página.
- GitHub Pages publica los archivos estáticos desde la rama main y la carpeta raíz.

Esta guía acompaña la demostración; cada integrante debe explicar con sus propias palabras los cambios que revisó.
