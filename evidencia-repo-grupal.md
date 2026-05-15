# Sprint – Mejoras de UX en Dashboard

**Fecha:** 15/05/2026  
**Rama:** `feat/prueba-Mabe`

## Archivos modificados

- `src/app/dashboard/page.tsx`
- `src/app/dashboard/Dashboard.module.css`

---

#  HU-13 · Contadores numéricos en filtros de estado

**Archivo:** `src/app/dashboard/page.tsx`  
**Estilo:** `src/app/dashboard/Dashboard.module.css`

## Cambios realizados

Los *filter chips* del panel **"Planes de Test"** ahora muestran un badge numérico con la cantidad real de tests por estado, calculada dinámicamente desde los datos del workspace activo.

| Filtro | Dato mostrado |
|---|---|
| Todos | `analytics.total` |
| Borradores | Cantidad de tests en borrador |
| En progreso | Cantidad de tests activos |
| Finalizados | Cantidad de tests completados |

## Implementación

- Cada chip calcula su conteo utilizando `analytics.byStatus`
- El chip **"Todos"** muestra el total general mediante `analytics.total`
- El badge cambia visualmente cuando el filtro está activo:
  - Fondo blanco semitransparente
  - Contraste visual sobre el chip azul activo
- Se agregaron atributos accesibles `aria-label`
  - Ejemplo: `"Borradores: 3 tests"`
- Nuevas clases CSS implementadas:
  - `.filter-chip-count`
  - `.filter-chip-count-active`

## Beneficio UX

La navegación es más eficiente, ya que el usuario conoce la cantidad de elementos disponibles antes de aplicar un filtro, reduciendo clics innecesarios y mejorando la exploración visual del dashboard.

---

#  HU-10 · Reorganización de tarjetas de métricas

## Cambios realizados

Las KPI Cards del dashboard fueron reorganizadas en dos niveles de jerarquía visual para priorizar las métricas más importantes del proyecto.

### Antes

- 4 tarjetas distribuidas en una grilla uniforme `2 × 2`
- Todas las métricas tenían el mismo peso visual
- No existía diferenciación de prioridad

### Después

| Nivel | Cards | Tamaño del valor | Indicador visual |
|---|---|---|---|
| Primario | Tasa de Éxito · Tests Completados | `2rem` | Borde izquierdo de color |
| Secundario | Tiempo Promedio · Hallazgos | `1.5rem` | Diseño compacto sin acento |

## Implementación

- Nueva sección `.kpi-primary-row`
  - Ubica las métricas principales en la parte superior
- Clase `.kpi-card-primary`
  - Agrega borde lateral de color
  - Verde → éxito
  - Azul → tests completados
- Clase `.kpi-value-primary`
  - Escala los valores principales a `2rem`
- Clase `.kpi-sublabel`
  - Añade contexto debajo del indicador
  - Ejemplo: `"de N planes registrados"`
- Las métricas secundarias mantienen un diseño compacto y menos dominante visualmente

## Beneficio UX

La información ahora posee una jerarquía clara y escaneable.  
El usuario puede identificar rápidamente el estado general del proyecto sin necesidad de recorrer visualmente toda la grilla de métricas.

