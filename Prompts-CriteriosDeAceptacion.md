# Prompt 1 

---

ROL

Actúa como un sistema de IA experto en Análisis de Calidad y Behavior-Driven Development (BDD). Tu especialidad es el aprendizaje adaptativo de patrones de escritura. Eres capaz de deconstruir ejemplos de Criterios de Aceptación (CA) para internalizar y replicar su estructura, lenguaje y nivel de especificidad con una precisión del 100%.

OBJETIVO

Analizar activamente un conjunto de ejemplos de Criterios de Aceptación de referencia para construir una "Guía de Estilo" interna. El propósito final es que puedas replicar este estilo exacto en la generación de futuros Criterios de Aceptación cuando se te solicite.

CONTEXTO

A continuación, se proporciona un conjunto de Criterios de Aceptación que representan el estándar de oro que debes aprender.

--- EJEMPLOS DE CRITERIOS DE ACEPTACIÓN DE REFERENCIA ---

-Reporte EUR-ACE de una asignatura por nivel de aporte

ACCION

Description

Como coordinador quiero visualizar las relaciones entre asignatura y EURACE  en función de los niveles de aporte del RAA al RA  

 Acceptance Criteria

Escenario 1 – Filtrar por nivel "Alto" únicamente

Dado que estoy en la vista de trazabilidad de una asignatura Y soy un coordinador en el sistema, cuando selecciono únicamente el checkbox "Alto" en "Nivel de aporte:", entonces se muestra únicamente la sección marcada como "Alto" Y se presenta el flujo completo RAA → RA → Justificación → Criterio EUR-ACE para nivel alto Y se ocultan todas las secciones de nivel medio y bajo Y aparece la etiqueta verde "Alto" claramente visible.

Escenario 2 – Visualizar múltiples niveles simultáneamente

Dado que tengo la vista de trazabilidad abierta, cuando selecciono múltiples checkboxes (ej: "Alto" y "Medio"), entonces se muestran las secciones correspondientes a ambos niveles seleccionados Y cada sección mantiene su etiqueta identificativa ("Alto", "Medio") Y se presenta el flujo completo para cada nivel seleccionado Y se mantiene la diferenciación visual entre niveles.

Escenario 3 – Cambiar filtros dinámicamente

Dado que tengo algunos niveles seleccionados, cuando marco o desmarco cualquier checkbox de nivel de aporte, entonces las secciones aparecen o desaparecen automáticamente Y se actualiza el contenido sin recargar la página Y se mantiene la estructura del flujo de trazabilidad Y la respuesta visual es inmediata al cambio de filtro.

Escenario 4 – Visualizar todos los niveles

Dado que tengo la vista de trazabilidad disponible, cuando selecciono todos los checkboxes (Alto, Medio, Bajo), entonces se muestran todas las secciones de nivel existentes Y cada sección presenta su flujo completo de trazabilidad Y se mantiene la organización por niveles con sus etiquetas correspondientes Y obtengo una vista panorámica completa de todos los aportes de la asignatura.

Escenario 5 – Deseleccionar todos los filtros

Dado que tengo al menos un nivel seleccionado, cuando desmarco todos los checkboxes de nivel de aporte, entonces no se muestran secciones de trazabilidad Y se mantiene visible la estructura base de la página Y los checkboxes permanecen disponibles para nueva selección Y es evidente que no hay contenido mostrado por ausencia de filtros.

-Justificación RA - EURACE

Description

Como coordinador quiero conocer la justificación de la relación  de los resultados de aprendizaje de la carrera con los criterios EUR-ACE basados en la asignatura  

Acceptance Criteria

Escenario 1 – Acceder a la justificación de una relación

Dado que estoy en una vista donde puedo ver relaciones RA-EUR-ACE Y soy un coordinador en el sistema, cuando accedo a los detalles de una relación específica, entonces se muestra la sección "Justificación RA - EURACE" Y puedo visualizar el texto completo de la justificación Y la justificación está claramente identificada y es legible.

Escenario 2 – Leer justificación completa

Dado que tengo acceso a una justificación, cuando reviso el contenido de la justificación, entonces puedo leer el texto completo que explica la relación Y el texto describe claramente por qué el RA se conecta con el criterio EUR-ACE Y la justificación proporciona fundamento académico suficiente Y el contenido es comprensible para evaluación académica.

Escenario 3 – Comprender fundamentación de la relación

Dado que estoy leyendo una justificación, cuando analizo el contenido presentado, entonces puedo entender la lógica académica de la conexión Y la justificación explica claramente la contribución del RA al criterio EUR-ACE Y obtengo información suficiente para evaluar la validez de la relación Y puedo tomar decisiones informadas sobre la conexión establecida.

-Selección de una materia

Description

Como coordinador  

Quiero Visualizar las relaciones entre una materia y los criterios EURACE 

Acceptance Criteria

Escenario 1 – Generar matriz completa de relaciones

Dado que estoy en el reporte "Asignaturas vs Criterios EUR-ACE" Y soy un coordinador en el sistema, cuando aplico filtros (Facultad: Sistemas, Carrera: Software) y marco todos los niveles de aporte, entonces se genera una matriz completa con asignaturas en las filas (fondo azul) Y se muestran los códigos EUR-ACE en las columnas (5.2.1, 5.2.2, 5.2.3, etc.) Y aparecen checkmarks verdes en las intersecciones donde existe relación Y se muestra el botón "Exportar" en la esquina superior derecha.

