# Product Backlog - Usability Test Dashboard

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

## Tema

Desarrollo de la Planificación para el primer sprint

## Semestre

Quinto "A"

## Periodo Académico

Enero 2026 – Agosto 2026

---

## 1. Presentación general del proyecto

El proyecto **Usabilidad Test Dashboard** consiste en el desarrollo de una aplicación web full-stack orientada a la gestión, registro y análisis de pruebas de usabilidad, permitiendo digitalizar procesos que anteriormente se realizaban en hojas de cálculo Excel.

El sistema permite crear pruebas mediante un modelo tipo Wizard de múltiples pasos, registrar tareas, almacenar observaciones del moderador y visualizar métricas mediante un dashboard interactivo con indicadores visuales en tiempo real.

Además, el aplicativo centraliza la información en una base de datos persistente, permitiendo a los equipos de desarrollo analizar resultados de usabilidad desde una única plataforma organizada y accesible.

### Objetivo general

Desarrollar una aplicación web que permita planificar, ejecutar y analizar pruebas de usabilidad, facilitando la recolección estructurada de datos y la visualización de métricas mediante un dashboard interactivo, asegurando la accesibilidad y eficiencia en la evaluación de interfaces digitales.

---

## 2. Arquitectura tecnológica

El sistema se desarrolló bajo un modelo full-stack con separación de responsabilidades, utilizando arquitectura limpia (Clean Architecture) y principios SOLID, lo que permite una mayor escalabilidad y mantenibilidad del software.

| Componente | Tecnología | Descripción |
|------------|-------------|-------------|
| Frontend | Next.js v16 | Framework basado en React para desarrollo de interfaces web dinámicas |
| Backend | NestJS | Framework modular para desarrollo backend robusto |
| ORM | TypeORM | Manejo de entidades y persistencia de datos |
| Base de datos | MySQL | Sistema relacional para almacenamiento estructurado |
| Arquitectura | Clean Architecture | Separación por capas (Dominio, Aplicación, Infraestructura, Presentación) |
| Control de versiones | Git + GitHub | Manejo de versiones mediante Git Flow |
| Evaluación de calidad | WAVE, Stark, Lighthouse | Herramientas para evaluación de accesibilidad y rendimiento |

El sistema utiliza una estructura basada en capas que permite separar la lógica del dominio de la infraestructura y la presentación, facilitando el mantenimiento y escalabilidad del software.

---

## 3. Lógica esperada por el sistema

El flujo principal del sistema está diseñado para permitir al usuario crear pruebas de usabilidad mediante un proceso guiado y posteriormente analizar los resultados obtenidos.

### Flujo lógico del sistema

| Paso | Proceso |
|------|---------|
| 1 | Creación de prueba mediante Wizard |
| 2 | Registro de tareas del test |
| 3 | Registro de perfiles y observaciones |
| 4 | Almacenamiento de notas del moderador |
| 5 | Actualización del estado del test |
| 6 | Visualización de métricas en dashboard |

El sistema realiza solicitudes HTTP como:

- POST → creación de notas
- PUT → actualización de pruebas
- PATCH → cambio de estado del test

Estas operaciones permiten mantener el progreso del test en estado IN_PROGRESS dentro de la base de datos.

---

## 4. Reglas de Negocio

Las reglas de negocio definen el comportamiento lógico que el sistema debe cumplir para garantizar el correcto funcionamiento.

| Código | Regla |
|--------|-------|
| RN-01 | Todo test debe contener información básica antes de ser guardado |
| RN-02 | Un test puede contener múltiples tareas |
| RN-03 | Cada tarea debe incluir escenario, resultado esperado y criterio de éxito |
| RN-04 | Un test puede contener múltiples notas del moderador |
| RN-05 | El estado del test debe actualizarse automáticamente según el progreso |
| RN-06 | Solo se pueden visualizar métricas cuando existen datos registrados |
| RN-07 | Los datos deben persistirse correctamente en la base de datos |
| RN-08 | El sistema debe validar datos antes de almacenarlos |
| RN-09 | El dashboard debe mostrar indicadores clave del estado de los tests |
| RN-10 | El sistema debe permitir filtrado dinámico por estado |

