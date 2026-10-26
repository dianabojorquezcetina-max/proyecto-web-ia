# Portal Interdimensional

Aplicación web para consultar personajes de Rick and Morty. La información se obtiene de una API pública y se puede explorar con búsqueda, filtros y favoritos.

## Integrantes

- Diana Guadalupe Bojórquez Cetina
- Genny Diudone Navarrete Aguilar

## Enlaces

- Repositorio: https://github.com/dianabojorquezcetina-max/proyecto-web-ia
- Aplicación: https://dianabojorquezcetina-max.github.io/proyecto-web-ia/

## Cómo usar la aplicación

1. Abre el enlace de GitHub Pages.
2. Espera a que carguen los personajes desde la API.
3. Busca por nombre o utiliza los filtros disponibles.
4. Pulsa «Cargar más» para consultar más personajes.
5. Guarda personajes en favoritos y abre esa sección para verlos. Los favoritos se conservan en el navegador.

## Cómo está hecha

La página utiliza HTML para organizar el contenido, CSS para presentarlo y adaptarlo a distintos tamaños de pantalla, y JavaScript para consultar la API y controlar la búsqueda, los filtros y los favoritos. La consulta se realiza con fetch(). Los favoritos se guardan en localStorage.

## Uso de inteligencia artificial

Se utilizó ChatGPT como apoyo para proponer código, aclarar funciones y corregir detalles. El código se revisó y se ajustó desde el editor web de GitHub.

### Prompts utilizados

- «Crea una página web que consulte personajes de Rick and Morty API y muestre su nombre, imagen, estado y especie».
- «Agrega búsqueda por nombre, filtros por estado y especie y una opción para cargar más personajes».
- «Ayúdame a guardar personajes favoritos en localStorage y a mostrarlos en una sección propia».

### Respuesta que se corrigió

Una propuesta inicial no coincidía del todo con los nombres de los archivos y los controles del proyecto. Se adaptó el código a index.html, style.css y script.js, y se revisó que los botones llamaran a las funciones correspondientes.

### Error y solución

La consulta a la API puede fallar si no hay conexión o el servicio no responde. Se agregó manejo de errores para mostrar un aviso en la página en lugar de dejar la sección sin explicación.

### Modificación adicional

Se añadió la opción de ordenar los personajes alfabéticamente. El botón activa o desactiva ese orden para que sea más fácil recorrer los resultados.

## Reflexión personal

Borrador para que Diana lo revise y ajuste a su experiencia antes de entregar:

Durante esta actividad entendí mejor cómo se complementan HTML, CSS y JavaScript para crear una página interactiva. Aprendí que fetch() sirve para solicitar información a una API y que también hay que considerar qué mostrar si la consulta falla. Usé la IA para obtener ideas y aclarar algunas partes, pero tuve que revisar sus respuestas y adaptar el código a lo que necesitaba el proyecto. También comprendí mejor cómo funcionan la búsqueda, los filtros y el guardado de favoritos. Para mejorar la página, probaría más búsquedas y revisaría su uso con teclado.

## Trabajo en GitHub

El repositorio contiene los archivos del proyecto, los Issues y un Pull Request integrado. El historial de commits permite revisar los cambios guardados. En el historial actual, los commits aparecen bajo la cuenta de Diana; por eso, no se atribuyen cambios de código a Genny que no figuren allí.

## Presentación en clase

En la demostración se puede mostrar la carga de personajes, la búsqueda, los filtros, los favoritos y la opción de ordenar. Todas las integrantes deben poder explicar cómo se consulta la API, qué hacen HTML, CSS y JavaScript, qué ocurre si la consulta falla y cómo se publicó el sitio en GitHub Pages.
