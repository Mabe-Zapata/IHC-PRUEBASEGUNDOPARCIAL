# Evidencia de Uso de Inteligencia Artificial - Usability Test Dashboard

---

## Universidad Técnica de Ambato

### Facultad de Ingeniería en Sistemas, Electrónica e Industrial

### Carrera de Software

---

## Integrantes

- Guerron Chiluisa Erick Patricio
- Perez Perez Xabier David
- Punina Chisag Anthony Israel
- Zapata Reyes Maria Belen

## Materia

Interacción Humano Computador

## Proyecto

Usability Test Dashboard

## Periodo Académico

Enero 2026 – Agosto 2026

---

## 1. Introducción

El presente documento tiene como objetivo registrar y documentar la utilización de herramientas de Inteligencia Artificial, específicamente ChatGPT, durante el proceso de desarrollo del proyecto Usability Test Dashboard. Este registro responde a los estándares establecidos por la Universidad Técnica de Ambato para la transparente incorporación de tecnologías de IA en proyectos académicos.

La documentación de estas herramientas permite evaluar de manera crítica su aporte al proceso de desarrollo, identificando tanto las ventajas como las limitaciones que presentan, garantizando así la integridad académica y el aprendizaje efectivo por parte de los integrantes del equipo de trabajo.

---

## 2. Procesos Realizados con Inteligencia Artificial

A continuación se presenta el registro de las diferentes actividades donde se utilizó ChatGPT como herramienta de apoyo durante el desarrollo del proyecto.

### 2.1 Generación de Documentación

| Proceso | Descripción | Herramienta IA Utilizada | Output Obtenido |
|---------|-------------|--------------------------|-----------------|
| Elaboración de Product Backlog | Creación del documento backlog con historias de usuario, reglas de negocio y criterios de aceptación | ChatGPT | Estructura completa del Product Backlog |
| Estructura de evidencia IA | Generación de plantilla para documentar uso de IA en el proyecto | ChatGPT | Plantilla inicial del documento |
| Matriz Heurística | Generación de tabla en formato Markdown con los hallazgos de evaluación heurística | ChatGPT | Matriz formateada correctamente |

### 2.2 Desarrollo Técnico

| Proceso | Descripción | Herramienta IA Utilizada | Output Obtenido |
|---------|-------------|--------------------------|-----------------|
| ?? | ?? | ?? | ?? |

### 2.3 Análisis y Diseño

| Proceso | Descripción | Herramienta IA Utilizada | Output Obtenido |
|---------|-------------|--------------------------|-----------------|
| ?? | ?? | ?? | ?? |

---

## 3. Matriz Heurística - Evaluación de Usabilidad

A continuación se presenta el análisis de la pantalla principal del aplicativo donde se identificaron los siguientes fallos correspondientes al dashboard de ingreso:

| # | Heurística | Pantalla | Problema detectado | Severidad |
|---|------------|----------|--------------------|-----------|
| 01 | H2- Relación entre el sistema y el mundo real | Dashboard principal | La gráfica correspondiente a evolución de test de los últimos 30 días cuenta con etiquetas en inglés mientras que todo el sistema se encuentra en español | Media |
| 02 | H8- Diseño estético y minimalista | Dashboard principal | Existe una sobrecarga de datos que puede sobreestimular con información al usuario ya que presenta datos sobre los principales test pero específicos sobre solo el que se está presentando en las tarjetas | Baja |
| 03 | H3- Control y libertad del usuario | Dashboard principal | Al exportar el PDF correspondiente al resumen ejecutivo se muestra en una pantalla externa a la correspondiente dentro del sistema obligando al usuario a salir del flujo del aplicativo | Alta |
| 04 | H4- Consistencia y estándares | Dashboard principal (Métricas) | El indicador de "Tiempo Promedio" muestra un valor negativo (-10%) en color rojo. En rendimiento, reducir el tiempo suele ser positivo, por lo que el uso del color rojo contradice la semántica del éxito en el dominio del software | Media |
| 05 | H7- Flexibilidad y eficiencia de uso | Dashboard principal (Planes de test) | Las pestañas de filtrado (Borradores, En progreso, etc.) no muestran contadores numéricos. El usuario debe hacer clic en cada una para saber si hay contenido, aumentando el esfuerzo para obtener un resumen rápido | Baja |
| 06 | H1- Visibilidad del estado del sistema | Dashboard principal (Gráficas) | Las gráficas de líneas en las tarjetas de métricas carecen de etiquetas de datos o puntos de información (tooltips). El usuario ve la tendencia pero no puede conocer el valor exacto en un punto específico del tiempo | Media |
| 07 | H8- Diseño estético y minimalista | Dashboard principal (General) | El contraste de las etiquetas de texto pequeñas (como "3 TOTAL" o los ejes de la gráfica de barras) es demasiado bajo respecto al fondo, dificultando la legibilidad y violando principios de accesibilidad visual | Baja |