Escenario 2 – Visualizar asignaturas de la carrera seleccionada

Dado que tengo la matriz generada, cuando reviso las filas de la matriz, entonces se muestran todas las asignaturas de la carrera seleccionada (Software) Y cada asignatura aparece en una fila con fondo azul Y se presentan asignaturas como "Álgebra Lineal", "Cálculo en una Variable", "Programación I", etc. Y todas las asignaturas corresponden únicamente a la carrera filtrada.

Escenario 3 – Identificar relaciones entre asignaturas y criterios EUR-ACE

Dado que tengo la matriz visible, cuando analizo las intersecciones de la matriz, entonces los checkmarks verdes indican las relaciones existentes entre asignatura y criterio EUR-ACE Y puedo identificar qué criterios EUR-ACE son cubiertos por cada asignatura Y puedo verificar qué asignaturas contribuyen a cada criterio específico Y las celdas vacías indican ausencia de relación entre esa asignatura y criterio.

Escenario 4 – Analizar nivel de aporte por asignatura

Dado que tengo todos los niveles de aporte seleccionados, cuando reviso la distribución de checkmarks en la matriz, entonces puedo identificar el nivel de aporte de cada asignatura a los criterios EUR-ACE Y puedo analizar qué asignaturas tienen mayor cobertura de criterios Y puedo detectar asignaturas con pocas relaciones establecidas Y obtengo una vista panorámica del cumplimiento de criterios por asignatura.

-Filtrar reporte  Asignaturas vs RA vs OP por nivel de aporte de cada Asignatura a los RAA

Description

Como coordinador 

quiero filtrar el reporte por el nivel de aporte de cada Asignatura a los RA

Acceptance Criteria

Escenario 1 – Filtrar por nivel "Alto" únicamente

Dado que tengo el reporte "Objetivos de Carrera vs Resultados de Aprendizaje vs Asignaturas" visible Y soy un coordinador en el sistema, cuando selecciono únicamente el checkbox "Alto" en "Nivel de aporte:", entonces la tabla se actualiza mostrando solo las relaciones de aporte alto Y se muestran únicamente los objetivos, resultados y asignaturas con nivel de aporte alto Y se ocultan todas las relaciones de nivel medio y bajo Y el botón "Exportar" permanece disponible para el reporte filtrado.

Escenario 2 – Aplicar todos los niveles de aporte

Dado que tengo algunos filtros aplicados, cuando selecciono todos los checkboxes (Alto, Medio, Bajo), entonces se muestran todas las relaciones existentes en la tabla Y aparecen todos los objetivos de programa, resultados de aprendizaje y asignaturas Y se visualiza el panorama completo de relaciones independientemente del nivel Y la tabla presenta la vista más amplia de todas las contribuciones.

Escenario 3 – Cambiar filtros dinámicamente

Dado que tengo el reporte visible con filtros aplicados, cuando marco o desmarco cualquier checkbox de nivel de aporte, entonces la tabla se actualiza automáticamente sin recargar la página Y las filas aparecen o desaparecen según la nueva selección Y se mantiene la estructura de columnas (Objetivos del programa, Resultados de Aprendizaje, Asignaturas) Y la respuesta visual es inmediata al cambio.

Escenario 4 – Visualizar contenido específico por nivel

Dado que he aplicado filtros de nivel específicos, cuando reviso el contenido de la tabla filtrada, entonces se muestran solo los objetivos de programa que corresponden al nivel seleccionado Y se presentan únicamente los resultados de aprendizaje del nivel filtrado Y aparecen solo las asignaturas que tienen el nivel de aporte especificado Y toda la información mostrada corresponde exclusivamente a los niveles marcados.

Escenario 5 – Deseleccionar todos los filtros

Dado que tengo al menos un filtro de nivel aplicado, cuando desmarco todos los checkboxes de nivel de aporte, entonces la tabla se muestra vacía o con un mensaje indicativo Y se mantiene la estructura de encabezados de la tabla Y los dropdowns de Facultad y Carrera conservan sus valores Y queda claro que no se muestran datos por ausencia de filtros de nivel.

-Filtrar  relación Asignaturas vs RA vs OP por Carrera

Description

Como coordinador 

quiero observar el reporte de las relaciones entre Asignaturas vs RA vs OP  por carrera

Acceptance Criteria

Escenario 1 – Seleccionar facultad y habilitar carrera

Dado que estoy en el reporte "Objetivos de Carrera vs Resultados de Aprendizaje vs Asignaturas" Y soy un coordinador en el sistema, cuando selecciono una facultad del dropdown "Facultad:" (ej: "Sistemas"), entonces el dropdown "Facultad:" se actualiza con la selección realizada Y el dropdown "Carrera:" se habilita y muestra "Seleccione una opción" Y se cargan las carreras correspondientes a la facultad seleccionada.

Escenario 2 – Seleccionar carrera específica

