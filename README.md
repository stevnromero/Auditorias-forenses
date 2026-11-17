# PROYECTO DE INVESTIGACIÓN APLICADA
# AUDITORÍA DE DATOS Y PENSAMIENTO CRÍTICO FRENTE A SESGOS COGNITIVOS EN DEBATES POLARIZADOS

**Autor:** Steven  
**Formación:** Tecnólogo en Análisis y Desarrollo de Software (ADSO) – SENA | Analítica de Datos – UNAD  
**Fecha:** Noviembre de 2026  
**Área de aplicación:** Ciencia de Datos, Ingeniería de Sistemas, Calidad de Datos y Lógica Argumentativa  

---

## 1. Resumen Ejecutivo

El presente proyecto propone el diseño y aplicación de una metodología basada en principios de ingeniería de software y analítica de datos para auditar debates cotidianos, deportivos, sociales e institucionales caracterizados por la polarización, la desinformación y la presencia de sesgos cognitivos.

La propuesta utiliza procesos ETL (Extracción, Transformación y Carga), validación documental mediante fuentes primarias, matrices de trazabilidad e indicadores clave de desempeño (KPI). Su finalidad es evaluar la verificabilidad de las afirmaciones, identificar inconsistencias informativas y examinar la calidad argumentativa de los participantes, incluido el propio investigador.

El proyecto incorpora reglas de control metodológico para reducir la subjetividad del análisis: conservación de los registros originales, aplicación de criterios uniformes, documentación de errores propios y revisión independiente de los resultados.

**Nota de alcance:** El estudio tiene carácter exploratorio, descriptivo y aplicado. Sus resultados se limitan a los casos efectivamente examinados y no pretenden establecer relaciones causales ni generalizar conclusiones a poblaciones, edades o profesiones.

---

## 2. Planteamiento del Problema

En los entornos digitales y sociales actuales, numerosos debates presentan dificultades relacionadas con la calidad de la información y la evaluación de argumentos.

Entre los problemas identificados se encuentran:

- **Datos de baja calidad (*Garbage Data*):** utilización de titulares sensacionalistas, fragmentos audiovisuales fuera de contexto, información incompleta y anacronismos históricos.
- **Afirmaciones sin respaldo suficiente:** presentación de acusaciones graves, como corrupción, amaños o delitos, sin documentación que permita verificar su existencia o alcance.
- **Sesgo de confirmación y selección:** tendencia a favorecer información que respalda las creencias propias, omitiendo contexto o rechazando evidencias contrarias.
- **Inconsistencias argumentativas:** contradicciones, cambios injustificados de tema y utilización de argumentos que no responden directamente a la afirmación examinada.
- **Desgaste cognitivo:** consumo de tiempo y recursos mentales en intercambios que no producen información nueva ni permiten contrastar evidencias.

Estos problemas no son exclusivos de una persona o grupo. Pueden afectar a todos los participantes, incluido el investigador.

### Pregunta de investigación

¿Cómo puede una metodología de auditoría basada en principios de ingeniería de software y analítica de datos mejorar la verificabilidad de las afirmaciones y reducir la influencia de sesgos cognitivos en debates polarizados?

---

## 3. Objetivos

### 3.1. Objetivo General

Diseñar un marco metodológico de auditoría de datos y análisis argumentativo, basado en principios de ingeniería de software y analítica de datos, para identificar inconsistencias informativas, evaluar afirmaciones y reconocer posibles sesgos cognitivos en debates polarizados.

### 3.2. Objetivos Específicos

1. Aplicar procesos ETL (Extracción, Transformación y Carga) a conversaciones y registros digitales para separar hechos verificables, opiniones e interpretaciones.
2. Diseñar matrices de trazabilidad que permitan identificar el origen, la evidencia documental y el estado de cada afirmación auditada.
3. Construir indicadores clave de desempeño (KPI), mediante rúbricas explícitas, para evaluar el rigor fáctico, la autocrítica, la coherencia lógica y el control emocional observable.
4. Establecer mecanismos de revisión independiente y auditoría propia para reducir la subjetividad del investigador.
5. Implementar protocolos de cierre ordenado que permitan administrar el tiempo y los recursos cognitivos cuando un intercambio deja de ser productivo.

