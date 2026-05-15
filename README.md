# Usability Test Dashboard 2.0 — HCI Final Project

## Descripción del proyecto

Este repositorio contiene el desarrollo de la prueba final de Interacción Humano Computador (HCI), enfocada en el análisis, evaluación y mejora del sistema **“Usability Test Dashboard 2.0”** mediante principios de UX, arquitectura de información, evaluación heurística y metodología Scrum.

El objetivo principal fue identificar problemas reales de usabilidad dentro del dashboard institucional y proponer mejoras funcionales y visuales centradas en el usuario, implementando cambios reales sobre el sistema y documentando todo el proceso mediante GitHub.

---

# Objetivos aplicados

- Aplicar principios HCI y UX en un sistema real
- Realizar evaluación heurística completa del aplicativo
- Detectar problemas críticos, moderados y leves
- Mejorar la navegación y organización visual del dashboard
- Implementar mejoras funcionales reales
- Aplicar Scrum para planificación y seguimiento
- Documentar el proceso técnico y visual
- Utilizar herramientas IA como apoyo en diseño y documentación

---

# Trabajo realizado dentro del proyecto

## 1. Planificación Scrum

Se desarrolló la planificación inicial del proyecto utilizando una estructura Scrum básica:

- Product Backlog
- Sprint Backlog
- Historias de usuario
- Priorización de tareas
- Fases internas del sprint
- Definición de terminado (DoD)

Además, se construyó un sprint específico enfocado en mejoras heurísticas y optimización UX del dashboard.

---

# 2. Evaluación Heurística

Se realizó una evaluación heurística sobre múltiples pantallas del sistema:

- Dashboard principal
- Gestión de grupos
- Configuración
- Métricas
- Navegación
- Reportes

## Problemas detectados

Se identificaron problemas relacionados con:

- Consistencia visual
- Navegación contextual
- Accesibilidad
- Jerarquía visual
- Prevención de errores
- Feedback visual
- Reconocimiento de acciones
- Sobrecarga cognitiva

Los hallazgos fueron clasificados según severidad:

- Críticos
- Moderados
- Leves

Además, se construyeron matrices heurísticas completas utilizando principios de Nielsen.

---

# 3. Rediseño UX aplicado

Se trabajó principalmente sobre el Dashboard principal del sistema, aplicando:

- Jerarquización visual de métricas
- Reorganización de KPI Cards
- Arquitectura de información
- Optimización de navegación
- Mejora de accesibilidad visual
- Diseño centrado en comprensión rápida del estado del sistema

## Mejoras implementadas

### HU-13 — Contadores numéricos en filtros

Se añadieron badges dinámicos en los filtros de estado para mostrar la cantidad real de tests disponibles antes de aplicar un filtro.

### HU-10 — Reorganización de métricas

Las métricas principales fueron reorganizadas visualmente en niveles de prioridad para mejorar la lectura y escaneo rápido del dashboard.

---

# 4. Implementación funcional

Las mejoras UX fueron implementadas directamente dentro del proyecto utilizando:

- React / Next.js
- CSS Modules
- Componentes dinámicos
- Feedback visual
- Accesibilidad mediante `aria-label`
- Estados activos visuales

## Archivos modificados

```bash
src/app/dashboard/page.tsx
src/app/dashboard/Dashboard.module.css
