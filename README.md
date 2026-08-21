# AsistentAsistente Pedagógico Curricular y Evaluador Inteligente

© SIP - SYSTEM INTELLIGENCE PLATFORM 2026

Plataforma inteligente para docentes universitarios y escolares orientada al análisis curricular, diseño pedagógico, generación supervisada de evaluaciones y análisis de resultados académicos.

---

1. Propósito

El sistema transforma materiales académicos proporcionados por el docente —como mallas curriculares, sílabos, sumillas, capítulos, PDF, presentaciones, textos y resúmenes— en recursos pedagógicos estructurados.

Su propósito no es únicamente generar preguntas, sino apoyar el ciclo completo de planificación, enseñanza, evaluación y mejora educativa.

Flujo principal

Material académico → Análisis curricular → Diagnóstico pedagógico → Diseño de evaluación → Preguntas → Revisión docente → Aprobación → Examen → Resultados → Retroalimentación

---

2. Funciones principales

Análisis curricular

- Identificación de competencias.
- Identificación de resultados de aprendizaje.
- Organización de unidades, temas y subtemas.
- Identificación del nivel de profundidad conceptual.
- Análisis de coherencia entre contenidos y resultados.
- Detección de contenidos insuficientemente evaluados.
- Matriz de alineación curricular.

Asistencia pedagógica

El sistema puede proponer:

- estrategias metodológicas;
- metodologías activas;
- aprendizaje basado en problemas;
- aprendizaje basado en proyectos;
- estudio de casos;
- aula invertida;
- actividades colaborativas;
- actividades de refuerzo;
- evaluación formativa;
- estrategias de innovación educativa;
- recomendaciones para mejorar la coherencia entre enseñanza y evaluación.

Las recomendaciones deben estar vinculadas al contenido y a los resultados de aprendizaje, evitando sugerencias genéricas.

---

3. Evaluación inteligente

El sistema genera bancos de preguntas a partir del material fuente.

Cada pregunta debe mantener trazabilidad con:

- curso;
- unidad;
- tema;
- subtema;
- competencia;
- resultado de aprendizaje;
- material fuente;
- ubicación o referencia del contenido;
- nivel cognitivo;
- dificultad;
- tipo de pregunta;
- respuesta correcta;
- distractores;
- justificación pedagógica.

Niveles cognitivos

Se contempla una clasificación basada en la progresión cognitiva:

1. Recordar
2. Comprender
3. Aplicar
4. Analizar
5. Evaluar
6. Crear

El sistema debe detectar desequilibrios, por ejemplo, una evaluación excesivamente concentrada en memoria y comprensión.

---

4. Revisión y aprobación docente

Las preguntas generadas por IA no deben publicarse automáticamente.

Cada pregunta debe pasar por un proceso de control:

Generada → En revisión → Corregida → Aprobada → Disponible para examen

También debe poder:

- editarse;
- rechazarse;
- regenerarse;
- modificar sus alternativas;
- cambiar su dificultad;
- cambiar su nivel cognitivo;
- consultar su fuente;
- consultar su objetivo educativo.

La decisión final sobre la publicación de una pregunta corresponde al docente.

---

5. Generación de exámenes

El docente podrá seleccionar:

- cantidad de preguntas;
- unidades;
- temas;
- competencias;
- resultados de aprendizaje;
- dificultad;
- nivel cognitivo;
- tipo de pregunta;
- tiempo disponible;
- puntaje;
- nota mínima aprobatoria.

El sistema podrá generar diferentes versiones:

- Examen A
- Examen B
- Examen C
- Examen D

Cada versión podrá modificar:

- orden de preguntas;
- orden de alternativas.

La aleatorización debe conservar la equivalencia pedagógica entre versiones.

No se debe generar una versión más fácil o más difícil simplemente por haber sido barajada.

---

6. Examen interactivo

La interfaz del alumno podrá incluir:

- una pregunta por pantalla;
- temporizador;
- indicador de progreso;
- alternativas aleatorias;
- navegación configurable;
- guardado de respuestas;
- envío automático al finalizar el tiempo;
- cálculo automático de resultados.

El comportamiento de navegación y revisión deberá ser configurable por el docente.

---

7. Resultados y analítica

El sistema podrá calcular:

- puntaje obtenido;
- porcentaje;
- nota final;
- aprobado/desaprobado;
- promedio;
- mediana;
- distribución de calificaciones;
- rendimiento por unidad;
- rendimiento por competencia;
- rendimiento por resultado de aprendizaje;
- rendimiento por pregunta;
- preguntas con mayor porcentaje de error.

El objetivo es pasar de una simple calificación a un diagnóstico del aprendizaje.

Ejemplo:

«El estudiante obtuvo 14/20. Presenta dominio adecuado de los contenidos conceptuales, pero evidencia dificultades en preguntas de aplicación y análisis correspondientes a la Unidad 3.»

---

8. Diagnóstico de la evaluación

La plataforma debe analizar la calidad de una evaluación antes de su publicación.

Puede identificar:

- exceso de preguntas memorísticas;
- ausencia de preguntas de aplicación;
- ausencia de preguntas de análisis;
- temas sobrerrepresentados;
- temas sin evaluar;
- resultados de aprendizaje sin evidencia;
- desequilibrio de dificultad;
- problemas de alineación curricular.

Ejemplo