---

## 4. Marco Metodológico y Reglas Anti-Sesgo

En el desarrollo de software, los datos de entrada deben validarse antes de ser procesados. Este proyecto traslada ese principio al análisis del discurso mediante procedimientos de calidad, trazabilidad y verificación documental.

Como referencias conceptuales se consideran el modelo de calidad de datos ISO/IEC 25012 y la ontología de procedencia W3C PROV-O.

### 4.1. Fases del Proceso de Auditoría

**Fase 1. Extracción e ingesta**

- Recopilar las intervenciones que conforman el debate.
- Asignar un identificador único a cada registro.
- Registrar fecha, contexto y código anonimizado del participante.
- Conservar una copia íntegra del registro original.
- Evitar modificaciones que impidan reconstruir la información inicial.

**Fase 2. Transformación y clasificación**

- Separar afirmaciones verificables, opiniones e interpretaciones.
- Dividir afirmaciones compuestas en unidades de análisis independientes.
- Normalizar fechas, nombres de documentos y referencias.
- Identificar elementos comunicativos como sarcasmo, insultos, ironías, ataques personales o cambios de tema.
- Conservar el texto original y registrar las etiquetas de clasificación en campos separados.

**Criterio de integridad:** la limpieza ETL no debe eliminar información relevante del registro original. Los elementos comunicativos se clasifican y documentan, pero se conserva el contenido íntegro para permitir su posterior revisión.

**Fase 3. Validación documental (*Ground Truth*)**

Cada afirmación verificable se contrasta con fuentes pertinentes y, cuando sea posible, primarias.

Jerarquía orientativa de fuentes:

- **Ámbito jurídico:** resoluciones judiciales, legislación vigente, documentos oficiales y expedientes públicos disponibles.
- **Ámbito deportivo:** reglamentos oficiales de IFAB, FIFA y UEFA, actas de competición y registros estadísticos verificables.
- **Ámbito institucional:** informes oficiales, documentos administrativos y publicaciones de organismos competentes.
- **Ámbito histórico:** archivos institucionales y registros documentales contrastables.

Las fuentes secundarias pueden utilizarse como apoyo, pero no deben sustituir automáticamente la documentación primaria cuando esta se encuentre disponible.

**Fase 4. Evaluación de integridad y dictamen**

Cada afirmación se clasifica utilizando las siguientes categorías:

| Clasificación | Descripción |
|---|---|
| Verificada | La evidencia consultada respalda la afirmación en su contexto. |
| Falsa | La evidencia disponible contradice la afirmación. |
| Parcialmente cierta | Contiene elementos correctos, pero omite información relevante o presenta una conclusión incompleta. |
| No verificable | No se dispone de evidencia suficiente para confirmar o refutar la afirmación. |
| Desactualizada | La afirmación pudo ser válida anteriormente, pero no representa el estado documental actual. |
| Opinión | Expresa una valoración subjetiva que no puede verificarse como un hecho objetivo. |

La clasificación debe aplicarse a cada afirmación concreta, no a la persona que la formula.

### 4.2. Reglas Anti-Sesgo del Analista

Para reducir la subjetividad se establecen las siguientes reglas:

1. Aplicar exactamente los mismos criterios de evaluación a las afirmaciones propias y a las ajenas.
2. Registrar los errores propios detectados durante el proceso.
3. Diferenciar hechos, inferencias, hipótesis y opiniones.
4. Documentar las fuentes utilizadas y la fecha de consulta.
5. Someter los resultados a revisión independiente cuando sea posible.
6. Evitar etiquetas descalificativas sobre los participantes y diagnósticos psicológicos.
7. No confundir la falta de evidencia con una demostración de falsedad.
8. Actualizar los dictámenes cuando aparezca nueva documentación relevante.

