# PROYECTO ACADÉMICO: AUDITORÍA DE DATOS Y PENSAMIENTO CRÍTICO FRENTE A SESGOS COGNITIVOS EN DEBATES POLARIZADOS

**Autor:** Steven Romero
**Formación:** Tecnólogo en Análisis y Desarrollo de Software (ADSO) – SENA | Analítica de Datos – UNAD (Primer Semestre)  
**Fecha:** Noviembre de 2026  
**Área de aplicación:** Calidad de Datos, Analítica Básica y Lógica Argumentativa  

---

## 1. Resumen Ejecutivo

Este proyecto propone una metodología básica basada en **principios de calidad de datos y análisis de información** para evaluar debates cotidianos y deportivos marcados por la polarización. 

Mediante la limpieza de información irrelevante (*Garbage Data*), la consulta de fuentes oficiales y el uso de una tabla de verificación con conteo de frecuencias, se examina la validez de las afirmaciones de cada participante, **incluido el propio autor**, utilizando criterios claros, objetivos y verificables.

> **Nota de alcance y muestra ($N$):** Este es un estudio de caso exploratorio de carácter cualitativo-descriptivo con un tamaño de muestra $N = 1$ (un intercambio bilateral). Sus resultados describen únicamente el caso revisado y no buscan generalizarse estadísticamente a otras poblaciones.

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
2. Elaborar una **matriz de verificación** que relacione cada afirmación con su respectiva fuente oficial de contraste (*Ground Truth*).
3. Evaluar la calidad de las intervenciones mediante una **matriz de frecuencias y niveles de desempeño** aplicada tanto al interlocutor como al propio autor, evitando asignaciones numéricas subjetivas.
4. Establecer **reglas de cierre** (*Graceful Shutdown*) para finalizar una discusión cuando deja de aportar datos útiles.

---

## 4. Metodología de Trabajo

En el desarrollo de software (ADSO), ningún sistema procesa datos sin validarlos primero. Este proyecto aplica esa misma lógica en cuatro pasos simples:

1. **Extracción (Recopilación):** Se toman las afirmaciones principales del debate y se registran en una tabla, manteniendo anonimizados a los participantes (**Analista** e **Interlocutor A**).
2. **Transformación (Limpieza):** Se filtran insultos, burlas, ataques personales (*Ad Hominem*) y cambios de tema para quedarse únicamente con los datos verificables.
3. **Validación (*Ground Truth*):** Cada dato se compara con fuentes primarias oficiales:
   * *Ámbito jurídico:* Notas oficiales del poder judicial y leyes vigentes.
   * *Ámbito deportivo:* Reglamentos oficiales (IFAB) y registros históricos verificados (FIFA).
4. **Dictamen y Conteo de Frecuencias:** Se clasifica cada afirmación (*Verificada, Falsa, Imprecisa* o *Sesgo de selección*) y se contabilizan los eventos observables para reducir la subjetividad del evaluador.

### Reglas de imparcialidad del autor
* Aplicar exactamente los mismos criterios de evaluación a las afirmaciones propias y a las ajenas.
* Documentar obligatoriamente los errores propios cometidos durante el debate.
* Evaluar el dato (*"afirmación sin fuente"*), nunca descalificar a la persona (*"fanático"*, *"anti"*).

---

## 5. Caso de Estudio Exploratorio ($N = 1$)

> **Consideración ética:** Para respetar la privacidad y evitar conflictos personales, se omiten nombres reales y datos identificables. Se analizan las intervenciones registradas entre el **Analista** (autor del proyecto) y el **Interlocutor A**.

### 5.1. Matriz de Verificación (Debate Deportivo y Jurídico)