Estas reglas se basan en las relaciones entre entidades como UsabilityTest, TestTask, ModeratorNote y UsabilityMetric, las cuales mantienen relaciones uno-a-muchos dentro del sistema.

---

## 5. Marco legal que se aplica dentro de Ecuador

El desarrollo del sistema debe cumplir con normativas tecnológicas y legales vigentes en el Ecuador.

| Norma | Descripción |
|-------|-------------|
| Ley de Comercio Electrónico, Firmas Electrónicas y Mensajes de Datos | Regula el uso de sistemas electrónicos y almacenamiento digital |
| Ley Orgánica de Protección de Datos Personales | Protege la información personal de los usuarios |
| Norma Técnica Ecuatoriana de Accesibilidad Web | Garantiza accesibilidad digital |
| ISO 9241-11 | Estándar internacional sobre usabilidad |
| WCAG 2.2 | Estándar internacional de accesibilidad web |

El cumplimiento de estándares como WCAG 2.2 fue validado mediante herramientas como WAVE y Stark para asegurar accesibilidad en el sistema.

---

## 6. Conocimiento Técnico

El desarrollo del proyecto requirió conocimientos técnicos relacionados con desarrollo web moderno, arquitectura limpia y evaluación de accesibilidad.

| Área | Descripción |
|------|-------------|
| Programación Frontend | Desarrollo con Next.js y React |
| Programación Backend | Desarrollo con NestJS |
| Bases de Datos | Diseño relacional con MySQL |
| Arquitectura de Software | Clean Architecture |
| Diseño UI/UX | Uso de Wizard y Dashboard |
| Control de Versiones | Git y GitHub |
| Accesibilidad Web | Evaluación con WAVE y Stark |
| Testing | Pruebas funcionales y de accesibilidad |

El uso de herramientas como Lighthouse permitió analizar el rendimiento del aplicativo y detectar posibles mejoras en la estructura HTML.

---

## 7. Capacidad del equipo de trabajo

### Distribución de horas por integrante

| Integrante | Cantidad de días de trabajo | Cantidad de horas por día entre semana | Cantidad de horas por fin de semana | Total de horas de trabajo por integrante |
|------------|-----------------------------|----------------------------------------|-------------------------------------|------------------------------------------|
| Anthony Punina | 13 | 2 | 4 | 40 |
| Xabier Perez | 13 | 2 | 4 | 40 |
| Erick Guerrón | 13 | 2 | 4 | 40 |
| Maria Zapata | 13 | 2 | 4 | 40 |

### Total de horas del equipo

| Concepto | Horas |
|----------|-------|
| Total horas disponibles | 160 |
| Margen de imprevistos (-10%) | 16 |
| Total horas efectivas | 144 |

### Habilidades de los integrantes

| Integrante | Habilidad |
|------------|-----------|
| Erick Guerrón | Desarrollador Fullstack |
| Xabier Perez | Desarrollador Fullstack |
| Anthony Punina | Desarrollador Fullstack |
| Maria Zapata | Desarrollador Fullstack |

El trabajo colaborativo del equipo se caracterizó por comunicación constante y coordinación mediante herramientas compartidas, lo que permitió mantener el progreso del proyecto sin interrupciones.

---

## 8. Product Backlog – Usability Test Dashboard