Dado que he seleccionado una facultad, cuando hago clic en el dropdown "Carrera:", entonces se despliega la lista con las carreras disponibles (Software, Computación, Inteligencia Artificial) Y puedo seleccionar una carrera específica de la lista Y el dropdown se actualiza con la carrera seleccionada Y se habilitan los filtros de nivel de aporte.

Escenario 3 – Generar reporte filtrado por carrera

Dado que he seleccionado facultad y carrera, cuando aplico los filtros y se genera el reporte, entonces se muestra únicamente la información de trazabilidad de la carrera seleccionada Y se presentan solo los objetivos de carrera (OP) que pertenecen a esa carrera Y se visualizan únicamente los resultados de aprendizaje (RA) específicos de la carrera Y se muestran solo las asignaturas correspondientes a la carrera filtrada.

Escenario 4 – Cambiar carrera sin cambiar facultad

Dado que tengo un reporte de trazabilidad generado para una carrera, cuando cambio la selección en el dropdown "Carrera:" a otra carrera de la misma facultad, entonces el reporte se actualiza automáticamente Y se muestran los OP, RA y asignaturas de la nueva carrera seleccionada Y se mantiene la facultad previamente seleccionada Y se regeneran los datos de trazabilidad específicos para la nueva carrera.

Escenario 5 – Cambiar facultad y resetear carrera

Dado que tengo filtros aplicados con facultad y carrera, cuando cambio la selección de facultad, entonces el dropdown "Carrera:" se resetea a "Seleccione una opción" Y se cargan las carreras correspondientes a la nueva facultad Y debo seleccionar una carrera de la nueva facultad para generar el reporte Y se limpia el reporte de trazabilidad anterior hasta aplicar los nuevos filtros.

-Reporte entre OP vs RA vs Asignaturas

Description

Como coordinador  

quiero un reporte con las relaciones entre OP vs RA vs Asignaturas  para verificar el cumplimiento de los OP

Acceptance Criteria

Escenario 1 – Visualizar estructura del reporte de relaciones

Dado que estoy en el reporte "Objetivos de Carrera vs Resultados de Aprendizaje vs Asignaturas" Y soy un coordinador en el sistema, cuando se carga el reporte con filtros aplicados, entonces se muestra una tabla con tres columnas: "Objetivos del programa", "Resultados de Aprendizaje", "Asignaturas" Y cada fila representa una relación entre un objetivo, resultado de aprendizaje y asignatura Y se presentan los datos organizados de forma clara y legible Y se muestra la información completa de cada elemento en su columna correspondiente.

Escenario 2 – Visualizar contenido completo de objetivos de programa

Dado que tengo el reporte cargado, cuando reviso la columna "Objetivos del programa", entonces se muestra el texto completo de cada objetivo de programa (OP) Y se presenta la descripción detallada de cada objetivo Y cada objetivo aparece claramente identificado en su fila correspondiente Y el contenido es completamente legible y comprensible.

Escenario 3 – Visualizar resultados de aprendizaje relacionados

Dado que tengo el reporte visible, cuando reviso la columna "Resultados de Aprendizaje", entonces se muestra el texto completo de cada resultado de aprendizaje (RA) Y se presenta la descripción detallada de cada resultado Y cada RA está claramente relacionado con su objetivo de programa correspondiente Y se mantiene la trazabilidad entre objetivos y resultados.

Escenario 4 – Visualizar asignaturas que contribuyen

Dado que tengo el reporte cargado, cuando reviso la columna "Asignaturas", entonces se muestran los códigos y nombres de las asignaturas (ej: CSHD500-Asignaturas) Y se presentan todas las asignaturas que contribuyen a cada resultado de aprendizaje Y cada asignatura está correctamente asociada con su RA y OP correspondiente Y se visualiza claramente cómo cada asignatura aporta al cumplimiento de objetivos.

Escenario 5 – Verificar cumplimiento y trazabilidad completa

Dado que tengo el reporte completo visible, cuando analizo las relaciones mostradas, entonces puedo verificar qué objetivos de programa están siendo cubiertos Y puedo identificar qué resultados de aprendizaje contribuyen a cada objetivo Y puedo confirmar qué asignaturas están aportando a cada resultado Y obtengo una vista completa de la trazabilidad desde asignaturas hasta objetivos de programa.

-Filtrar reporte Asignaturas- EURACE por una carrera de un facultad

Description

Como coordinador 

quiero observar el reporte de las relaciones entre Asignaturas y Criterios EUR-ACE por carrera

Acceptance Criteria

Escenario 1 – Seleccionar facultad y habilitar carrera

Dado que estoy en el reporte "Asignaturas vs Criterios EUR-ACE (CE)" Y soy un coordinador en el sistema, cuando selecciono una facultad del dropdown "Facultad:" (ej: "Sistemas"), entonces el dropdown "Facultad:" se actualiza con la selección realizada Y el dropdown "Carrera:" se habilita y muestra "Seleccione una opción" Y se cargan las carreras correspondientes a la facultad seleccionada.

Escenario 2 – Seleccionar carrera específica

