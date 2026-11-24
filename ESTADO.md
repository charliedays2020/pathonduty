# ESTADO — pathonduty (página pública de PathOnDuty)

**Dueño:** Claude Web (cuenta 2) — programa y hace PR
**Auditor:** Claude App (cuenta 1) — revisa los PR, no hace commits aquí
**Autoriza:** Carlos (charliedays2020) — único que fusiona en `main`

## Versión actual (21-nov-2026)
| Archivo | Estado | Para qué |
|---|---|---|
| `index.html` | 18-nov-2026 | Página de la app |
| `privacidad.html` | «Última actualización: 21 de noviembre de 2026» (en el PR de la auditoría) | Política de privacidad registrada en Google Play |
| `play/` | 18-nov-2026 (icono 512 pasa a PNG de 32 bits con alfa el 21-nov) | Icono 512, gráfico destacado 1024×500 y 6 capturas de la ficha de Play |

- Se publica con GitHub Pages desde `main`. Repo público.
- El código de la app no está aquí: vive en el repo privado `TrackOnDuty`.
- `privacidad.html` es igual a `docs/play/privacidad-pathonduty.html` de TrackOnDuty (rama `prueba`).

- PR #2 (`estado/reparto-claude`, este `ESTADO.md`) ya está en `main`.

## En curso
- **Política para PathOnDuty 1.3.0 (24-nov)**, rama `politica/1.3.0-salidas` → `main`: «Mis salidas» y el resumen, huellas y camino del guía
  en el teléfono, peso opcional solo en el teléfono, barómetro, y compartir GPX/imagen solo si la persona lo hace. Fecha 24-nov.
  El mismo texto va en TrackOnDuty (`docs/play/privacidad-pathonduty.html`). **Fusionar los dos el mismo día, antes de subir la 1.3.0 a Play.**

- **PR de la auditoría de Claude App (21-nov)**, rama `auditoria/politica-21nov` → `main`. Esperando OK de Carlos:
  - política corregida y con fecha 21-nov: quién borra (la app), Wi-Fi Aware, número de emergencia del grupo en Firebase, a dónde va «Enviar reporte»;
  - el mismo cambio va en el PR de TrackOnDuty a `prueba` (`docs/play/privacidad-pathonduty.html`). **Fusionar los dos el mismo día.**
  - trae el `README.md` del PR #1 con la línea «© 2026 Carlos Díaz (carlday)»: al fusionar este, el **PR #1 se puede cerrar**;
  - icono 512 como PNG de 32 bits con alfa.

## Pendiente
- [ ] Capturas nuevas (auditoría 21-nov), las toma Carlos en el teléfono con la versión de prueba actual:
  - captura 1: pantalla de inicio sin desplazar (hoy «Iniciar salida» sale cortado arriba);
  - capturas 2 y 3: en El Cimarrón o en una ruta de ejemplo, **sin calles de Tegucigalpa ni su posición real**.
    El botón «Siguiéndome» ya no existe en la app (desde 2.1.2 es «◎ Centrar»), así que no hace falta arreglar nada en TrackOnDuty.
  - Las capturas viejas siguen en el historial de git aunque se reemplacen.
- [ ] Revisar la política cuando llegue el encargo 50 (PathOnDuty 1.1.0): las huellas de las salidas se guardarán en el teléfono para siempre (hasta «Borrar mis huellas»).
- [ ] Actualizar capturas de `play/` cuando cambie la pantalla (puntos de referencia de la 1.0.4, flechas y velocidad de la 1.0.9).

## Decisiones tomadas
- 18-nov-2026 — Repo público separado solo para la página y la política que pide Google Play.
- 18-nov-2026 — Edad: mayores de 18; menores solo con permiso y acompañados por un adulto del grupo.
- 21-nov-2026 — Reparto: este repo es de Claude Web; auditoría cruzada con Claude App.
- 21-nov-2026 — Política: se dice lo que hace la app de verdad (la app borra, no el servidor; el número personal no sale del teléfono).

## No tocar sin autorización
- El nombre del repo y la ruta `privacidad.html` (la URL está registrada en Google Play).
- Cualquier cambio de la política: Play compara lo que dice con lo que hace la app.

## Notas para el auditor
- Toda edición de `privacidad.html` debe coincidir con `TrackOnDuty/docs/play/privacidad-pathonduty.html` y con el comportamiento real de la app (permisos, datos en Firebase, borrado).
- No subir aquí nada del código ni datos personales: el repo es público.
