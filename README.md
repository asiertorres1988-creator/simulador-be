# Simulador Pista B+E · Marcha atrás en curva

Simulador web para practicar la **maniobra G del examen B+E en España** (marcha atrás en recta y curva, la "L"): bordillo en un lado, línea en el otro, 10 m de recta antes y después de la curva.

Está modelado con un **BMW X5 E70** y un **remolque de doble eje** con toldo, y la física es la cinemática real del conjunto coche + remolque: el remolque solo obedece a la bola de enganche, sin ayudas escondidas. Lo importante es entender y automatizar cómo responde el remolque al volante cuando vas hacia atrás.

## Cómo usarlo

Abre `index.html` en cualquier navegador moderno (ordenador, tablet o móvil en horizontal). No necesita instalación.

| Control | Acción |
|---|---|
| ← → | Girar el volante (o arrástralo con el ratón o el dedo) |
| ↓ / S | Freno progresivo · Espacio = freno a fondo |
| ↑ / W | Acelerador (en R el coche retrocede solo al ralentí, como un automático) |
| P R N D | Selector de marchas (con el coche parado) |
| Q / E, arrastrar | Mirar a los lados en la vista de conductor |
| 1 2 3 | Cámara de conductor, exterior o cenital |
| Retroceso | Volver 5 s atrás (entrenamiento) |
| 0 | Reiniciar |

También funciona con volantes y mandos de juego (eje 1 dirección, gatillos gas y freno).

## Qué simula

- Geometría del X5 E70: batalla 2,933 m, voladizo trasero 1,08 m, vía 1,65 m, dirección de 3 vueltas de tope a tope.
- Remolque de doble eje configurable: longitud de caja, lanza y posición de la bola. Mide el tuyo y ajústalo.
- Retrovisores reales en pantalla (imagen invertida, el derecho convexo) con bajada automática del derecho al meter la R, como el E70.
- Cambio automático con arrastre al ralentí y freno dosificable.
- Juez de examen: bordillo, líneas, jalones, detenerse, girar en parado, rectificar hacia delante y tijera.
- Modo entrenamiento con trayectoria prevista de las ruedas, ángulo de equilibrio del remolque y cuánto volante hace falta para mantener el ángulo.
- Modo examen: solo vista de conductor y retrovisores, sin ayudas.

Las medidas de la pista (anchura del carril y radio del bordillo) no están publicadas por la DGT y cambian entre centros de examen: ajústalas en **Ajustes** a las de tu pista.

## Publicarlo con GitHub Pages

1. Sube `index.html` y este `README.md` a un repositorio.
2. En el repositorio: **Settings → Pages → Deploy from a branch → main / (root)**.
3. En un par de minutos estará en `https://<tu-usuario>.github.io/<repositorio>/`.

Referencia de la maniobra: [DGT, maniobras para permisos B+E](https://www.dgt.es/nuestros-servicios/permisos-de-conducir/maniobras-be/).