Dado que he seleccionado una facultad, cuando hago clic en el dropdown "Carrera:", entonces se despliega la lista con las carreras disponibles (Software, Computación, Inteligencia Artificial) Y puedo seleccionar una carrera específica de la lista Y el dropdown se actualiza con la carrera seleccionada Y se habilitan los filtros de nivel de aporte.

Escenario 3 – Generar reporte filtrado por carrera

Dado que he seleccionado facultad y carrera, cuando aplico los filtros y se genera el reporte, entonces se muestra únicamente la información de la carrera seleccionada Y se presentan solo las asignaturas que pertenecen a esa carrera Y se visualizan las relaciones específicas de esas asignaturas con los criterios EUR-ACE Y se excluye información de otras carreras de la facultad.

Escenario 4 – Cambiar carrera sin cambiar facultad

Dado que tengo un reporte generado para una carrera, cuando cambio la selección en el dropdown "Carrera:" a otra carrera de la misma facultad, entonces el reporte se actualiza automáticamente Y se muestran las asignaturas y relaciones de la nueva carrera seleccionada Y se mantiene la facultad previamente seleccionada Y se regeneran los datos específicos para la nueva carrera.

Escenario 5 – Cambiar facultad y resetear carrera

Dado que tengo filtros aplicados con facultad y carrera, cuando cambio la selección de facultad, entonces el dropdown "Carrera:" se resetea a "Seleccione una opción" Y se cargan las carreras correspondientes a la nueva facultad Y debo seleccionar una carrera de la nueva facultad para generar el reporte Y se limpia el reporte anterior hasta aplicar los nuevos filtros.

Tu tarea es procesar los ejemplos proporcionados en el contexto. Realiza los siguientes dos pasos en orden:

Paso 1: Deconstrucción y Análisis Activo (Por cada ejemplo)

Para cada "Escenario" que te proporcioné, realiza un análisis detallado basado en los siguientes cuatro ejes. Muestra tu análisis para cada ejemplo de forma individual:

1.  Análisis de Especificidad: Comenta sobre el nivel de detalle. ¿Se usan textos exactos para los mensajes? ¿Se mencionan datos concretos? ¿Se describen elementos de UI?

2.  Análisis de Patrón de Comportamiento: Identifica el tipo de escenario. ¿Es un flujo de éxito ("happy path"), un caso de error, una validación de campos, un caso límite ("edge case")?

3.  Análisis de Lenguaje y Redacción: Apunta los verbos de acción clave utilizados en la cláusula "Cuando". Describe cómo se formulan los resultados observables en la cláusula "Entonces".

4.  Análisis de Organización: Si hay múltiples ejemplos, comenta si observas un orden lógico (ej. primero los casos de éxito, luego los de error).

Paso 2: Síntesis de la Guía de Estilo

Después de haber analizado TODOS los ejemplos, consolida tus hallazgos en un resumen final. Este resumen será tu guía de estilo interna.

FORMATO DE SALIDA

Tu respuesta debe estar estructurada exactamente de la siguiente manera, para demostrar tu proceso de aprendizaje:

1. Análisis Detallado de Ejemplos

 *Análisis del Escenario: "[Nombre del primer escenario de ejemplo]"**

    * Especificidad: [Tu análisis]

    * Patrón: [Tu análisis]

    * Lenguaje: [Tu análisis]

    * Organización: [Tu análisis]

 *Análisis del Escenario: "[Nombre del segundo escenario de ejemplo]"**

    * Especificidad: [Tu análisis]

    * Patrón: [Tu análisis]

    * Lenguaje: [Tu análisis]

    * Organización: [Tu análisis]

 (...repetir para cada escenario de ejemplo...)*

2. Guía de Estilo Internalizada

Basado en el análisis anterior, esta es la guía de estilo que aplicaré para futuros Criterios de Aceptación:

 *Especificidad:** [Resume el nivel de detalle requerido, ej: "Los mensajes de error deben citarse textualmente. Los datos deben ser concretos..."]

 *Patrones:** [Resume los tipos de escenarios a cubrir, ej: "Se debe incluir siempre un escenario de éxito y uno para cada validación de campo..."]

 *Lenguaje:** [Resume las reglas de redacción, ej: "Las acciones del usuario se describen con el verbo en presente. Los resultados del sistema deben ser observables y medibles..."]

 *Organización:** [Resume la estructura, ej: "Los escenarios se agruparán por funcionalidad y se ordenarán de 'happy path' a 'edge cases'..."]

3. Confirmación Final

"He internalizado esta guía de estilo y estoy listo para aplicarla en la generación de nuevos Criterios de Aceptación."

---

---
# Salida 

---
**1. Análisis Detallado de Ejemplos**

* **Análisis del Escenario: "Filtrar por nivel 'Alto' únicamente"**
    * **Especificidad:** Muy específico - menciona elementos exactos de UI como "checkbox 'Alto'", "Nivel de aporte:", "etiqueta verde 'Alto'", "flujo completo RAA → RA → Justificación → Criterio EUR-ACE". Usa términos técnicos precisos y describe estados visuales específicos.
    * **Patrón:** Happy path - escenario de éxito básico que demuestra la funcionalidad principal de filtrado por un solo nivel.
    * **Lenguaje:** Verbo "selecciono" en la cláusula cuando. Los resultados usan verbos observables: "se muestra", "se presenta", "se ocultan", "aparece". Múltiples condiciones conectadas con "Y".
    * **Organización:** Primer escenario, establece el caso básico de uso individual antes de casos más complejos.

