# Marcador de Juegos de Mesa (PWA)

Aplicación web instalable para **Chinchón**, **Kharma**, **Los Cuadraditos** y **La Cuenta**.

## Publicar en GitHub + Netlify

Repositorio previsto: `MarcadoreJuegos`.

1. Descomprime el ZIP.
2. En GitHub abre el repositorio `MarcadoreJuegos`.
3. Usa **Add file > Upload files** y sube **el contenido de esta carpeta**, no el ZIP.
4. Confirma los cambios con **Commit changes**.
5. Netlify, al estar conectado con el repositorio, publicará automáticamente la nueva versión.

No hace falta comando de build. `netlify.toml` publica la raíz del repositorio.

## Instalar/actualizar en iPad

1. Abre la URL principal de Netlify en Safari.
2. Recarga la página para obtener la nueva versión.
3. Si ya la tienes añadida a la pantalla de inicio, ciérrala por completo y vuelve a abrirla.
4. El service worker usa la caché `v7` y permite abrir la aplicación sin conexión después de una carga correcta.

## La Cuenta — versión v7

- De 3 a 8 jugadores.
- Ahorros iniciales automáticos: 900 € con 3 jugadores y +100 € por cada jugador adicional.
- Para registrar una cuenta solo se indica quién paga, el importe y si fue obligada o voluntaria.
- El saldo nunca baja de 0 €.
- Cuando un jugador llega a **0 €**, queda **eliminado** y deja de aparecer como posible pagador de nuevas cuentas.
- La partida continúa mientras haya más de 3 jugadores activos.
- Cuando una eliminación deja **3 jugadores activos o menos**, la partida se cierra automáticamente.
- Entre los jugadores que siguen activos, gana quien conserve más ahorros; se contemplan empates.
- En una partida que comenzó con solo 3 jugadores, la primera eliminación cierra la partida.
- La clasificación, el contador de jugadores activos y el historial muestran las eliminaciones.
- **Nueva partida** conserva los jugadores y restaura los ahorros iniciales.

## Datos

Las partidas se guardan en el almacenamiento local del navegador/dispositivo. No se envían a GitHub ni a Netlify.
