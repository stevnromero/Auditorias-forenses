# PROYECTO ACADÉMICO: AUDITORÍA DE DATOS Y PENSAMIENTO CRÍTICO FRENTE A SESGOS COGNITIVOS EN DEBATES POLARIZADOS

**Autor:** Steven  
**Formación:** Tecnólogo en Análisis y Desarrollo de Software (ADSO) – SENA | Analítica de Datos – UNAD  
**Fecha:** Noviembre de 2026  
**Área de aplicación:** Calidad de Datos, Analítica Básica y Lógica Argumentativa  

---

## 1. Resumen Ejecutivo

Este proyecto propone una metodología sencilla basada en **principios de calidad de datos y análisis de información** para evaluar debates cotidianos y deportivos marcados por la polarización. 

Mediante la limpieza de información irrelevante, la consulta de fuentes oficiales y el uso de una tabla de verificación, se examina la validez de las afirmaciones de cada participante, **incluido el propio autor**, utilizando criterios claros, objetivos y verificables.

> **Nota de alcance:** Este es un ejercicio académico exploratorio. Sus resultados describen únicamente los casos revisados y no buscan generalizarse a otras personas, edades o profesiones.

---

## 2. Planteamiento del Problema

En las discusiones cotidianas y en redes sociales sobre temas polarizantes (como el fútbol o la gestión institucional), suelen presentarse fallas comunes en el manejo de la información:

* **Datos de baja calidad (*Garbage Data*):** Uso de titulares sensacionalistas, videos recortados fuera de contexto y errores de fechas históricas.
* **Afirmaciones sin respaldo:** Dar por ciertas acusaciones graves (como corrupción o amaños) sin sentencias judiciales ni documentos oficiales que las prueben.
* **Sesgo de confirmación y selección:** Tendencia a aceptar solo los datos que confirman las creencias propias e ignorar las pruebas contrarias. **Este sesgo afecta a todos los participantes, incluido el analista.**
* **Desgaste de tiempo:** Discusiones repetitivas en las que se cambia de tema cuando faltan argumentos.

**Pregunta de investigación:**  
*¿Cómo puede una metodología básica de auditoría de datos mejorar la verificación de afirmaciones y reducir los sesgos cognitivos en un debate polarizado?*

---

## 3. Objetivos

### 3.1. Objetivo General
Diseñar una guía práctica de **auditoría de datos y análisis argumentativo** para verificar afirmaciones e identificar sesgos cognitivos en debates polarizados.

### 3.2. Objetivos Específicos
1. Aplicar un proceso básico de **limpieza y organización de datos (ETL)** a conversaciones informales para separar hechos comprobables de opiniones.
2. Elaborar una **matriz de verificación** que relacione cada afirmación con su respectiva fuente oficial de contraste.
3. Evaluar la calidad de las intervenciones mediante una **rúbrica sencilla (escala de 0 a 10)** aplicada tanto al interlocutor como al propio autor.
4. Establecer **reglas de cierre** para finalizar una discusión cuando deja de aportar datos útiles.

---

## 4. Metodología de Trabajo

En el desarrollo de software (ADSO), ningún sistema procesa datos sin validarlos primero. Este proyecto aplica esa misma lógica en cuatro pasos simples:

1. **Extracción (Recopilación):** Se toman las afirmaciones principales del debate y se registran en una tabla, manteniendo anonimizados a los participantes (**Analista** e **Interlocutor A**).
2. **Transformación (Limpieza):** Se filtran insultos, burlas, ataques personales (*Ad Hominem*) y cambios de tema para quedarse únicamente con los datos verificables.
3. **Validación (*Ground Truth*):** Cada dato se compara con fuentes primarias oficiales:
   * *Ámbito jurídico:* Notas oficiales del poder judicial y leyes vigentes.
   * *Ámbito deportivo:* Reglamentos oficiales (IFAB) y registros históricos verificados (FIFA).
4. **Dictamen:** Se clasifica cada afirmación como *Verificada, Falsa, Imprecisa* o *Sesgo de selección*.

### Reglas de imparcialidad del autor
* Aplicar exactamente los mismos criterios de evaluación a las afirmaciones propias y a las ajenas.
* Documentar obligatoriamente los errores propios cometidos durante el debate.
* Evaluar el dato (*"afirmación sin fuente"*), nunca descalificar a la persona (*"fanático"*, *"anti"*).

---

## 5. Caso de Estudio Exploratorio

> **Consideración ética:** Para respetar la privacidad y evitar conflictos personales, se omiten nombres reales y datos identificables.

### 5.1. Matriz de Verificación (Debate Deportivo y Jurídico)

| ID | Tema Auditado | Afirmación Examinada (Input) | Verificación del Analista (Query) | Fuente Oficial de Contraste | Resultado |
| :--- | :--- | :--- | :--- | :--- | :--- |
| **AUD-001** | **Tipicidad penal** | Se afirma que existe delito de cohecho y compra comprobada de árbitros. | La Audiencia de Barcelona dejó sin efecto la imputación por cohecho al concluir que Negreira no era funcionario público. La investigación sigue por otros delitos, pero no existe sentencia firme de compra arbitral. | CGPJ (24 de mayo de 2024) – Nota oficial Audiencia de Barcelona. | **Falso / Impreciso** |
| **AUD-002** | **Cronología histórica** | Se confunden fechas de mundiales pasados y se menciona una final perdida en el Mundial 2026. | Se revisan las fechas y resultados oficiales de las copas del mundo disputadas hasta noviembre de 2026. | Registros Históricos Oficiales FIFA (2026). | **Error de Datos** |
| **AUD-003** | **Reglamento técnico** | Se niegan faltas visibles en video y se omiten acontecimientos de partidos de ida. | Se revisa la eliminatoria completa bajo el reglamento vigente y se reconocen también jugadas puntuales favorables. | IFAB – *Laws of the Game 2026/27* (Reglas 5, 11 y 12). | **Sesgo de Selección** |
| **AUD-004** | **Gestión institucional** | Se mezclan trámites administrativos de inscripción con presuntos amaños arbitrales. | Se diferencia la gestión administrativa y contable del rendimiento deportivo en cancha. | Ley 39/2022, de 30 de diciembre, del Deporte (BOE). | **Cambio de Tema** |