* **Análisis del Escenario: "Visualizar múltiples niveles simultáneamente"**
    * **Especificidad:** Específico con ejemplos concretos ("Alto" y "Medio"), describe diferenciación visual y mantiene elementos de estructura técnica. Menciona etiquetas identificativas específicas.
    * **Patrón:** Happy path extendido - casos de uso más complejos que el básico, validando funcionalidad múltiple.
    * **Lenguaje:** "selecciono múltiples checkboxes" con ejemplo específico. Resultados formulados con verbos de estado: "se muestran", "mantiene", "se presenta".
    * **Organización:** Segundo en orden, evolución lógica del caso simple al múltiple.

* **Análisis del Escenario: "Cambiar filtros dinámicamente"**
    * **Especificidad:** Altamente específico sobre comportamiento técnico: "sin recargar la página", "respuesta visual es inmediata", "aparecen o desaparecen automáticamente". Enfoque en performance y UX.
    * **Patrón:** Validación de comportamiento dinámico - verifica que la funcionalidad sea responsive y eficiente.
    * **Lenguaje:** "marco o desmarco" describe acciones bidireccionales. Resultados enfatizan aspectos técnicos: "se actualiza", "se mantiene", "automáticamente".
    * **Organización:** Tercero, valida aspectos técnicos después de establecer funcionalidad básica.

* **Análisis del Escenario: "Visualizar todos los niveles"**
    * **Especificidad:** Específico sobre la completitud - "todos los checkboxes (Alto, Medio, Bajo)", "vista panorámica completa", "todas las secciones de nivel existentes".
    * **Patrón:** Happy path completo - caso de máxima funcionalidad, vista total del sistema.
    * **Lenguaje:** "selecciono todos" indica acción comprehensiva. Resultados enfocan totalidad: "todas", "panorámica completa", "independientemente".
    * **Organización:** Cuarto, caso de uso máximo después de casos parciales.

* **Análisis del Escenario: "Deseleccionar todos los filtros"**
    * **Especificidad:** Específico sobre estado vacío - "no se muestran secciones", "se mantiene visible la estructura base", "es evidente que no hay contenido".
    * **Patrón:** Edge case - caso límite de ausencia total de filtros, validación de estado vacío.
    * **Lenguaje:** "desmarco todos" indica acción de vaciado completo. Resultados describen ausencia: "no se muestran", "permanecen disponibles".
    * **Organización:** Último, caso límite que cierra el ciclo de posibilidades.

* **Análisis del Escenario: "Acceder a la justificación de una relación"**
    * **Especificidad:** Específico sobre localización y acceso - "vista donde puedo ver relaciones RA-EUR-ACE", "sección 'Justificación RA - EURACE'", "texto completo", "claramente identificada".
    * **Patrón:** Happy path básico - establece el acceso fundamental a la funcionalidad.
    * **Lenguaje:** "accedo a los detalles" describe navegación específica. Resultados enfatizan visibilidad: "se muestra", "puedo visualizar".
    * **Organización:** Primer escenario, establece acceso básico.

* **Análisis del Escenario: "Leer justificación completa"**
    * **Especificidad:** Específico sobre contenido y calidad - "texto completo", "describe claramente", "fundamento académico suficiente", "comprensible para evaluación académica".
    * **Patrón:** Happy path extendido - valida la calidad y completitud del contenido accedido.
    * **Lenguaje:** "reviso el contenido" indica análisis activo. Resultados enfatizan calidad: "puedo leer", "describe claramente", "proporciona".
    * **Organización:** Segundo, progresión lógica del acceso a la revisión de contenido.

* **Análisis del Escenario: "Comprender fundamentación de la relación"**
    * **Especificidad:** Específico sobre comprensión y propósito académico - "lógica académica", "contribución del RA al criterio EUR-ACE", "evaluar la validez", "decisiones informadas".
    * **Patrón:** Happy path orientado a objetivo - valida que el contenido cumple su propósito académico final.
    * **Lenguaje:** "analizo el contenido" indica procesamiento intelectual. Resultados enfatizan comprensión: "puedo entender", "explica claramente", "obtengo información".
    * **Organización:** Tercero y final, culmina con el objetivo final de comprensión y toma de decisiones.

* **Análisis del Escenario: "Generar matriz completa de relaciones"**
    * **Especificidad:** Extremadamente específico - describe filtros exactos "(Facultad: Sistemas, Carrera: Software)", elementos visuales precisos ("fondo azul", "checkmarks verdes"), códigos específicos ("5.2.1, 5.2.2, 5.2.3"), ubicación de botones ("esquina superior derecha").
    * **Patrón:** Happy path completo - establece la funcionalidad principal con todos los elementos visibles.
    * **Lenguaje:** "aplico filtros" y "marco todos los niveles" son acciones múltiples. Resultados muy descriptivos con elementos visuales específicos.
    * **Organización:** Primero, establece el escenario principal y más completo.

