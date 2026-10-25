# NEON RIDERS — Duelo online de motos

Juego de carreras para dos personas desde dos dispositivos distintos.

## Tecnologías
- HTML, CSS y JavaScript
- Canvas 2D para la pista en perspectiva, motos, obstáculos y HUD
- Supabase Realtime Broadcast para sincronizar jugadores
- Vercel para publicar la web estática

## Cómo jugar
1. En el primer dispositivo pulsa Crear sala nueva.
2. Comparte el código con el segundo jugador.
3. El segundo jugador abre la misma página, escribe el código y pulsa Unirse.
4. El jugador 1 inicia la carrera.
5. Jugador 1: W acelera y A/D giran. Jugador 2: flecha arriba acelera y flechas izquierda/derecha giran.
6. Gana quien complete tres vueltas.

## Configuración
La URL de Supabase y una clave publicable están en index.html. La app usa canales públicos de Realtime y no requiere tablas SQL para este prototipo. No pongas claves secretas ni service_role en el navegador.

## Publicar
El proyecto es estático y tiene index.html en la raíz. Importa Jhonn16ax/proyecto-2 en Vercel, deja el directorio raíz en ./ y usa la configuración estática predeterminada.

## Limitaciones
La carretera es una simulación visual 2D con perspectiva, no un motor 3D real. Los canales públicos son apropiados para una demostración de clase, no para un juego competitivo de producción; faltan autenticación y validación del estado en servidor.