---

## 4. Análisis de Hallazgos

### 4.1 Hallazgos de Severidad Alta

| ID | Problema | Impacto | Recomendación |
|----|----------|---------|---------------|
| H3 | Exportación de PDF en pantalla externa | El usuario abandona el flujo natural de la aplicación, generando fricción en la experiencia | Implementar modal o vista embebida dentro del sistema para la visualización del PDF |

### 4.2 Hallazgos de Severidad Media

| ID | Problema | Impacto | Recomendación |
|----|----------|---------|---------------|
| H2 | Gráficas en inglés | Inconsistencia idiomática que puede confundir al usuario | Localizar todas las etiquetas de las gráficas al español |
| H4 | Indicador de tiempo en rojo | Semántica contradictoria que puede malinterpretarse | Utilizar color verde para indicar mejora (reducción de tiempo) |
| H1 | Gráficas sin tooltips | Usuario no puede obtener valores exactos | Implementar puntos interactivos con información al pasar el cursor |

### 4.3 Hallazgos de Severidad Baja

| ID | Problema | Impacto | Recomendación |
|----|----------|---------|---------------|
| H8 (sobrecarga) | Exceso de información en tarjetas | Puede generar sobrecarga cognitiva | Simplificar contenido mostrado, mostrar solo datos esenciales |
| H7 | Pestañas sin contadores | Usuario debe explorar cada pestaña manualmente | Agregar contadores numéricos en cada pestaña |
| H8 (contraste) | Contraste bajo en texto pequeño | Dificultad de lectura, problema de accesibilidad | Aumentar contraste entre texto y fondo |

---

## 5. Criterios de Evaluación del Uso de IA

| Criterio | Descripción | Cumplimiento |
|----------|-------------|--------------|
| Transparencia | Documentar claramente dónde se utilizó IA | ✓ |
| Validación | Verificar que el output generado sea correcto | ✓ |
| Aprendizaje | El equipo comprendió el proceso generado | ✓ |
| Originalidad | El código/documento fue adaptado a las necesidades del proyecto | ✓ |
| Ethical AI | Uso responsable de la herramienta de IA | ✓ |

---

## 6. Conclusiones

El uso de ChatGPT como herramienta de apoyo en el desarrollo del proyecto permitió optimizar tiempos en la generación de documentación inicial y estructuración de archivos. Sin embargo, es importante destacar que todo el contenido generado fue revisado, validado y adaptado por los integrantes del equipo de trabajo para garantizar su correcta aplicación al contexto específico del proyecto.

La evaluación heurística realizada sobre el dashboard principal permitió identificar 7 hallazgos de usabilidad, los cuales representan oportunidades de mejora para futuras iteraciones del aplicativo.

---

*Documento generado para el proyecto Usability Test Dashboard - Universidad Técnica de Ambato*
*Nota: Este documento se actualizará conforme se avance en el desarrollo del proyecto*