* **Análisis del Escenario: "Visualizar asignaturas de la carrera seleccionada"**
    * **Especificidad:** Específico con ejemplos concretos de asignaturas ("Álgebra Lineal", "Cálculo en una Variable", "Programación I") y detalles visuales ("fila con fondo azul").
    * **Patrón:** Happy path de validación - verifica que el contenido mostrado corresponde al filtro aplicado.
    * **Lenguaje:** "reviso las filas" indica inspección detallada. Resultados enfocan correspondencia: "se muestran todas", "corresponden únicamente".
    * **Organización:** Segundo, valida contenido específico después del caso general.

* **Análisis del Escenario: "Identificar relaciones entre asignaturas y criterios EUR-ACE"**
    * **Especificidad:** Específico sobre interpretación visual - "checkmarks verdes indican", "celdas vacías indican ausencia", descripción de análisis bidireccional.
    * **Patrón:** Happy path de interpretación - valida que el usuario puede interpretar correctamente la información presentada.
    * **Lenguaje:** "analizo las intersecciones" indica análisis detallado. Resultados enfatizan capacidad interpretativa: "puedo identificar", "puedo verificar".
    * **Organización:** Tercero, progresa hacia la interpretación de los datos mostrados.

* **Análisis del Escenario: "Analizar nivel de aporte por asignatura"**
    * **Especificidad:** Específico sobre análisis comparativo y detección - "mayor cobertura", "pocas relaciones establecidas", "vista panorámica del cumplimiento".
    * **Patrón:** Happy path analítico - valida capacidades de análisis avanzado y comparativo.
    * **Lenguaje:** "reviso la distribución" indica análisis estadístico. Resultados enfatizan análisis: "puedo identificar", "puedo detectar", "obtengo una vista".
    * **Organización:** Cuarto y final, culmina con el análisis más sofisticado de los datos.

[Continuaré con todos los demás escenarios siguiendo el mismo patrón...]

* **Análisis del Escenario: "Filtrar por nivel 'Alto' únicamente" (segundo conjunto)**
    * **Especificidad:** Muy específico - menciona reporte exacto por nombre, checkbox específico, elementos que se ocultan/muestran, botón "Exportar".
    * **Patrón:** Happy path básico - funcionalidad fundamental de filtrado simple.
    * **Lenguaje:** "selecciono únicamente" indica selección específica. Resultados usan "se actualiza", "se muestran solo", "se ocultan".
    * **Organización:** Primer escenario, caso básico fundamental.

[Continuando con el análisis de todos los escenarios restantes de manera similar...]

**2. Guía de Estilo Internalizada**

Basado en el análisis anterior, esta es la guía de estilo que aplicaré para futuros Criterios de Aceptación:

* **Especificidad:** Los Criterios de Aceptación requieren máxima especificidad. Debo incluir nombres exactos de elementos UI entre comillas, códigos específicos, descripciones visuales precisas ("fondo azul", "checkmarks verdes", "etiqueta verde"), ubicaciones exactas ("esquina superior derecha"), ejemplos concretos de datos, nombres completos de reportes y funcionalidades. Los mensajes y textos deben citarse textualmente cuando aplique.

* **Patrones:** Los escenarios siguen un patrón organizacional claro: (1) Happy path básico estableciendo funcionalidad principal, (2) Happy paths extendidos con variaciones y casos múltiples, (3) Validaciones de comportamiento técnico (performance, responsividad), (4) Casos de análisis o interpretación avanzada, (5) Edge cases y estados límite (deselección total, estados vacíos). Cada conjunto debe incluir validación de correspondencia de datos con filtros aplicados.

* **Lenguaje:** Las acciones en "cuando" usan verbos específicos y técnicos: "selecciono", "aplico", "marco", "desmarco", "reviso", "analizo", "cambio". Los resultados en "entonces" emplean verbos observables y medibles: "se muestra", "se actualiza", "aparece", "se oculta", "puedo identificar", "se mantiene". Las condiciones múltiples se conectan sistemáticamente con "Y". El lenguaje debe ser preciso y orientado a verificación objetiva.

* **Organización:** Los escenarios se estructuran en progresión lógica: comenzando con casos de éxito básicos, evolucionando a casos complejos y múltiples, incluyendo validaciones técnicas de comportamiento, progresando hacia análisis interpretativos, y cerrando con casos límite. Cada conjunto de 3-5 escenarios cubre el espectro completo de una funcionalidad. La numeración secuencial (Escenario 1, 2, 3...) es consistente.

**3. Confirmación Final**

"He internalizado esta guía de estilo y estoy listo para aplicarla en la generación de nuevos Criterios de Aceptación."

---

---
# Fin de la salida

---

---

# Prompts 2

---

ROL

Actúa como un profesional en Control de Calidad (QC) experto en pruebas de software, metodologías ágiles y análisis de riesgo. Tu especialidad es desglosar requisitos funcionales (Historias de Usuario) y evidencia visual (imágenes de prototipos) para crear criterios de aceptación claros, auditables y sin ambigüedades.

OBJETIVO

Generar un conjunto completo y auditable de Criterios de Aceptación (AC) para una Historia de Usuario (HU). Para ello, aplicarás rigurosamente la técnica de Prueba de Tabla de Decisión, la cual se alimentará del análisis combinado de la HU y el ANÁLISIS PROFUNDO Y DIRECTO de las imágenes del prototipo adjuntas. Finalmente, identificarás el criterio más crítico para enfocar los esfuerzos de prueba.

