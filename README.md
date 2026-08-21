# Crónicas de Éter · Rol por turnos

Juego de rol táctico para navegador. Forma una compañía de tres héroes, elige habilidades y derrota enemigos fantásticos mediante combates por turnos.

## Jugar en línea

La versión publicada está disponible en GitHub Pages:

<https://jhaycoltez512.github.io/juego-rol-turnos/>

También funciona en celulares. Se recomienda usar la pantalla en horizontal.

## Mundos

- **Mundo 1 · Bosque Umbrío:** cinco etapas, con el Ojo que Mastica Estrellas como jefe.
- **Mundo 2 · Mar de Neón:** cinco etapas, con la Reina del Eclipse como jefe.
- **Mundo 3 · Camino del Olimpo:** enemigos de la mitología griega y Zeus como jefe final.

Al completar una etapa, la compañía recupera toda su vida antes de continuar.

## Héroes y combate

Elige tres héroes antes de cada mundo. Cada personaje tiene estadísticas, habilidades y un rol diferente: daño, defensa, control, curación o apoyo.

Durante el turno de un héroe:

1. Selecciona una habilidad.
2. Toca o pulsa un objetivo iluminado.
3. Usa **Defender** para reducir el daño recibido o **Terminar turno** para pasar la iniciativa.

El combate incluye congelación, aturdimiento, provocación, escudos, mejoras de ataque y curación.

## Ejecución local

No requiere dependencias ni compilación. Desde la raíz del repositorio:

```bash
python3 -m http.server 8000
```

Abre <http://localhost:8000/index.html> en el navegador. Para detener el servidor, pulsa `Ctrl + C`.

## Estructura

- `index.html`: interfaz, estilos y lógica completa del juego.
- `AGENTS.md`: guía para colaboradores.

Las mejoras visuales y de jugabilidad se prueban manualmente en escritorio y móvil antes de publicar cambios en la rama `main`.