---

## 5. Caso de Estudio Exploratorio

### Consideración ética

Para proteger la privacidad de los participantes, se omiten nombres reales, edades y datos identificables.

Se utilizan dos perfiles:

- **Analista:** autor del proyecto.
- **Interlocutor A:** participante anonimizado.

La unidad de análisis es cada afirmación individual que pueda ser examinada mediante criterios documentales o argumentativos.

### 5.1. Caso 1: Matriz de Trazabilidad (Debate Deportivo y Jurídico)

| ID | Variable auditada | Afirmación examinada | Verificación requerida | Fuente de contraste | Estado |
|---|---|---|---|---|---|
| AUD-001 | Tipicidad penal | Se afirma que existe delito de cohecho y compra comprobada de árbitros en el caso Negreira. | Separar la cuestión jurídica del cohecho de las demás líneas de investigación. Comprobar el alcance exacto de las resoluciones y distinguir una imputación de una sentencia firme. | Consejo General del Poder Judicial y documentación judicial correspondiente. | Parcialmente cierta / conclusión no acreditada, según el alcance de cada afirmación. |
| AUD-002 | Cronología histórica | Se confunden fechas de mundiales anteriores o se afirma incorrectamente el resultado de la final del Mundial 2026. | Contrastar fechas, resultados y registros oficiales de las competiciones disputadas. | Archivo histórico y registros oficiales FIFA. | Pendiente de documentar cada afirmación concreta. |
| AUD-003 | Reglamento técnico | Se niegan infracciones observables en video o se omiten acontecimientos de los partidos de ida y vuelta de una eliminatoria. | Examinar las jugadas concretas, las imágenes disponibles, el reglamento aplicable y el contexto completo de la eliminatoria. | IFAB, actas oficiales y registros audiovisuales verificables. | Pendiente de evidencia específica. |
| AUD-004 | Gestión institucional | Se mezclan litigios administrativos de inscripción de jugadores con presuntos amaños arbitrales. | Separar los procedimientos administrativos, la normativa deportiva y las afirmaciones relativas a decisiones arbitrales. | Ley 39/2022 y documentación institucional pertinente. | Posible confusión de asuntos; requiere analizar el argumento concreto. |

**Observación metodológica:** las categorías de esta matriz son provisionales. No constituyen una sentencia judicial ni un dictamen definitivo sobre la conducta de los participantes. Cada resultado debe sustentarse con una fuente concreta, una fecha y una referencia documental verificable.

#### Desarrollo de AUD-001: Caso Negreira

El análisis debe diferenciar, como mínimo, las siguientes cuestiones:

- La existencia y el alcance de los pagos investigados.
- La calificación jurídica de los hechos.
- La resolución judicial relacionada con el delito de cohecho.
- La continuidad o situación de las restantes líneas de investigación.
- La existencia o inexistencia de una sentencia firme sobre las acusaciones examinadas.

La resolución relativa al cohecho no debe interpretarse automáticamente como una declaración de falsedad de todas las demás acusaciones ni como prueba de una compra de árbitros.