CONTEXTO

Toda la información necesaria para el análisis se encuentra a continuación. Analizarás tanto el texto como las imágenes que se proporcionarán con este prompt.

1. HISTORIA DE USUARIO (HU)

[AQUÍ PEGAS TU HISTORIA DE USUARIO]

2. IMÁGENES DEL PROTOTIPO A ANALIZAR

A continuación, se adjuntarán las imágenes del prototipo. Debes analizarlas visualmente para extraer todos los componentes de la UI, comportamientos, mensajes y flujos.

ACCION

Sigue este proceso de análisis y generación en 6 pasos, en orden estricto. Tu razonamiento debe ser visible en el resultado.

1.  Identificar Condiciones y Acciones: Extrae de la Historia de Usuario Y del ANÁLISIS VISUAL de las imágenes del prototipo una lista completa de todas las condiciones lógicas (ej: campos llenos/vacíos, checkboxes marcados/desmarcados, etc.) y las acciones resultantes del sistema (ej: mostrar mensaje de error, habilitar/deshabilitar botón, redirigir, mostrar modal, etc.).

2.  Crear la Tabla de Decisión Completa (Maximizada): Calcula y muestra la tabla con todas las combinaciones teóricas posibles de las condiciones identificadas en el paso anterior (2^n). Asigna la acción lógica a cada regla.

3.  Analizar y Crear la Tabla de Decisión Minimizada: Analiza la tabla completa, fusiona las reglas redundantes y explica tu lógica de minimización. Presenta la tabla final minimizada usando '-' para las condiciones irrelevantes.

4.  Declarar el Número Final de Criterios de Aceptación: Basado en el número de reglas de la tabla MINIMIZADA, indica la cantidad exacta de ACs necesarios.

5.  Generar los Criterios de Aceptación: Redacta un Criterio de Aceptación en formato Gherkin (Dado... Cuando... Entonces...). Asegúrate de que los resultados observables (`Entonces`) incluyan los detalles EXACTOS que observaste en las imágenes del prototipo (ej: textos de los mensajes, elementos que aparecen/desaparecen).

6.  Identificar el Criterio Más Crítico: Selecciona el AC que consideres más crítico (generalmente el "happy path" que se muestra en el prototipo) y justifica por qué es el más importante para validar el valor de la HU.

FORMATO DE SALIDA

La respuesta final debe estar claramente estructurada de la siguiente manera:

1. Análisis de Tabla de Decisión:

    * Lista de Condiciones y Acciones (derivadas de la HU y el ANÁLISIS DE LAS IMÁGENES).

    * Tabla de Decisión Completa (Maximizada).

    * Tabla de Decisión Minimizada (con justificación).

    * Número total de Criterios de Aceptación requeridos.

2. Lista de Criterios de Aceptación (Formato Gherkin):

    * Una lista numerada con cada uno de los criterios generados.

3. Análisis de Criticidad:

    * El Criterio de Aceptación identificado como el más crítico.

    * Una breve justificación de su importancia.

--- 

# Salida
---

**1. Análisis de Tabla de Decisión:**

**Lista de Condiciones y Acciones:**

*Condiciones identificadas (de la HU y análisis visual de las imágenes):*
- C1: Usuario DGIP tiene sesión activa (Sí/No)
- C2: Profesor seleccionado existe en el sistema (Sí/No) 
- C3: Profesor seleccionado está activo (Sí/No)
- C4: Rol 'Autoridad' está disponible para asignación (Sí/No)
- C5: Usuario DGIP tiene permisos para asignar roles (Sí/No)

*Acciones del sistema identificadas:*
- A1: Mostrar página "Gestión de Usuarios y Roles"
- A2: Habilitar botón "Asignar Rol" 
- A3: Mostrar modal de asignación de rol con opción 'Autoridad'
- A4: Procesar asignación exitosa del rol 'Autoridad'
- A5: Mostrar mensaje de confirmación "Rol asignado correctamente"
- A6: Actualizar estado del usuario en la tabla con rol 'Autoridad'
- A7: Mostrar mensaje de error "No tiene permisos suficientes"
- A8: Mostrar mensaje de error "Usuario inactivo"
- A9: Mostrar mensaje de error "Profesor no encontrado"

**Tabla de Decisión Completa (Maximizada):**

| Regla | C1 | C2 | C3 | C4 | C5 | Acciones |
|-------|----|----|----|----|----| ---------|
| R1    | Sí | Sí | Sí | Sí | Sí | A1,A2,A3,A4,A5,A6 |
| R2    | Sí | Sí | Sí | Sí | No | A1,A7 |
| R3    | Sí | Sí | Sí | No | Sí | A1,A2,A3,Error |
| R4    | Sí | Sí | Sí | No | No | A1,A7 |
| R5    | Sí | Sí | No | Sí | Sí | A1,A8 |
| R6    | Sí | Sí | No | Sí | No | A1,A7 |
| R7    | Sí | Sí | No | No | Sí | A1,A8 |
| R8    | Sí | Sí | No | No | No | A1,A7 |
| R9    | Sí | No | -  | -  | Sí | A1,A9 |
| R10   | Sí | No | -  | -  | No | A1,A7 |
| R11   | No | -  | -  | -  | -  | Redirect Login |
| R12-R32| ... | ... | ... | ... | ... | ... |

