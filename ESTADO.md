# ESTADO — pathonduty (página pública de PathOnDuty)

**Dueño:** Claude Web (cuenta 2) — programa y hace PR
**Auditor:** Claude App (cuenta 1) — revisa los PR, no hace commits aquí
**Autoriza:** Carlos (charliedays2020) — único que fusiona en `main`

## Versión actual (21-nov-2026)
| Archivo | Estado | Para qué |
|---|---|---|
| `index.html` | 18-nov-2026 | Página de la app |
| `privacidad.html` | «Última actualización: 18 de noviembre de 2026» | Política de privacidad registrada en Google Play |
| `play/` | 18-nov-2026 | Icono 512, gráfico destacado 1024×500 y 6 capturas de la ficha de Play |

- Se publica con GitHub Pages desde `main`. Repo público.
- El código de la app no está aquí: vive en el repo privado `TrackOnDuty`.
- `privacidad.html` es igual a `docs/play/privacidad-pathonduty.html` de TrackOnDuty (rama `prueba`).

## En curso
- PR #1 (`organizacion/readme` → `main`, 20-nov): agrega `README.md`. Esperando auditoría y OK de Carlos.

## Pendiente
- [ ] Corregir en la política quién borra los datos: hoy dice que el servidor borra la posición al terminar y los recorridos a los 90 días; lo hace la app (ver ESTADO de TrackOnDuty). Cambiar aquí y en `docs/play/` el mismo día y subir la fecha.
- [ ] Mencionar el WiFi directo (Wi-Fi Aware) en la política, porque la app lo usa.
- [ ] Actualizar capturas de `play/` cuando cambie la pantalla (por ejemplo, puntos de referencia de la 1.0.4).

## Decisiones tomadas
- 18-nov-2026 — Repo público separado solo para la página y la política que pide Google Play.
- 18-nov-2026 — Edad: mayores de 18; menores solo con permiso y acompañados por un adulto del grupo.
- 21-nov-2026 — Reparto: este repo es de Claude Web; auditoría cruzada con Claude App.

## No tocar sin autorización
- El nombre del repo y la ruta `privacidad.html` (la URL está registrada en Google Play).
- Cualquier cambio de la política: Play compara lo que dice con lo que hace la app.

## Notas para el auditor
- Toda edición de `privacidad.html` debe coincidir con `TrackOnDuty/docs/play/privacidad-pathonduty.html` y con el comportamiento real de la app (permisos, datos en Firebase, borrado).
- No subir aquí nada del código ni datos personales: el repo es público.
