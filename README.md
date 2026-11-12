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
- **Comidas**: día por día, últimos 7 días y lo que más comes.
- **Historial**: calendario del mes (más oscuro = más pasos; puntitos = comidas). Toca un día para editarlo.
- **Ajustes**: nombre, meta de pasos, largo del paso, comidas del día, copia de seguridad (JSON) y exportar a Excel (CSV).

## Pasos desde Salud
Una web no puede leer la app Salud. Crea un Atajo: *Buscar muestras de salud (Pasos, hoy) → Calcular estadísticas (Suma) → Redondear → Copiar al portapapeles*. Luego en Paso: **+ → Pasos → Pegar**.

## Actualizar
Si cambias archivos, sube `VERSION` en `sw.js` para que el iPhone baje la versión nueva.