Cobertura curricular              84%
Alineación curricular             78%
Recordar                           30%
Comprender                         30%
Aplicar                            25%
Analizar                           15%

⚠ Recomendación:
Incrementar preguntas de análisis
y aplicación en la Unidad 3.

---

9. Arquitectura prevista

La aplicación podrá evolucionar hacia una arquitectura basada en Next.js / React / TypeScript.

mi-app-docente/
├─ src/
│  ├─ app/
│  │  ├─ layout.tsx
│  │  ├─ page.tsx
│  │  ├─ globals.css
│  │  ├─ login/
│  │  ├─ dashboard/
│  │  ├─ cursos/
│  │  ├─ examenes/
│  │  ├─ alumnos/
│  │  ├─ resultados/
│  │  └─ api/
│  │
│  ├─ components/
│  ├─ features/
│  │  ├─ auth/
│  │  ├─ cursos/
│  │  ├─ curriculum/
│  │  ├─ materiales/
│  │  ├─ preguntas/
│  │  ├─ examenes/
│  │  ├─ alumnos/
│  │  ├─ resultados/
│  │  └─ pedagogia/
│  │
│  ├─ lib/
│  ├─ types/
│  └─ hooks/
│
├─ public/
├─ .env.example
├─ .gitignore
├─ package.json
├─ tsconfig.json
├─ next.config.js
├─ tailwind.config.ts
└─ README.md

---

10. Módulos funcionales

Dashboard

Panel central del docente con:

- cursos activos;
- materiales;
- preguntas pendientes;
- preguntas aprobadas;
- exámenes;
- alumnos;
- resultados;
- alertas pedagógicas.

Cursos

Gestión de:

- cursos;
- períodos académicos;
- docentes;
- unidades;
- temas;
- competencias;
- resultados de aprendizaje.

Materiales

Carga y organización de:

- PDF;
- Word;
- PPT/PPTX;
- TXT;
- contenidos pegados;
- capítulos;
- sílabos;
- sumillas;
- otros recursos académicos.

Currículo

Permite construir la relación:

Competencia → Resultado de aprendizaje → Contenido → Actividad → Evidencia → Evaluación

Banco de preguntas

Repositorio de preguntas revisadas y aprobadas.

Exámenes

Creación y administración de evaluaciones y versiones balotadas.

Alumnos

Gestión de estudiantes, cursos e inscripciones.

Resultados

Análisis individual y grupal.

Mejora pedagógica

Módulo destinado a generar recomendaciones de:

- metodología;
- actividades;
- innovación;
- refuerzo;
- evaluación;
- alineación curricular.

---

11. Principio de trazabilidad

Una característica fundamental del sistema será la trazabilidad.

Cada pregunta debe poder responder:

«¿De dónde salió esta pregunta?»

Y mostrar:

Curso
 ↓
Unidad
 ↓
Tema
 ↓
Resultado de aprendizaje
 ↓
Material fuente
 ↓
Página / sección
 ↓
Pregunta
 ↓
Nivel cognitivo
 ↓
Resultado del alumno

Esto permite auditar la relación entre el contenido enseñado y lo evaluado.

---

12. Principio de supervisión humana

La inteligencia artificial funciona como asistente, no como autoridad académica final.

El docente conserva el control sobre:

- contenidos;
- competencias;
- resultados;
- preguntas;
- respuestas;
- dificultad;
- ponderaciones;
- exámenes;
- publicación;
- interpretación pedagógica.

---

13. Estado actual

El repositorio contiene actualmente un prototipo inicial de interfaz ("index.html") que representa visualmente el concepto del dashboard.

La evolución del proyecto deberá realizarse sobre esta base, evitando crear múltiples "index.html" independientes o reemplazar innecesariamente archivos existentes.

La prioridad será transformar progresivamente el prototipo visual en módulos funcionales conectados.

---

14. Principio de desarrollo

El proyecto debe priorizar:

1. Funcionalidad real.
2. Integración entre módulos.
3. Persistencia de datos.
4. Trazabilidad.
5. Seguridad.
6. Usabilidad docente.
7. Diseño responsive.
8. Compatibilidad móvil.
9. Validación pedagógica.
10. Calidad del código.

No se considera terminado un módulo únicamente porque su interfaz visual exista.

Un módulo se considera funcional cuando:

interfaz + lógica + datos + validación + flujo completo

operan correctamente.

---

15. Visión

Convertir la plataforma en un sistema de inteligencia educativa capaz de asistir al docente desde la planificación curricular hasta el análisis posterior de los resultados.

La plataforma debe ayudar a responder cuatro preguntas:

¿Qué enseñar?

Análisis curricular y resultados de aprendizaje.

¿Cómo enseñar?

Metodologías, actividades e innovación pedagógica.

¿Cómo evaluar?

Diseño de instrumentos alineados con los resultados.

¿Qué aprendieron los estudiantes?

Análisis inteligente de resultados y detección de dificultades.

---

© SIP - SYSTEM INTELLIGENCE PLATFORM 2026

Asistente Pedagógico Curricular y Evaluador Inteligente

Sistema orientado a la asistencia docente, mejora curricular, evaluación educativa y análisis inteligente del aprendizaje.

© SIP - SYSTEM INTELLIGENCE PLATFORM 2026 — Todos los derechos reservados.e-Pedag-gico-Curricular-y-Evaluador-Inteligente-para-docentes-universitarios-y-escolares
