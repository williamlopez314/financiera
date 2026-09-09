# Rumbo a la U

Juego educativo de finanzas personales para estudiantes de 4° medio. Simula el primer año universitario (independencia, arriendo, movilización, imprevistos, créditos, ahorro, AFP/APV) en 6 rondas, jugable hasta con 4 personas desde computadores distintos, sincronizado con Firebase Realtime Database.

## Publicar en GitHub Pages

1. Crea un repositorio nuevo en GitHub (puede ser público).
2. Sube el archivo `index.html` a la raíz del repositorio (arrastrar y soltar en la web de GitHub funciona).
3. Ve a **Settings → Pages**.
4. En "Source" elige la rama `main` y la carpeta `/ (root)`, luego guarda.
5. En 1-2 minutos, GitHub te dará un link tipo `https://tu-usuario.github.io/tu-repositorio/`. Ese es el link para compartir con los estudiantes.

## Cómo se juega

1. Un/a estudiante crea una sala (recibe un código de 4 dígitos) y lo comparte con su grupo.
2. Hasta 3 personas más se unen escribiendo ese código y su nombre, cada una desde su propio computador.
3. El anfitrión/a inicia la partida cuando estén todos listos.
4. Cada jugador/a elige su arriendo, movilización e ingreso inicial (mes 0).
5. Se juegan 6 meses por turnos: cada jugador enfrenta el mismo evento del mes con sus propios números, y decide.
6. Al final se muestra un ranking con salud financiera, ahorro, deuda y un tip personalizado para cada uno/a.

Duración estimada con 4 jugadores: 25-30 minutos.

## Nota sobre los datos

La partida usa una base de datos en modo de prueba (abierta por 30 días desde su creación). Si planeas usar el juego después de esa fecha, entra a la consola de Firebase → Realtime Database → Reglas, y extiende la fecha de expiración o cambia las reglas a `".read": true, ".write": true` de forma permanente.