| ID | Historia de Usuario | Descripción | Prioridad | Valor de Negocio |
|----|---------------------|-------------|-----------|------------------|
| PB-01 | Crear Plan de Prueba | Como moderador quiero crear un plan de prueba para organizar las evaluaciones de usabilidad | Alta | Permite iniciar cualquier proceso de test |
| PB-02 | Gestionar Tareas del Test | Como moderador quiero registrar tareas para evaluar la interacción del usuario | Alta | Permite medir el desempeño del usuario |
| PB-03 | Registrar Participantes | Como evaluador quiero registrar perfiles de usuarios para analizar resultados | Alta | Permite segmentar resultados |
| PB-04 | Registrar Observaciones | Como evaluador quiero guardar errores, comentarios y tiempos | Alta | Permite identificar problemas de usabilidad |
| PB-05 | Registrar Hallazgos | Como analista quiero registrar problemas detectados y su severidad | Alta | Permite priorizar mejoras |
| PB-06 | Mostrar Dashboard Principal | Como usuario quiero visualizar indicadores gráficos del test | Alta | Facilita toma de decisiones rápida |
| PB-07 | Filtrar Tests por Estado | Como usuario quiero filtrar tests por estado | Media | Mejora navegación |
| PB-08 | Editar Test Existente | Como moderador quiero modificar datos del test | Media | Permite actualización de información |
| PB-09 | Eliminar Test | Como moderador quiero eliminar tests innecesarios | Media | Mantiene base organizada |
| PB-10 | Visualizar Métricas KPI | Como usuario quiero ver estadísticas de resultados | Alta | Permite análisis rápido |
| PB-11 | Exportar Resultados | Como analista quiero generar reportes | Media | Permite documentación formal |
| PB-12 | Validación de Formularios | Como sistema quiero validar datos antes de guardar | Alta | Evita errores en base de datos |
| PB-13 | Soporte Responsive | Como usuario quiero usar el sistema desde móvil o tablet | Media | Mejora accesibilidad |
| PB-14 | Gestión de Roles | Como administrador quiero definir roles del test | Media | Mejora control del sistema |
| PB-15 | Visualización Gráfica | Como usuario quiero ver gráficos de resultados | Alta | Facilita interpretación visual |

---

## 9. Definición de hecho

| Criterio | Descripción |
|----------|-------------|
| Código funcional | El módulo funciona sin errores críticos |
| Persistencia de datos | Los datos se guardan correctamente en MySQL |
| Validación implementada | Formularios validan entradas obligatorias |
| Interfaz usable | Cumple principios de usabilidad |
| Responsive | Funciona en escritorio y tablet |
| Pruebas realizadas | Evaluado con WAVE y Lighthouse |
| Documentación actualizada | Código y funcionalidades documentadas |
| Integración exitosa | Compatible con backend y frontend |

---

## 10. Historias de usuario

Ya que se solicitó un aplicativo completo para la fecha de entrega se planificó un solo sprint unificado basado en tareas generales para cada desarrollador, buscando cumplir con el prototipo completo para la entrega, donde se trabajaron solo 8 historias de usuario.

| ID | Historia de usuario | Valor de negocio | Prioridad |
|----|---------------------|------------------|-----------|
| HU-01 | Como moderador, quiero registrar tareas del test para organizar las actividades del participante | Permite estructurar correctamente los tests | Alta |
| HU-02 | Como moderador, quiero registrar observaciones durante el test para documentar comportamientos del usuario | Facilita el análisis posterior | Alta |
| HU-03 | Como evaluador, quiero registrar sesiones de testing para llevar control de cada ejecución | Permite trazabilidad del test | Alta |
| HU-04 | Como analista, quiero visualizar indicadores en el dashboard para medir el rendimiento del test | Facilita toma de decisiones | Alta |
| HU-05 | Como equipo UX, quiero registrar hallazgos detectados en el test para identificar problemas de usabilidad | Permite detectar errores críticos | Alta |
| HU-06 | Como desarrollador, quiero registrar mejoras sugeridas para optimizar la interfaz | Permite evolución continua del sistema | Media |
| HU-07 | Como usuario del sistema, quiero editar registros existentes para corregir errores | Mantiene consistencia de datos | Media |
| HU-08 | Como usuario, quiero visualizar resúmenes del test completado para analizar resultados | Facilita evaluación final | Media |

---

*Documento generado para el proyecto Usability Test Dashboard - Universidad Técnica de Ambato*