# isla-andrew
Feliz cumpleaños Andrewww

Una islita 3D para celebrar el cumpleaños de Andrew. Cada amigo entra con su muñequito, pasea por la isla, acaricia gatitos y perritos, sopla las velas del pastel, suelta farolitos, habla con los demás y le deja mensajes.

**Enlace:** https://lauren-dayanna-villanueva-camero.github.io/isla-andrew/

## Cómo está hecha

- Todo vive en `index.html`. El 3D usa Three.js y no hay que instalar nada.
- El multijugador y los mensajes usan Firebase Realtime Database. La dirección de la base está al inicio del script, en `CONFIG.firebaseUrl`. Si está vacía, la página funciona como vista previa para una sola persona.
- `reglas-firebase.json` es una copia de las reglas publicadas en Firebase (pestaña Rules de Realtime Database).
- `preview.png` es la imagen que aparece al compartir el enlace.

## Cambiar textos

Están al inicio del `<script>` de `index.html`:

- `CUMPLE`: el nombre que aparece en el letrero y en los mensajes.
- `FRASES_REGALOS`: las cinco frases de los regalos escondidos. Juntas forman la carta final.
- `MASCOTAS_DEF`: nombres y colores de los gatitos y perritos.

## Moderar mensajes

En la consola de Firebase, dentro de Realtime Database, pestaña Data, carpeta `mensajes`, se puede borrar cualquier mensaje. Desde la página nadie puede editar ni borrar los mensajes de otra persona.
