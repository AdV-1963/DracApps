# Cómo publicar Delta Phi Terra en deltaphi.es

Todo el sitio está en bloques de código autocontenidos, sin dependencias
externas (imágenes y tipografía van incrustadas). Solo hace falta copiar y
pegar. Hay tres versiones: castellano, inglés y catalán.

| Idioma | Archivo |
|---|---|
| Castellano | `wordpress-embed.html` |
| Inglés | `wordpress-embed-en.html` |
| Català | `wordpress-embed-ca.html` |

## 1. Crear las tres páginas

Repite esto tres veces, una por idioma:

1. Entra en `deltaphi.es/wp-admin`.
2. Ve a **Páginas → Añadir nueva**.
3. Como título pon `Delta Phi Terra` (o `Delta Phi Terra — EN` / `— CA` para
   distinguirlas en el listado de páginas; el título no sale en el diseño).
4. En el editor, borra el bloque de párrafo vacío que aparece por defecto.
5. Pulsa el botón **+** para añadir un bloque nuevo, escribe `HTML
   personalizado` en el buscador y selecciónalo (en inglés: "Custom HTML").
6. Abre el archivo correspondiente de la tabla de arriba, copia **todo** su
   contenido y pégalo dentro de ese bloque.
7. Pulsa **Publicar** y anota la URL final que le da WordPress a cada página
   (la verás en la barra de direcciones o en "Ver página").

## 2. Enlazar el selector de idioma (ES / EN / CA)

Cada versión tiene arriba a la derecha un selector "ES / EN / CA". Tal como
están los archivos, esos enlaces apuntan a `index.html`, `index-en.html` e
`index-ca.html` — nombres de archivo que solo funcionan si abres los HTML
en tu ordenador, **no** las URLs reales de WordPress. Hay que corregirlos
una vez publicadas las tres páginas y sepas sus URLs finales:

1. Edita la página en castellano → abre el bloque de HTML personalizado.
2. Busca (Ctrl+F) las tres apariciones de `index.html`, `index-en.html` y
   `index-ca.html` (están juntas, en la barra de navegación superior) y
   sustitúyelas por las URLs reales, por ejemplo:

   ```html
   <a href="/delta-phi-terra/">ES</a><span>/</span>
   <a href="/en/delta-phi-terra/">EN</a><span>/</span>
   <a href="/ca/delta-phi-terra/">CA</a>
   ```
3. Repite lo mismo en las páginas EN y CA (el bloque de navegación es
   idéntico en las tres, solo cambia qué idioma aparece resaltado).
4. Actualiza/publica cada página.

Dímelo si quieres y te devuelvo los tres archivos ya con las URLs
definitivas puestas, en cuanto sepas cómo vas a organizar las rutas
(por ejemplo `/terra/`, `/en/terra/`, `/ca/terra/`).

## 3. Enlazarlas en el menú

**Apariencia → Menús** → añade las páginas que quieras al menú principal
(normalmente solo la versión en castellano; el selector de idioma ya
permite saltar a las otras dos desde dentro de la página).

## 4. Favicon (icono de la pestaña del navegador)

En `assets/favicon-512.png` tienes el monograma ΔΦ listo para usar como
icono del sitio: **Ajustes → General → Icono del sitio** → subir esa imagen.
Esto aplica a todo `deltaphi.es`, no solo a esta página — coméntamelo si
prefieres dejarlo solo para esta sección.

## 5. Editar textos más adelante (sin ayuda)

El contenido vive dentro de ese mismo bloque de HTML personalizado. Para
cambiar un texto:

1. Entra a editar la página (**Páginas → [la que sea] → Editar**).
2. Haz clic dentro del bloque de HTML personalizado.
3. Busca el texto que quieres cambiar (con Ctrl+F si lo ves largo) y
   edítalo directamente — es texto normal entre etiquetas, por ejemplo:

   ```html
   <h1>Pequeños campos, nueva vida.</h1>
   ```

   Puedes cambiar cualquier frase entre `>` y `<` sin miedo a romper nada,
   mientras no borres las propias etiquetas (`<...>`). Recuerda que si
   cambias un texto en una versión, normalmente querrás cambiar también su
   equivalente en las otras dos páginas de idioma.
4. Actualiza/publica la página.

Para cambios más grandes (nuevas secciones, más fotos, reordenar bloques),
lo más simple es que me pidas el cambio y te devuelvo los bloques
actualizados (en los tres idiomas) para que sustituyas los anteriores.

## 6. Añadir más fotos a la galería

La sección "El entorno" ya tiene fotos reales tuyas. Si me pasas más, te
preparo esa sección ampliada o renovada con las imágenes nuevas incrustadas,
igual que las actuales.