**Fuente de consulta:** [Consejo General del Poder Judicial](https://www.poderjudicial.es/)

**Pendiente:** incorporar la referencia directa al auto judicial, su fecha, órgano emisor y fragmento relevante. También debe verificarse el estado procesal vigente en la fecha de cierre del proyecto.

#### Desarrollo de AUD-002: Cronología del Mundial 2026

La verificación debe realizarse mediante registros oficiales de FIFA.

Como dato de referencia, FIFA publicó el resultado de la final del Mundial 2026: España venció 1-0 a Argentina en la prórroga, el 19 de julio de 2026.

Fuente: [FIFA – España se proclama campeona de la Copa Mundial 2026](https://inside.fifa.com/es/organisation/news/espana-campeona-mundial-2026-nueva-york-nueva-jersey)

Este registro permite contrastar afirmaciones sobre el resultado de la final, pero no sustituye la revisión de otras fechas o partidos que se incorporen a la muestra.

#### Desarrollo de AUD-003: Reglamento técnico

Para analizar una jugada se deben registrar:

- Partido y competición.
- Fecha del encuentro.
- Minuto de la jugada.
- Regla aplicable.
- Evidencia audiovisual disponible.
- Interpretación del reglamento.
- Limitaciones de la evidencia.
- Conclusión y grado de certeza.

Fuente: [IFAB – Reglas de Juego 2026/27](https://www.theifab.com/es/laws-of-the-game-documents/)

No se debe declarar una infracción únicamente porque una imagen aislada parezca mostrarla. Es necesario examinar el contexto y la regla aplicable.

#### Desarrollo de AUD-004: Gestión institucional

La Ley 39/2022, de 30 de diciembre, del Deporte, constituye una referencia normativa para el análisis del marco deportivo español.

Fuente: [BOE – Ley 39/2022, de 30 de diciembre, del Deporte](https://www.boe.es/buscar/act.php?id=BOE-A-2022-24430)

La utilización de esta norma debe limitarse a las disposiciones pertinentes para el asunto examinado. Una controversia administrativa no demuestra por sí misma la existencia de una irregularidad arbitral.

### 5.2. Registro Obligatorio de Errores Propios del Analista

Para garantizar la honestidad intelectual, el investigador debe documentar sus propios errores cuando sean identificados durante la revisión.

| ID | Afirmación o conducta propia | Error identificado | Evidencia de contraste | Corrección aplicada |
|---|---|---|---|---|
| AUT-001 | [Registrar una afirmación propia real.] | [Describir la imprecisión, contradicción o falta de fuente.] | [Documento o enlace verificable.] | [Explicar la rectificación realizada.] |
| AUT-002 | [Registrar un segundo error propio real.] | [Describir el error.] | [Documento o enlace verificable.] | [Explicar la corrección.] |

**Importante:** esta tabla debe completarse con errores reales detectados. No deben inventarse errores para aparentar autocrítica ni dejarse registros ficticios como resultados del estudio.

Si durante la auditoría no se identifica un error propio, debe documentarse el procedimiento de revisión realizado y dejar constancia de que no se encontró uno dentro del material examinado.

### 5.3. Ampliación de la Muestra (Trabajo en Curso)

Para fortalecer el estudio se propone ampliar la muestra:

- **Caso 2:** análisis de un debate sobre gestión institucional o política, utilizando documentos oficiales y fuentes verificables.
- **Caso 3:** análisis de un debate con un segundo interlocutor anonimizado, con el objetivo de examinar la aplicación uniforme de los criterios.

Estos casos se consideran pendientes hasta que se recopilen y documenten las evidencias correspondientes.

---

## 6. Indicadores Clave de Desempeño (KPI) y Rúbrica

Se propone una escala cuantitativa de 0 a 10 para evaluar cuatro dimensiones de la calidad argumentativa.

| Rango | Nivel |
|---|---|
| 0–3 | Bajo |
| 4–6 | Medio |
| 7–8 | Alto |
| 9–10 | Excelente |

### 6.1. Rúbrica de Evaluación Argumentativa

| KPI | Ponderación | 0–3: Bajo | 4–6: Medio | 7–10: Alto / Excelente |
|---|---:|---|---|---|
| Rigor fáctico y legal | 35 % | Predominan afirmaciones sin fuentes o sustentadas en rumores. | Existe respaldo parcial, pero se mezclan datos verificados y suposiciones. | Las afirmaciones verificables se respaldan con fuentes pertinentes y contextualizadas. |
| Autocrítica | 25 % | No reconoce errores propios ante evidencias suficientes. | Reconoce errores parcialmente o después de recibir observaciones. | Reconoce, acepta y documenta errores propios de manera transparente. |
| Coherencia lógica | 25 % | Presenta contradicciones frecuentes y argumentos que no responden al tema. | Mantiene el hilo conductor, aunque presenta desvíos ocasionales. | Mantiene un razonamiento estructurado y consistente con el objeto del debate. |
| Control emocional observable | 15 % | Recurre frecuentemente a insultos o ataques personales. | Mantiene un tono variable con episodios puntuales de reactividad. | Mantiene una comunicación respetuosa incluso ante desacuerdos. |

**Nota:** el control emocional se evalúa exclusivamente a partir de conductas comunicativas observables. No se pretende diagnosticar estados psicológicos ni atribuir características personales.

### 6.1.1. Criterios para Asignar las Puntuaciones

Para mejorar la reproducibilidad de la evaluación se propone el siguiente procedimiento:

1. Identificar las afirmaciones y conductas relevantes del participante.
2. Registrar fragmentos concretos que respalden la evaluación.
3. Contrastar las afirmaciones verificables con las fuentes disponibles.
4. Aplicar los descriptores de la rúbrica.
5. Asignar una puntuación de 0 a 10 por dimensión.
6. Justificar cada puntuación mediante evidencia.
7. Solicitar una segunda evaluación independiente cuando sea posible.
8. Registrar y resolver las diferencias de interpretación.

Una puntuación sin evidencia documental o fragmentos observables debe considerarse provisional.

### 6.1.2. Fórmula del Índice de Calidad Argumentativa (IA)

El índice propuesto se calcula mediante una suma ponderada:

```text
IA = (RF * 0.35) + (AC * 0.25) + (CL * 0.25) + (CE * 0.15)
```

Donde:

- **RF:** Rigor fáctico y legal.
- **AC:** Autocrítica.
- **CL:** Coherencia lógica.
- **CE:** Control emocional observable.

El resultado se expresa en una escala de 0 a 10.

**Ejemplo ilustrativo de cálculo (no corresponde a resultados reales del estudio):**

```text
RF = 8
AC = 7
CL = 9
CE = 8

IA = (8 * 0.35) + (7 * 0.25) + (9 * 0.25) + (8 * 0.15)

IA = 2.80 + 1.75 + 2.25 + 1.20

IA = 8.00
```

Este ejemplo muestra el funcionamiento matemático de la fórmula. No representa una calificación del Analista ni del Interlocutor A.

### 6.2. Matriz de Resultados (Evaluación Externa)

La calificación definitiva debe ser asignada o validada por un evaluador independiente, con el propósito de reducir el conflicto de interés derivado de que el autor evalúe su propia participación.

| KPI | Analista | Interlocutor A | Evidencia documental |
|---|---:|---:|---|
| Rigor fáctico y legal (35 %) | Pendiente | Pendiente | Referencias de la matriz 5.1. |
| Autocrítica (25 %) | Pendiente | Pendiente | Registros documentados en la tabla 5.2. |
| Coherencia lógica (25 %) | Pendiente | Pendiente | Fragmentos de las intervenciones examinadas. |
| Control emocional (15 %) | Pendiente | Pendiente | Conductas comunicativas observables. |
| Índice consolidado (IA) | Pendiente | Pendiente | Cálculo basado en las puntuaciones justificadas. |

**Evaluador independiente:** pendiente de designación.  
**Fecha de evaluación:** pendiente.

No se asignan puntuaciones definitivas hasta contar con evidencias suficientes y una evaluación documentada.

---

## 7. Arquitectura Tecnológica Propuesta

Para automatizar el almacenamiento, la trazabilidad y el cálculo de métricas, se propone una implementación ligera con herramientas de análisis de datos y desarrollo de software.

### 7.1. Stack Tecnológico

| Tecnología | Aplicación en el proyecto |
|---|---|
| Python | Lenguaje principal para implementar la solución. |
| Pandas | Limpieza, transformación y manipulación de datos. |
| NumPy | Operaciones numéricas y cálculo de indicadores. |
| SQLite | Almacenamiento relacional local. |
| Jupyter Notebook | Documentación, análisis y ejecución reproducible. |
| Matplotlib | Visualización de resultados y métricas. |

### 7.2. Pipeline de Procesamiento

```text
┌───────────────────────────────────────┐
│       Conversación / Registro Bruto   │
└───────────────────┬───────────────────┘
                    │
                    ▼
┌───────────────────────────────────────┐
│ Módulo 1: Ingesta y Respaldo Original │
│              SQLite                  │
└───────────────────┬───────────────────┘
                    │
                    ▼
┌───────────────────────────────────────┐
│ Módulo 2: Clasificación y ETL         │
│              Pandas                   │
└───────────────────┬───────────────────┘
                    │
                    ▼
┌───────────────────────────────────────┐
│ Módulo 3: Validación Documental       │
│        Contraste de fuentes           │
└───────────────────┬───────────────────┘
                    │
                    ▼
┌───────────────────────────────────────┐
│ Módulo 4: Clasificación y Evaluación  │
│       Rúbrica / Evaluador             │
└───────────────────┬───────────────────┘
                    │
                    ▼
┌───────────────────────────────────────┐
│ Módulo 5: Cálculo de Indicadores      │
│           NumPy                       │
└───────────────────┬───────────────────┘
                    │
                    ▼
┌───────────────────────────────────────┐
│       Informe de Auditoría            │
│       Resultados y Visualización      │
└───────────────────────────────────────┘
```

### 7.3. Esquema de Base de Datos

Se propone una tabla principal denominada `auditoria_afirmaciones`.

| Campo | Tipo de dato | Descripción |
|---|---|---|
| id_auditoria | INTEGER PRIMARY KEY | Identificador único del registro. |
| participante | TEXT | Código anonimizado del participante. |
| afirmacion_original | TEXT | Texto literal de la afirmación. |
| fecha_registro | DATE | Fecha de la intervención. |
| contexto | TEXT | Contexto en el que se produjo la afirmación. |
| fuente_contraste | TEXT | Enlace o referencia documental. |
| fecha_consulta | DATE | Fecha en la que se consultó la fuente. |
| clasificacion | TEXT | Estado de verificación de la afirmación. |
| observaciones | TEXT | Notas del proceso de auditoría. |
| evaluador | TEXT | Identificador del evaluador o revisor. |

**Criterio de almacenamiento:** el registro original debe conservarse sin modificaciones. Las versiones normalizadas, etiquetas y resultados de evaluación deben almacenarse separadamente para mantener la trazabilidad.

### 7.4. Organización Propuesta del Repositorio

```text
auditoria-datos-pensamiento-critico/
│
├── README.md
│
├── data/
│   ├── originales/
│   └── procesados/
│
├── src/
│   ├── auditoria.py
│   ├── etl.py
│   ├── validacion.py
│   └── indicadores.py
│
├── notebooks/
│   └── analisis_exploratorio.ipynb
│
├── docs/
│   ├── metodologia.md
│   └── referencias.md
│
├── reports/
│   └── resultados/
│
├── tests/
│   └── test_indicadores.py
│
└── requirements.txt
```

Esta estructura es una propuesta de organización. Los directorios y archivos deben incorporarse cuando sus respectivos componentes estén implementados.

---

## 8. Protocolo de Higiene Cognitiva y Cierre de Sesión

Todo sistema informático requiere límites para evitar procesos que consuman recursos sin producir resultados útiles. En el análisis de debates se propone aplicar cuatro reglas:

### 8.1. Detección de Bucle Improductivo (*Infinite Loop*)

Cuando una discusión repite argumentos sin aportar evidencia nueva, se identifica una posible situación de intercambio improductivo.

La repetición de una afirmación no demuestra que sea verdadera o falsa. Se debe evaluar si aparecen datos nuevos, fuentes pertinentes o argumentos que modifiquen el análisis.

### 8.2. Cierre Ordenado (*Graceful Shutdown*)

El analista puede finalizar una interacción cuando no se producen avances verificables.

El cierre no exige que todos los participantes alcancen un consenso. La validez de una afirmación debe depender de la evidencia disponible y no de la aprobación interpersonal.

### 8.3. Verificación Previa al Cierre

Antes de finalizar, el analista debe revisar:

- Si aplicó los mismos criterios a todas las partes.
- Si verificó sus propias afirmaciones.
- Si confundió una opinión con un hecho.
- Si omitió información relevante.
- Si respondió a los argumentos reales y no a interpretaciones distorsionadas.
- Si documentó correctamente las fuentes consultadas.

### 8.4. Redirección Productiva

El tiempo recuperado puede destinarse a actividades de formación y desarrollo profesional, como:

- Desarrollo de software.
- Gestión de bases de datos.
- Análisis y visualización de datos.
- Automatización de procesos.
- Formación académica.

---

## 9. Limitaciones y Conclusiones

### 9.1. Limitaciones

**Tamaño de la muestra:** el estudio tiene carácter exploratorio y utiliza una cantidad reducida de casos. Por tanto, sus hallazgos no son estadísticamente generalizables.

**Participación del autor:** el investigador también interviene en los debates que analiza. Esto genera un posible sesgo de interpretación, que se busca mitigar mediante el registro de errores propios y la revisión independiente.

**Disponibilidad documental:** algunas afirmaciones pueden carecer de fuentes primarias accesibles o de evidencia suficiente para emitir un dictamen definitivo.

**Dependencia temporal:** las afirmaciones jurídicas, deportivas e institucionales pueden cambiar con la publicación de nuevas resoluciones, reglamentos o documentos oficiales.

**Subjetividad de la rúbrica:** aunque se establecen criterios explícitos, la evaluación de la coherencia lógica y del control emocional puede presentar diferencias entre evaluadores.

**Alcance tecnológico:** la arquitectura descrita constituye una propuesta de implementación. Su funcionamiento debe validarse mediante pruebas técnicas antes de considerarse un sistema operativo terminado.

### 9.2. Conclusiones

1. Los sesgos cognitivos y las deficiencias en la calidad de la información pueden afectar a cualquier participante de un debate. Por ello, la auditoría debe aplicar criterios uniformes y permitir la revisión de las afirmaciones propias.

2. Los principios de calidad de datos, trazabilidad y procesos ETL pueden trasladarse al análisis del discurso para organizar información, identificar inconsistencias y mejorar la verificabilidad de las afirmaciones.

3. La formación en ADSO y Analítica de Datos proporciona herramientas prácticas para diseñar procesos de validación, estructuras de almacenamiento, indicadores y procedimientos reproducibles.

4. La conservación de los registros originales y la documentación de las transformaciones permiten mantener la integridad y trazabilidad del análisis.

5. La evaluación mediante KPI puede aportar una estructura sistemática para examinar la calidad argumentativa, siempre que las puntuaciones estén justificadas mediante evidencias y criterios reproducibles.

6. El objetivo de una auditoría argumentativa no es ganar una discusión interpersonal, sino evaluar afirmaciones con rigor, reconocer errores y establecer conclusiones proporcionales a la evidencia disponible.

### 9.3. Recomendaciones y Trabajo Futuro

- Ampliar la muestra con nuevos casos deportivos, jurídicos e institucionales.
- Implementar el sistema de almacenamiento y procesamiento en Python y SQLite.
- Incorporar pruebas automatizadas para validar los cálculos de los KPI.
- Desarrollar visualizaciones que permitan comparar resultados.
- Establecer un protocolo de evaluación entre dos o más revisores.
- Evaluar la concordancia entre evaluadores mediante indicadores apropiados, como el coeficiente Kappa de Cohen cuando se cumplan sus condiciones de aplicación.
- Actualizar las referencias documentales cuando cambie el estado de una afirmación.
- Publicar únicamente resultados que puedan reproducirse a partir de los datos y fuentes disponibles.

---

## 10. Referencias Bibliográficas (APA 7.ª Edición)

Boletín Oficial del Estado. (2022). *Ley 39/2022, de 30 de diciembre, del Deporte*. BOE núm. 314, de 31 de diciembre de 2022.  
https://www.boe.es/buscar/act.php?id=BOE-A-2022-24430

Consejo General del Poder Judicial. (2024). *Documentación institucional sobre la resolución de la Audiencia Provincial de Barcelona relativa al delito de cohecho en el caso Negreira*. Poder Judicial de España.  
https://www.poderjudicial.es/

Fédération Internationale de Football Association. (2026, 19 de julio). *España se proclama campeona de la Copa Mundial de la FIFA 2026™ en Nueva York Nueva Jersey*.  
https://inside.fifa.com/es/organisation/news/espana-campeona-mundial-2026-nueva-york-nueva-jersey

International Football Association Board. (2026). *Reglas de Juego 2026/27*.  
https://www.theifab.com/es/laws-of-the-game-documents/

International Organization for Standardization. (2008). *ISO/IEC 25012:2008: Software engineering — Software product Quality Requirements and Evaluation (SQuaRE) — Data quality model*. ISO.

Kahneman, D. (2011). *Thinking, fast and slow*. Farrar, Straus and Giroux.

Tversky, A., & Kahneman, D. (1974). Judgment under uncertainty: Heuristics and biases. *Science, 185*(4157), 1124–1131.  
https://doi.org/10.1126/science.185.4157.1124

World Wide Web Consortium. (2013). *PROV-O: The PROV Ontology*.  
https://www.w3.org/TR/prov-o/

---

## Anexo A. Criterios Mínimos de Auditoría

Cada afirmación incorporada al sistema debe contar, cuando corresponda, con los siguientes elementos:

| Elemento | Requisito |
|---|---|
| Identificador | Código único de auditoría. |
| Participante | Código anonimizado. |
| Texto original | Conservación literal de la afirmación. |
| Contexto | Información necesaria para interpretar el contenido. |
| Fuente | Documento o referencia utilizada para contrastar. |
| Fecha de consulta | Fecha de verificación documental. |
| Clasificación | Estado asignado a la afirmación. |
| Justificación | Explicación del dictamen. |
| Evaluador | Responsable de la revisión. |
| Estado de revisión | Pendiente, revisado o validado. |

## Anexo B. Principios de Integridad del Proyecto

1. No inventar evidencias, resultados ni puntuaciones.
2. No presentar hipótesis como hechos comprobados.
3. No confundir una investigación judicial con una sentencia condenatoria.
4. No eliminar registros originales durante el procesamiento.
5. No utilizar la rúbrica para descalificar personas.
6. No ocultar errores propios.
7. No emitir conclusiones más amplias que las permitidas por la muestra.
8. Mantener actualizadas las referencias documentales.

## Anexo C. Estado de Desarrollo del Proyecto

| Componente | Estado |
|---|---|
| Planteamiento del problema | Definido |
| Objetivos | Definidos |
| Marco metodológico | Propuesto |
| Reglas anti-sesgo | Definidas |
| Matriz de trazabilidad | Estructurada; requiere completar evidencias |
| Registro de errores propios | Pendiente de completar con datos reales |
| Casos adicionales | Pendientes de análisis |
| Rúbrica de KPI | Diseñada |
| Evaluación independiente | Pendiente |
| Arquitectura tecnológica | Diseñada como propuesta |
| Implementación Python y SQLite | Pendiente de desarrollo y pruebas |
| Resultados finales | Pendientes de obtención |

---

**Principio central del proyecto:** una auditoría rigurosa no busca confirmar las creencias del investigador, sino someter cada afirmación —incluidas las propias— a criterios de evidencia, trazabilidad, consistencia y revisión.