### 5.2. Registro de Errores Propios del Analista
*Para mantener la objetividad, el autor registra aquí sus propias fallas detectadas durante la revisión:*

| ID | Afirmación o Conducta Propia | Qué estuvo mal | Corrección Aplicada |
| :--- | :--- | :--- | :--- |
| **AUT-001** | `[Escribir aquí un dato citado de memoria sin verificar primero]` | `[Falta de fuente inmediata]` | `[Se buscó el documento oficial y se aclaró el dato]` |
| **AUT-002** | `[Escribir aquí una respuesta con tono algo irónico]` | `[Reactividad emocional puntual]` | `[Se retomó el tono neutral centrado en los hechos]` |

---

## 6. Rúbrica de Evaluación (Escala de 0 a 10)

Para medir la calidad de las intervenciones se utiliza una escala simple donde **0–3 es Bajo**, **4–6 es Medio** y **7–10 es Alto**:

| Criterio | 0–3 (Bajo) | 4–6 (Medio) | 7–10 (Alto) |
| :--- | :--- | :--- | :--- |
| **Rigor Fáctico** | Afirma cosas sin fuentes ni pruebas. | Presenta algunas fuentes, pero mezcla suposiciones. | Respalda casi todas sus afirmaciones con fuentes oficiales. |
| **Autocrítica** | No acepta errores aunque vea pruebas. | Acepta errores solo tras mucha insistencia. | Reconoce y corrige errores propios de forma abierta. |
| **Coherencia Lógica** | Cambia de tema constantemente o se contradice. | Mantiene el tema con algunos desvíos. | Mantiene el hilo del debate sin contradicciones. |
| **Control Emocional** | Usa insultos, burlas o ataques personales. | Tono variable con momentos de molestia. | Mantiene un trato respetuoso en todo momento. |

### Tabla de Resultados (Para revisión de un tercero)
*Lo ideal es que un compañero o docente asigne estas notas revisando la conversación:*

| Criterio | Analista | Interlocutor A | Observaciones |
| :--- | :---: | :---: | :--- |
| Rigor Fáctico | `[ ]/10` | `[ ]/10` | `[Basado en la tabla 5.1]` |
| Autocrítica | `[ ]/10` | `[ ]/10` | `[Incluye la tabla 5.2]` |
| Coherencia Lógica | `[ ]/10` | `[ ]/10` | `[Completar]` |
| Control Emocional | `[ ]/10` | `[ ]/10` | `[Completar]` |
| **Promedio Final** | **`[ ]/10`** | **`[ ]/10`** | **Revisado por:** `[Nombre o rol]` |

---

## 7. Protocolo de Cierre de Debate

Cuando una discusión deja de aportar información nueva, se aplican tres reglas prácticas:

1. **Identificar el bucle improductivo:** Si ante un documento oficial o reglamento la respuesta es una burla o evasión repetida, el análisis ha terminado.
2. **Cierre ordenado (*Graceful Shutdown*):** Se finaliza la conversación de forma respetuosa sin necesidad de obligar al otro a dar la razón. La validez de un dato depende de la fuente, no de la aprobación del interlocutor.
3. **Enfoque productivo:** Redirigir el tiempo hacia el estudio, el desarrollo de software y proyectos académicos.

---

## 8. Conclusiones

1. Los sesgos cognitivos afectan a cualquier persona; aplicar una **metodología básica de verificación de datos** ayuda a separar los hechos reales de las opiniones emocionales.
2. Los conocimientos de **ADSO y Analítica de Datos** son útiles para organizar información cotidiana con orden y evidencia, siempre que el analista también evalúe sus propios errores.
3. El propósito de auditar un debate no es "ganar" una discusión, sino **comprobar los hechos con fuentes confiables y saber retirarse a tiempo** cuando el intercambio no es productivo.

---


<FollowUp>
Si quieres, puedes compartir **un par de ejemplos reales** de imprecisiones que hayas tenido en esos debates para ayudarte a redactar la **Tabla 5.2 (Errores Propios)** con el mismo tono académico.
</FollowUp>

## 9. Referencias (APA 7.ª Edición)

* Boletín Oficial del Estado. (2022). *Ley 39/2022, de 30 de diciembre, del Deporte*. BOE núm. 314. https://boe.es
* Consejo General del Poder Judicial. (2024, 24 de mayo). *La Audiencia de Barcelona desestima el delito de cohecho en el caso Negreira* [Nota de prensa]. Poder Judicial de España. https://poderjudicial.es
* Fédération Internationale de Football Association. (2026, 19 de julio). *Spain crowned FIFA World Cup 2026 champions in New York New Jersey*. https://fifa.com