| ID | Tema Auditado | Afirmación Examinada (Input) | Verificación del Analista (Query) | Fuente Oficial de Contraste | Resultado |
| :--- | :--- | :--- | :--- | :--- | :--- |
| **AUD-001** | **Tipicidad penal** | Se afirma que existe delito de cohecho y compra comprobada de árbitros. | La Audiencia de Barcelona dejó sin efecto la imputación por cohecho al concluir que Negreira no era funcionario público. La investigación sigue por otros delitos, pero no existe sentencia firme ni transferencias comprobadas a árbitros. | CGPJ (24 de mayo de 2024) – Nota oficial Audiencia de Barcelona. | **Falso / Impreciso** |
| **AUD-002** | **Cronología histórica** | Se confunde el Mundial 1982 con 1986, se afirman 6 penales en Qatar 2022 y se cita una final perdida en el Mundial 2026. | Se revisan las fechas y estadísticas oficiales: el partido ante Inglaterra ocurrió en México 1986, en Qatar 2022 fueron 5 penales y la final del Mundial 2026 la ganó España. | Registros Históricos Oficiales FIFA (2026). | **Error de Datos** |
| **AUD-003** | **Reglamento técnico** | Se niegan infracciones visibles en video (planchazo y simulación) y se omiten acontecimientos de partidos de ida. | Se revisan las eliminatorias completas bajo el reglamento vigente (expulsiones omitidas, ley de la ventaja) y se admiten también jugadas puntuales favorables al equipo propio. | IFAB – *Laws of the Game 2026/27* (Reglas 5, 11 y 12). | **Sesgo de Selección** |
| **AUD-004** | **Gestión institucional** | Se mezclan trámites administrativos de inscripción de jugadores con presuntos amaños arbitrales. | Se diferencia la gestión administrativa y los plazos de prescripción deportiva del rendimiento en cancha. | Ley 39/2022, de 30 de diciembre, del Deporte (BOE). | **Cambio de Tema** |

### 5.2. Registro de Errores Propios del Analista

*Para mantener la objetividad y mitigar el sesgo del observador, el autor registra aquí sus propias fallas detectadas durante la revisión de los registros:*

| ID | Afirmación o Conducta Propia | Qué estuvo mal | Corrección Aplicada |
| :--- | :--- | :--- | :--- |
| **AUT-001** | Uso de adjetivos descalificativos en el intercambio (*"cínico"*, *"incrédulo y abominable"*, *"ardido"*). | Incumplimiento de la regla de control emocional y ataque *Ad Hominem* leve bajo provocación. | Se reconoció la reactividad, se retomó el tono amistoso y se cerró la conversación con respeto. |
| **AUT-002** | Afirmar porcentajes exactos de justicia arbitral (*"perjudicados al 80%"*, *"beneficiados el 85%"*). | Presentar apreciaciones o percepciones personales como si fueran métricas estadísticas oficiales. | Se aclaró en el análisis que son estimaciones subjetivas sobre el desarrollo del partido, no datos oficiales. |
| **AUT-003** | Proponer una apuesta monetaria (*"¿cuánto quieres apostar?"*) para resolver la discusión sobre una sentencia futura. | Desviación del método científico; una apuesta no valida ni refuta un hecho jurídico. | Se descartó la apuesta y se aplicó el protocolo de cierre ordenado (*graceful shutdown*). |

---

## 6. Evaluación Objetiva por Frecuencia y Niveles

Para evitar asignar calificaciones numéricas arbitrarias a conductas humanas, se emplea una **matriz de conteo de eventos observables** acompañada de niveles cualitativos definidos (**Bajo, Medio, Alto**):

| Criterio | Nivel Bajo | Nivel Medio | Nivel Alto |
| :--- | :--- | :--- | :--- |
| **Rigor Fáctico** | 0 fuentes oficiales citadas; predominan suposiciones. | Cita fuentes oficiales, pero incluye al menos 1 dato no verificado. | Respalda sus afirmaciones con fuentes oficiales verificables sin datos falsos. |
| **Autocrítica** | 0 errores propios reconocidos frente a evidencia contraria. | Reconoce errores propios solo tras insistencia o revisión posterior. | Reconoce y corrige errores propios de forma abierta durante el intercambio. |
| **Coherencia Lógica** | Presenta 2 o más cambios de tema o falacias de distracción. | Presenta 1 desviación temática o argumento no científico. | Mantiene el hilo conductor sin desviaciones lógicas. |
| **Control Emocional** | Presenta 3 o más ataques personales, burlas o descalificaciones. | Presenta entre 1 y 2 descalificaciones o momentos de reactividad. | Mantiene un trato respetuoso y neutral en el 100% de las intervenciones. |

### 6.1. Matriz de Resultados Aplicada

