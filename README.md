# Paso · tracker de pasos y comidas

App web (PWA) para el iPhone: registro mis pasos, lo que como y mi actividad de la semana.
Los datos se guardan solo en el teléfono (no hay servidor).

## Instalar en el iPhone
1. Activa GitHub Pages: **Settings → Pages → Branch: `main` / `(root)` → Save**.
2. Abre `https://sh31lby.github.io/Tracker-Comida/` en **Safari**.
3. Botón Compartir → **Añadir a pantalla de inicio**.

## Qué tiene
- **Hoy**: pasos del día con anillo de progreso, media semanal con barras, las comidas del día (Desayuno, Almuerzo, Lonche, Cena), objetivos de la semana y el mapa del mes. Vista Hoy / Semana / Mes.
- **Actividad**: pasos por semana o mes, media, mejor día, días cumplidos y km.
- **Comidas por partes con cantidad**: Desayuno y Lonche (bebida, panes, acompañamiento), Almuerzo y Cena (entrada, segundo, postre, bebida). Las partes se cambian en Ajustes.
- **Extra**: lo que no encaja en ninguna comida (una gaseosa, un postre suelto…). No cuenta para la meta.
- **Agua**: vasos del día con meta (8 × 250 ml por defecto).
- **Comidas**: día por día, últimos 7 días y "Lo que más comes" separado por comida y parte (este mes o todo).
- **Historial**: calendario del mes (más oscuro = más pasos; puntitos = comidas). Toca un día para editarlo.
- **Ajustes**: nombre, metas de pasos y agua, largo del paso, comidas y sus partes, copia de seguridad (JSON).

## Exportar a CSV (análisis de fin de mes)
En **Historial** (el mes que estás viendo) o en **Ajustes** (un mes o todo):
- **CSV detallado**: una fila por alimento — Fecha, Mes, Día, Tipo (Comida / Extra / Agua / Pasos), Comida, Hora, Parte, Alimento, Cantidad, Unidad.
- **CSV resumen por día**: pasos, km, agua, si cumpliste cada meta, qué comiste en cada comida y los extras.

Separado por `;` y con decimales con coma, para que Excel en español lo abra directo.

## Pasos desde Salud
Una web no puede leer la app Salud. Crea un Atajo: *Buscar muestras de salud (Pasos, hoy) → Calcular estadísticas (Suma) → Redondear → Copiar al portapapeles*. Luego en Paso: **+ → Pasos → Pegar**.

## Actualizar
Si cambias archivos, sube `VERSION` en `sw.js` para que el iPhone baje la versión nueva.
