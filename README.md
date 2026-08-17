# Marcador de Juegos de Mesa (PWA)

Aplicación web instalable para **Chinchón**, **Kharma** y **Los Cuadraditos**.

## Publicar en GitHub + Netlify

Repositorio previsto: `MarcadoreJuegos`.

1. Descomprime el ZIP.
2. En GitHub abre el repositorio `MarcadoreJuegos`.
3. Usa **Add file > Upload files** y sube **el contenido de esta carpeta**, no el ZIP.
4. Confirma los cambios (Commit changes).
5. En Netlify elige **Add new project > Import an existing project**.
6. Selecciona GitHub y el repositorio `MarcadoreJuegos`.
7. No hace falta comando de build. `netlify.toml` indica que la carpeta publicada es la raíz del repositorio.
8. Publica el proyecto.

A partir de ese momento, cada cambio que subas al repositorio podrá desplegarse automáticamente en Netlify.

## Instalar en iPad

1. Abre la URL de Netlify en Safari.
2. Pulsa **Compartir**.
3. Selecciona **Añadir a pantalla de inicio**.
4. Abre el icono del marcador desde la pantalla de inicio.

Después de que la web se haya cargado correctamente al menos una vez, el service worker guarda la aplicación básica para poder abrirla sin conexión.

## Archivos

- `index.html`: aplicación completa.
- `manifest.webmanifest`: información de la app instalable.
- `sw.js`: soporte offline.
- `icon-192.png`, `icon-512.png`, `apple-touch-icon.png`: iconos.
- `netlify.toml`: configuración de despliegue y caché.

## Datos de las partidas

Las partidas se guardan en el almacenamiento local del navegador/dispositivo. No se envían a GitHub ni a Netlify. Si borras los datos de Safari o del sitio, se pueden perder las partidas guardadas.
