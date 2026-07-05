# Cómo publicar Delta Phi Terra en deltaphi.es

Todo el sitio está en un único bloque de código, sin dependencias externas
(las imágenes van incrustadas). Solo hace falta copiar y pegar.

## 1. Crear la página

1. Entra en `deltaphi.es/wp-admin`.
2. Ve a **Páginas → Añadir nueva**.
3. Como título pon `Delta Phi Terra`.
4. En el editor, borra el bloque de párrafo vacío que aparece por defecto.
5. Pulsa el botón **+** para añadir un bloque nuevo, escribe `HTML
   personalizado` en el buscador y selecciónalo (en inglés: "Custom HTML").
6. Abre el archivo `wordpress-embed.html` de este proyecto, copia **todo**
   su contenido y pégalo dentro de ese bloque.
7. Arriba a la derecha, usa la pestaña **Vista previa** del propio bloque
   (o el botón "Vista previa" de la página) para comprobar que se ve bien.
8. Pulsa **Publicar**.

Ese archivo (`wordpress-embed.html`) ya lleva las imágenes del logo
incrustadas en el propio código — no hace falta subir nada a la Biblioteca
de medios ni enlazar archivos sueltos.

## 2. Enlazarla en el menú

**Apariencia → Menús** → añade la página "Delta Phi Terra" al menú principal
(o donde prefieras que aparezca).

## 3. Favicon (icono de la pestaña del navegador)

En `assets/favicon-512.png` tienes el monograma ΔΦ listo para usar como
icono del sitio: **Ajustes → General → Icono del sitio** → subir esa imagen.
Esto aplica a todo `deltaphi.es`, no solo a esta página — coméntamelo si
prefieres dejarlo solo para esta sección.

## 4. Editar textos más adelante (sin ayuda)

El contenido vive dentro de ese mismo bloque de HTML personalizado. Para
cambiar un texto:

1. Entra a editar la página (**Páginas → Delta Phi Terra → Editar**).
2. Haz clic dentro del bloque de HTML personalizado.
3. Busca el texto que quieres cambiar (con Ctrl+F si lo ves largo) y
   edítalo directamente — es texto normal entre etiquetas, por ejemplo:

   ```html
   <h1>Recuperamos fincas agrícolas y regeneramos el suelo mediterráneo.</h1>
   ```

   Puedes cambiar cualquier frase entre `>` y `<` sin miedo a romper nada,
   mientras no borres las propias etiquetas (`<...>`).
4. Actualiza/publica la página.

Para cambios más grandes (nuevas secciones, fotos reales de las fincas,
reordenar bloques), lo más simple es que me pidas el cambio y te devuelvo
el bloque de HTML actualizado para que sustituyas el anterior.

## 5. Sustituir las fotos de ejemplo

La sección "Fincas en recuperación" tiene tres recuadros de marcador de
posición (con el texto "Foto finca...", etc.). Cuando tengas fotografías
reales, dime y te preparo esa sección con las imágenes reales incrustadas
igual que el logo.