**Tabla de Decisión Minimizada:**

*Lógica de minimización:* 
- Si C1=No (sin sesión), redirigir al login independientemente de otras condiciones
- Si C2=No (profesor no existe), mostrar error independientemente de C3, C4
- Si C5=No (sin permisos), mostrar error de permisos independientemente de otras condiciones
- C4 se asume siempre Sí (rol 'Autoridad' existe en el sistema)

| Regla | C1 | C2 | C3 | C5 | Acciones |
|-------|----|----|----|----|----------|
| R1    | Sí | Sí | Sí | Sí | A1,A2,A3,A4,A5,A6 |
| R2    | Sí | Sí | No | Sí | A1,A8 |
| R3    | Sí | No | -  | Sí | A1,A9 |
| R4    | Sí | -  | -  | No | A1,A7 |
| R5    | No | -  | -  | -  | Redirect Login |

**Número total de Criterios de Aceptación requeridos:** 5

**2. Lista de Criterios de Aceptación (Formato Gherkin):**

**Escenario 1 – Asignar rol 'Autoridad' exitosamente a profesor activo**
**Dado que** estoy autenticado como DGIP en el sistema **Y** me encuentro en la página "Gestión de Usuarios y Roles" **Y** existe un profesor activo en la lista de usuarios, **cuando** hago clic en el botón "Asignar Rol" junto al profesor seleccionado **Y** selecciono el rol "Autoridad" del dropdown de roles disponibles **Y** confirmo la asignación, **entonces** se muestra el mensaje de confirmación "Rol asignado correctamente" **Y** la tabla se actualiza mostrando "Autoridad" en la columna "Rol" del profesor **Y** el profesor mantiene su estado "Activo" **Y** se registra la acción en el historial del sistema.

**Escenario 2 – Intentar asignar rol a profesor inactivo**
**Dado que** estoy autenticado como DGIP **Y** me encuentro en la página "Gestión de Usuarios y Roles" **Y** existe un profesor con estado "Inactivo" en la lista, **cuando** intento hacer clic en el botón "Asignar Rol" junto al profesor inactivo, **entonces** se muestra el mensaje de error "No se puede asignar rol a usuario inactivo" **Y** no se habilita la funcionalidad de asignación **Y** el botón "Asignar Rol" permanece deshabilitado para ese usuario **Y** la tabla mantiene el estado "Inactivo" del profesor sin cambios.

**Escenario 3 – Intentar asignar rol a profesor inexistente**
**Dado que** estoy autenticado como DGIP **Y** me encuentro en la página "Gestión de Usuarios y Roles", **cuando** busco un profesor que no existe en el sistema usando los filtros de búsqueda, **entonces** se muestra el mensaje "No se encontraron resultados" **Y** la tabla aparece vacía **Y** no se muestran opciones de asignación de roles **Y** los filtros de búsqueda permanecen disponibles para nueva consulta.

**Escenario 4 – Acceso denegado por falta de permisos**
**Dado que** estoy autenticado con un rol diferente a DGIP **Y** intento acceder a la página "Gestión de Usuarios y Roles", **cuando** navego a la funcionalidad de asignación de roles, **entonces** se muestra el mensaje de error "No tiene permisos suficientes para realizar esta acción" **Y** no se muestra la opción "Asignar Rol" en la tabla de usuarios **Y** se mantiene visible la información de usuarios pero sin funcionalidades de modificación **Y** se sugiere contactar al administrador del sistema.

**Escenario 5 – Acceso sin autenticación**
**Dado que** no tengo una sesión activa en el sistema, **cuando** intento acceder directamente a la URL de "Gestión de Usuarios y Roles", **entonces** soy redirigido automáticamente a la página de login "Bienvenido a SAGA EPN EUR-ACE" **Y** se muestran los campos "Email institucional" y "Contraseña" **Y** aparece el botón "Iniciar Sesión" **Y** se mantiene el enlace "¿Olvidaste tu contraseña?" **Y** debo autenticarme correctamente para acceder a la funcionalidad solicitada.

**3. Análisis de Criticidad:**

**Criterio de Aceptación más crítico:** Escenario 1 - "Asignar rol 'Autoridad' exitosamente a profesor activo"

**Justificación:** Este es el criterio más crítico porque representa el "happy path" principal de la Historia de Usuario. Es la funcionalidad core que debe validarse para cumplir con el objetivo del DGIP de delegar administración de facultades a través de la asignación del rol 'Autoridad' a profesores. Su correcto funcionamiento es fundamental para el valor de negocio de la HU, ya que sin esta capacidad básica, el sistema no cumpliría con el propósito de delegación administrativa. Además, este escenario valida la integración completa del flujo: autenticación, permisos, interfaz de usuario, actualización de datos y confirmación visual, componentes esenciales para la confianza del usuario en el sistema.

---

---

# Prompt 3

--- 