| Criterio | Analista (Frecuencia / Nivel) | Interlocutor A (Frecuencia / Nivel) | Evidencia Documentada en el Registro |
| :--- | :---: | :---: | :--- |
| **Rigor Fáctico** | **Nivel Medio-Alto**<br>*(4 fuentes oficiales / 1 dato subjetivo)* | **Nivel Bajo**<br>*(0 fuentes oficiales / 4 errores fácticos)* | **Analista:** Cita CGPJ, FIFA, IFAB y BOE con precisión; se penaliza el uso de porcentajes subjetivos (AUT-002).<br>**Interlocutor A:** Repite afirmaciones falsas o anacrónicas (AUD-001, AUD-002) sin aportar documentos. |
| **Autocrítica** | **Nivel Medio-Alto**<br>*(3 errores propios documentados)* | **Nivel Bajo**<br>*(0 errores reconocidos)* | **Analista:** Admite fallas administrativas de su club y errores arbitrales a favor, además de documentar sus fallas en la Tabla 5.2.<br>**Interlocutor A:** No reconoce ningún error factual ni arbitral frente a evidencia visual. |
| **Coherencia Lógica** | **Nivel Medio**<br>*(1 desviación lógica)* | **Nivel Bajo**<br>*(Múltiples cambios de tema)* | **Analista:** Separa correctamente los despachos de la cancha; se penaliza proponer una apuesta económica (AUT-003).<br>**Interlocutor A:** Cambia de tema constantemente (AUD-004) cuando se refutan sus datos. |
| **Control Emocional** | **Nivel Medio**<br>*(1 episodio de reactividad)* | **Nivel Bajo**<br>*(Recurrencia constante)* | **Analista:** Busca la conciliación en varios tramos, pero pierde la compostura usando adjetivos descalificativos (AUT-001).<br>**Interlocutor A:** Recurre con frecuencia a burlas, sarcasmos y descalificaciones personales. |

---

## 7. Protocolo de Cierre de Debate

Cuando una discusión deja de aportar información nueva, se aplican tres reglas prácticas:

1. **Identificar el bucle improductivo:** Si ante un documento oficial o reglamento la respuesta es una burla o evasión repetida, el análisis ha terminado.
2. **Cierre ordenado (*Graceful Shutdown*):** Se finaliza la conversación de forma respetuosa sin necesidad de obligar al otro a dar la razón. La validez de un dato depende de la fuente, no de la aprobación del interlocutor.
3. **Enfoque productivo:** Redirigir el tiempo hacia el estudio, el desarrollo de software y proyectos académicos.

---

## 8. Conclusiones y Trabajo Futuro

### 8.1. Conclusiones del Estudio
1. Los sesgos cognitivos afectan a cualquier persona; aplicar una **metodología básica de verificación de datos** ayuda a separar los hechos reales de las opiniones emocionales.
2. Reemplazar calificaciones numéricas arbitrarias por **conteos de frecuencias observables** reduce la subjetividad del analista al evaluar conversaciones.
3. El propósito de auditar un debate no es "ganar" una discusión, sino **comprobar los hechos con fuentes confiables y saber retirarse a tiempo** cuando el intercambio no es productivo.

### 8.2. Escalabilidad del Proyecto (Trabajo Futuro)
Dado que este trabajo corresponde a una etapa inicial de formación (Primer Semestre) y opera sobre una muestra unitaria ($N=1$), se proyectan tres fases de evolución técnica conforme avance la formación en **ADSO y Analítica de Datos**:
* **Fase 1 (Ampliación de Muestra):** Recolectar un conjunto de datos (*dataset*) más amplio ($N \ge 30$) a partir de hilos públicos anonimizados para identificar patrones recurrentes de desinformación.
* **Fase 2 (Automatización ETL):** Implementar scripts básicos en **Python** para automatizar la limpieza de ruido textual (eliminación de signos, *stopwords* y detección de palabras clave).
* **Fase 3 (Almacenamiento y Visualización):** Estructurar los registros auditados en una base de datos relacional (**SQL**) y generar tableros de control para visualizar la frecuencia de cada tipo de sesgo.

---

## 9. Referencias (APA 7.ª Edición)

* Boletín Oficial del Estado. (2022). *Ley 39/2022, de 30 de diciembre, del Deporte*. BOE núm. 314. https://boe.es
* Consejo General del Poder Judicial. (2024, 24 de mayo). *La Audiencia de Barcelona desestima el delito de cohecho en el caso Negreira* [Nota de prensa]. Poder Judicial de España. https://poderjudicial.es
* Fédération Internationale de Football Association. (2026, 19 de julio). *Spain crowned FIFA World Cup 2026 champions in New York New Jersey*. https://fifa.com
* International Football Association Board. (2026). *Laws of the Game 2026/27*. https://theifab.com
* Kahneman, D. (2011). *Thinking, Fast and Slow*. Farrar, Straus and Giroux.
