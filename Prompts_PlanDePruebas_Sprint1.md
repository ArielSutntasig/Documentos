# Prompt para Plan de Pruebas
---
# Prompt 1

---

ROL
Actúa como un sistema de IA experto en Análisis de Calidad, con una especialidad en aprendizaje adaptativo de patrones de documentación. Eres capaz de deconstruir ejemplos de referencia (Casos de Prueba) para internalizar y replicar su estructura, lenguaje, tono y nivel de especificidad con una precisión del 100%.
OBJETIVO
Analizar activamente un conjunto de ejemplos de referencia para construir una "Guía de Estilo" interna y detallada. El propósito final es que puedas replicar este estilo exacto en la generación de futuros artefactos de prueba cuando se te solicite.
CONTEXTO
A continuación, se proporciona un archivo excel adjunto con un conjunto de ejemplos en su tercera hoja de excel, que representan el estándar de oro que debes aprender y seguir.

ACCION
Tu tarea es procesar los ejemplos proporcionados en el contexto. Realiza los siguientes dos pasos en orden:
Paso 1: Deconstrucción y Análisis Activo (Por cada ejemplo)
Para cada ejemplo principal que te proporcioné (ej. caso de prueba), realiza un análisis detallado basado en los siguientes cuatro ejes.
1.  Análisis de Especificidad: Comenta sobre el nivel de detalle. ¿Se usan textos exactos para los mensajes? ¿Se mencionan datos o componentes de UI concretos? ¿Qué tan detallados son los pasos o los resultados esperados?
2.  Análisis de Patrón y Estructura: Identifica el tipo de escenario o caso (ej: Flujo de éxito, caso de error, validación, caso límite). Describe la estructura general (ej: formato de tabla de pruebas).
3.  Análisis de Lenguaje y Tono: Apunta los verbos de acción clave utilizados. Describe la redacción de los resultados observables. ¿El tono es formal, técnico, directo?
4.  Análisis de Organización: Si hay múltiples ejemplos, comenta si observas un orden lógico (ej. primero los casos de éxito, luego los de error) o alguna agrupación específica.
Paso 2: Síntesis de la Guía de Estilo
Después de haber analizado TODOS los ejemplos, consolida tus hallazgos en un resumen final. Este resumen será tu guía de estilo interna.
FORMATO DE SALIDA
Tu respuesta debe estar estructurada exactamente de la siguiente manera, para demostrar tu proceso de aprendizaje:
1. Análisis Detallado de Ejemplos
* Análisis del Ejemplo 1: "[Título o ID del primer ejemplo]"
    * Especificidad: [Tu análisis]
    * Patrón y Estructura: [Tu análisis]
    * Lenguaje y Tono: [Tu análisis]
    * Organización: [Tu análisis]
* (...repetir para cada ejemplo principal...)
2. Guía de Estilo Internalizada
Basado en el análisis anterior, esta es la guía de estilo que aplicaré para futuros documentos de prueba:
* Especificidad: [Resume el nivel de detalle requerido.]
* Estructura: [Resume el formato y los patrones a seguir.]
* Lenguaje: [Resume las reglas de redacción y el tono.]
* Organización: [Resume la estructura y el orden lógicos.]
3. Confirmación Final
"He internalizado esta guía de estilo y estoy listo para aplicarla con precisión en futuras solicitudes."
---
# Salida

--- 
Entiendo perfectamente tu solicitud. Necesito analizar el archivo Excel que proporcionaste para crear una guía de estilo interna basada en los ejemplos de casos de prueba. Voy a proceder a leer el archivo y examinar específicamente la tercera hoja donde indicas están los ejemplos.Perfecto, he accedido exitosamente al archivo Excel y he encontrado los casos de prueba en la hoja "Guión". Puedo ver una extensa colección de casos de prueba con una estructura muy detallada. Procederé ahora con el análisis según tu solicitud.

## 1. Análisis Detallado de Ejemplos

### **Análisis del Ejemplo 1: "Registrar Profesores-Escenario 1 – Abrir modal de nuevo profesor"**

* **Especificidad:** Altamente específico. Utiliza textos exactos como "Tabla de Profesores", "Nuevo Profesor", menciona componentes específicos de UI como botones con colores definidos ("Cancelar" en rojo, "Guardar" en verde), especifica nombres exactos de campos ("Nombres", "Apellidos", "Cédula", "Facultad", "Correo", "Contraseña") y usa datos concretos como "Química" para el autocompletado.

* **Patrón y Estructura:** Caso de flujo positivo básico. Estructura de tabla con múltiples pasos secuenciales (Paso1-Paso6). Cada paso tiene tres columnas principales: "Nombre Paso", "Descripción Paso", y "Resultados Esperados". Los pasos siguen una lógica de interacción UI: acceso → acción → verificación → confirmación.

* **Lenguaje y Tono:** Utiliza verbos de acción directos y técnicos: "Acceder", "Hacer clic", "Verificar", "Confirmar". Los resultados esperados usan un lenguaje muy descriptivo y observable: "Se carga correctamente", "Se muestra", "Se presenta", "Se visualiza". El tono es formal, técnico y orientado a la verificación objetiva.

* **Organización:** Los casos siguen un patrón lógico iniciando con flujos de éxito, seguidos de validaciones y casos de error. Los escenarios están numerados secuencialmente y agrupados por funcionalidad (Registrar Profesores, Listar Profesores, etc.).

### **Análisis del Ejemplo 2: "Registrar Profesores-Escenario 2 – Completar información del profesor"**

* **Especificidad:** Extremadamente específico con datos de prueba reales: "José David" para nombres, "Terán Ramos" para apellidos, "1726285040" para cédula, "jose.teran@epn.edu.ec" para correo, "Teranosaurio123*" para contraseña. Especifica formatos exactos y validaciones técnicas.

* **Patrón y Estructura:** Caso de flujo de entrada de datos (Tipo: Negativo, aunque el contenido sugiere positivo). Mantiene la estructura de pasos múltiples, cada uno enfocado en completar un campo específico. Sigue el patrón: prerrequisito → acción → validación → resultado.

* **Lenguaje y Tono:** Lenguaje muy técnico con especificaciones precisas: "Se ingresa correctamente", "El campo acepta", "Se valida formato", "No se permiten caracteres no numéricos". Mantiene consistencia en la descripción de comportamientos esperados del sistema.

* **Organización:** Secuencia lógica de campos siguiendo un orden típico de formulario (nombres, apellidos, cédula, correo, contraseña), con verificación final del estado del formulario.

### **Análisis del Ejemplo 3: "Agregar Nueva Autoridad-Escenario 1 – Abrir modal de nueva autoridad"**

* **Especificidad:** Muy específico en nomenclatura: "Nueva Autoridad", "Tabla de Autoridad". Menciona elementos exactos de UI como placeholders específicos ("Ej. José David", "Ej. Decano"), valores predefinidos ("Autoridad" en campo Rol), y colores específicos de botones.

* **Patrón y Estructura:** Caso de apertura de modal (Tipo: Positivo). Estructura similar con verificación de elementos de UI paso a paso. Patrón: navegación → acción → verificación modal → confirmación campos → confirmación botones.

* **Lenguaje y Tono:** Consistente con otros casos. Usa "Se ejecuta", "Se presenta", "Se muestra" para describir comportamientos del sistema. Lenguaje técnico preciso para describir interacciones UI.

* **Organización:** Agrupa funcionalidades por módulos (Facultad-Profesores, Facultad-Autoridad, CEI) y sigue una progresión lógica de complejidad dentro de cada módulo.

### **Análisis del Ejemplo 4: "Filtrar Profesores-Escenario 1 – Filtrar profesores por palabra clave"**

* **Especificidad:** Usa ejemplos específicos de búsqueda ("José"), especifica comportamientos técnicos detallados como "El filtrado funciona tanto en nombres como en correos electrónicos", menciona actualización de contadores y paginación específicamente.

* **Patrón y Estructura:** Caso de funcionalidad de filtrado (Tipo: Positivo). Estructura de interacción: acceso → entrada → ejecución → verificación múltiple. Más complejo que los casos de modal básicos.

* **Lenguaje y Tono:** Mantiene la consistencia terminológica. Usa "Se ejecuta inmediatamente", "La tabla se actualiza", "Solo se muestran". Lenguaje orientado a verificación de comportamientos dinámicos del sistema.

* **Organización:** Los casos de filtrado siguen una progresión: éxito → sin resultados → limpiar filtro → mantener funcionalidad, cubriendo todos los escenarios posibles.

## 2. Guía de Estilo Internalizada

Basado en el análisis anterior, esta es la guía de estilo que aplicaré para futuros documentos de prueba:

* **Especificidad:** Usar textos exactos de UI, datos de prueba reales y específicos, nombres precisos de campos y componentes, colores específicos de botones, valores exactos de placeholders, y comportamientos técnicos detallados. Evitar generalidades - cada elemento debe ser verificable objetivamente.

* **Estructura:** Mantener formato tabular con columnas estándar. Organizar por escenarios numerados secuencialmente dentro de cada funcionalidad. Usar pasos múltiples (Paso1, Paso2, etc.) con tres elementos: Nombre del Paso, Descripción del Paso, y Resultados Esperados. Seguir progresión lógica: flujos positivos → validaciones → casos negativos → casos límite.

* **Lenguaje:** Usar verbos de acción técnicos consistentes: "Acceder", "Hacer clic", "Verificar", "Confirmar", "Ingresar", "Seleccionar". Para resultados esperados usar: "Se carga correctamente", "Se muestra", "Se presenta", "Se visualiza", "Se ejecuta", "Se actualiza". Mantener tono formal, técnico, y orientado a verificación objetiva. Usar formato de lista con viñetas (•) para resultados esperados múltiples.

* **Organización:** Agrupar por módulos funcionales (ej: Facultad-Profesores, Facultad-Autoridad). Dentro de cada módulo seguir orden lógico: operaciones básicas → funcionalidades avanzadas → casos de error → casos límite. Usar nomenclatura consistente: "Módulo-Funcionalidad-Escenario X – Descripción específica". Incluir metadatos: Fecha, Modo (Manual), Prioridad (Alta/Media/Baja), Complejidad, Tipo de Caso (Positivo/Negativo), Tipo de Prueba (Funcional).

## 3. Confirmación Final

He internalizado esta guía de estilo y estoy listo para aplicarla con precisión en futuras solicitudes.

---
# Prompt 2
---
ROL
Actúa como un Ingeniero de Control de Calidad (QC) Senior, con una mentalidad meticulosa orientada a la verificación del producto y la detección de defectos. Tu especialidad es la creación de planes de prueba ejecutables y la deconstrucción de requisitos y prototipos visuales para asegurar que ninguna condición de fallo quede sin probar.

OBJETIVO
Generar un plan de verificación con casos de prueba ejecutables para la Historia de Usuario proporcionada. El objetivo es validar el cumplimiento funcional de cada Criterio de Aceptación y, crucialmente, detectar posibles defectos mediante un análisis sistemático de la HU y su prototipo visual.

CONTEXTO
A continuación se detalla toda la información necesaria para la creación del plan de verificación. Debes analizar tanto el texto como las imágenes que se proporcionarán.
-HU: Asignar Rol de Autoridad
Description
Como DGIP
Quiero asignar el rol de 'Autoridad' a profesores Para delegar la administración de facultades
Acceptance Criteria
Escenario 1 – Asignar rol 'Autoridad' exitosamente a profesor activo
Dado que estoy autenticado como DGIP en el sistema Y me encuentro en la página "Gestión de Usuarios y Roles" Y existe un profesor activo en la lista de usuarios, cuando hago clic en el botón "Asignar Rol" junto al profesor seleccionado Y selecciono el rol "Autoridad" del dropdown de roles disponibles Y confirmo la asignación, entonces se muestra el mensaje de confirmación "Rol asignado correctamente" Y la tabla se actualiza mostrando "Autoridad" en la columna "Rol" del profesor Y el profesor mantiene su estado "Activo" Y se registra la acción en el historial del sistema.
Escenario 2 – Intentar asignar rol a profesor inactivo Dado que estoy autenticado como DGIP Y me encuentro en la página "Gestión de Usuarios y Roles" Y existe un profesor con estado "Inactivo" en la lista, cuando intento hacer clic en el botón "Asignar Rol" junto al profesor inactivo, entonces se muestra el mensaje de error "No se puede asignar rol a usuario inactivo" Y no se habilita la funcionalidad de asignación Y el botón "Asignar Rol" permanece deshabilitado para ese usuario Y la tabla mantiene el estado "Inactivo" del profesor sin cambios.
Escenario 3 – Intentar asignar rol a profesor inexistente Dado que estoy autenticado como DGIP Y me encuentro en la página "Gestión de Usuarios y Roles", cuando busco un profesor que no existe en el sistema usando los filtros de búsqueda, entonces se muestra el mensaje "No se encontraron resultados" Y la tabla aparece vacía Y no se muestran opciones de asignación de roles Y los filtros de búsqueda permanecen disponibles para nueva consulta.
Escenario 4 – Acceso denegado por falta de permisos Dado que estoy autenticado con un rol diferente a DGIP Y intento acceder a la página "Gestión de Usuarios y Roles", cuando navego a la funcionalidad de asignación de roles, entonces se muestra el mensaje de error "No tiene permisos suficientes para realizar esta acción" Y no se muestra la opción "Asignar Rol" en la tabla de usuarios Y se mantiene visible la información de usuarios pero sin funcionalidades de modificación Y se sugiere contactar al administrador del sistema.
Escenario 5 – Acceso sin autenticación Dado que no tengo una sesión activa en el sistema, cuando intento acceder directamente a la URL de "Gestión de Usuarios y Roles", entonces soy redirigido automáticamente a la página de login "Bienvenido a SAGA EPN EUR-ACE" Y se muestran los campos "Email institucional" y "Contraseña" Y aparece el botón "Iniciar Sesión" Y se mantiene el enlace "¿Olvidaste tu contraseña?" Y debo autenticarme correctamente para acceder a la funcionalidad solicitada.

IMÁGENES DEL PROTOTIPO (Evidencia Visual) A continuación, se adjuntarán las imágenes del prototipo. Analízalas visualmente para identificar todos los puntos de verificación, comportamientos observables y posibles condiciones de error que deban ser probadas.
Sigue este proceso de 4 pasos con una mentalidad de QC:
1.  Análisis de Puntos de Verificación: Realiza un análisis combinado de la HU, cada Criterio de Aceptación y las imágenes del prototipo. De cada AC, deriva un caso de prueba específico. Un solo AC debe descomponerse en múltiples verificaciones atómicas (ej: una para el clic, una para el hover, una para el estado visual del icono, etc.).

Guia para el Uso del Reporte de Pruebas: Objetivo Monitorear el progreso de pruebas de un software desarrollado o adquirido por [Empresa] basado en GUIONES de prueba. Este reporte ayudara en el monitoreo del progreso de la prueba, la calidad de la prueba y el SLA para el arreglo en el desarrollo. Procedimiento
Para comenzar las pruebas, verifique que el guión esté completo.
Si existe suficiente informacion disponible del requisito, realice el plan detallado de qué tipo de casos de prueba tienen que ser probados.
Al planificarse pruebas para una fecha, planifique cuantos casos de prueba tienen que ser ejecutados por día para asegurarse de que las pruebas estén completamente terminadas dentro del periodo de tiempo establecido. Realizar la planificacion de las pruebas de tal forma que todos los casos sean probados al menos 1 dia antes de la fecha de fin de las pruebas.
Durante las pruebas, revise todos los dias si existen riesgos/dificultades/problemas que puedan parar/detener las pruebas. Documente los riesgos/dificultades/problemas para la revisión y tome las acciones apropiadas para reducir el riesgo de retraso del cronograma ó de baja calidad. Guia - General Si hay un control de cambios, este tiene que ser monitoreado de manera separada en el docuento de requisitos. Si el control de cambio es pequeño, puede ser planeado conjuntamente con la actualización del presente guión. Si hay muchos ciclos de pruebas de los mismos casos de pruebas, cada una tiene que ser planeada en una hora diferente por razones de monitoreo. HOJA DE TRABAJO - Guion Fecha Ejecucion Estimada: Ingresar la Fecha de Ejecucion estimada (DD-MM-AAAA) Modo Ejecucion: Detallar el tipo de ejecucion (Manual o Automatico) Prioridad Testing: Detallar la prioridad del caso (Alta, Media o Baja) Complejidad: Detallar la complejidad del caso (Alta, Media o Baja) Nombre Testing: USER STORY ID -USER STORY TITLE-NUMERO ESCENARIO Pre-Condiciones: Detallar los pre-requisitos requeridos antes de iniciar las pruebas funcionales Descripcion Caso: Describir brevemente la accion que se va a ejecutar Modulo: Describir el Modulo o Aplicativo a ser probado Rol: Describir el Rol del usuario ejecutor Nombre Paso: Número secuencial del paso a seguir en el caso de prueba (Paso 1, Paso 2, etc. ) Description Paso: Describir el paso a ejecutar Resultados Esperados: Describir el resultado esperado del paso ejecutado Resultados Obtenidos: Describir el resultado obtenido (Estado Prueba, Ok, Pendiente, Error, Desarcartado) Restricciones: Ingresar las restriciones para la ejecucion del paso Tipo de Prueba: Describir el tipo de prueba ejecutado (Funciona, No Funcional, Técnica) Observaciones: Describa las observaciones del caso
Cálculo de Fechas: Para la columna "Fecha Ejecución Estimada", utiliza la fecha del día siguiente a la fecha actual (si hoy es 25 de septiembre, usa 26 de septiembre de 2025).

Redacción de Casos de Prueba Ejecutables: Construye la tabla final. Asegúrate de que cada "Descripción Paso" sea una instrucción clara y ejecutable para un tester, y que cada "Resultado Esperado" sea una condición observable y binaria (el sistema pasa o falla la verificación).

FORMATO DE SALIDA
Presenta el resultado final en una única tabla Markdown, siguiendo la estructura y ejemplos aprendidos del excel analizado. El título debe reflejar que es un plan de verificación.
Por ejemplo: Plan de Verificación y Casos de Prueba para HU4: Seleccionar un RA**
(Fecha de ejecución estimada para todos los casos: 26 de septiembre de 2025)
| Fecha Ejecución Estimada | Modo Ejecución | Prioridad Testing | Complejidad | Nombre Testing | Pre-Condiciones | Descripción Caso | Módulo | Rol | Nombre Paso | Descripción Paso | Resultados Esperados | Resultados Obtenido | Restricciones | Tipo de Caso | Tipo de Prueba | Observaciones |

---
# Salida

---
**Plan de Verificación y Casos de Prueba para HU: Asignar Rol de Autoridad**
*(Fecha de ejecución estimada para todos los casos: 26 de septiembre de 2025)*

| Fecha Ejecución Estimada | Modo Ejecución | Prioridad Testing | Complejidad | Nombre Testing | Pre-Condiciones | Descripción Caso | Módulo | Rol | Nombre Paso | Descripción Paso | Resultados Esperados | Resultados Obtenido | Restricciones | Tipo de Caso | Tipo de Prueba | Observaciones |
|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|
| 2025-09-26 | Manual | Alta | Media | Asignar Rol Autoridad-Escenario 1 – Acceso a página de gestión | • El usuario debe estar autenticado como DGIP<br>• Debe existir al menos un profesor activo en el sistema<br>• El usuario debe tener permisos administrativos | Verificar que se pueda acceder correctamente a la página "Gestión de Usuarios y Roles" como DGIP | Gestión Usuarios y Roles | DGIP | Paso1 | FORMULARIO: Acceder al formulario "Gestión de Usuarios y Roles" desde el menú lateral | • Se carga correctamente la página "Gestión de Usuarios y Roles"<br>• Se muestra el título "Gestión de Usuarios y Roles"<br>• Se visualizan las pestañas "Usuarios" y "Roles"<br>• La pestaña "Usuarios" está activa por defecto | ESTADO PRUEBA |  | Positivo | Funcional |  |
|  |  |  |  |  |  |  |  |  | Paso2 | Verificar presencia de la tabla "Listado de Usuarios" | • Se muestra la tabla con las columnas: "Email", "Nombre", "Rol", "Estado", "Último Acceso", "Acciones"<br>• Se visualiza el campo "Buscar usuario..." en la parte superior<br>• Se muestran profesores existentes en la tabla<br>• Los datos se presentan organizados y estructurados | ESTADO PRUEBA |  |  |  |  |
|  |  |  |  |  |  |  |  |  | Paso3 | Confirmar presencia de profesores activos en la lista | • Se identifican profesores con estado "Activo" mostrado en color verde<br>• Cada profesor muestra información completa: email, nombre, rol actual<br>• Se visualizan botones de acción para cada usuario<br>• Los profesores activos tienen opciones de gestión disponibles | ESTADO PRUEBA |  |  |  |  |
| 2025-09-26 | Manual | Alta | Alta | Asignar Rol Autoridad-Escenario 1 – Proceso de asignación exitosa | • El usuario debe estar autenticado como DGIP<br>• Debe estar en la página "Gestión de Usuarios y Roles"<br>• Debe existir un profesor activo sin rol de Autoridad | Verificar que se pueda asignar exitosamente el rol "Autoridad" a un profesor activo | Gestión Usuarios y Roles | DGIP | Paso1 | Localizar un profesor activo en la tabla de usuarios | • Se identifica un profesor con estado "Activo" en color verde<br>• El profesor muestra información completa y actualizada<br>• Se confirma que el profesor no tiene rol "Autoridad" actualmente<br>• Los botones de acción están disponibles para ese usuario | ESTADO PRUEBA |  | Positivo | Funcional |  |
|  |  |  |  |  |  |  |  |  | Paso2 | Hacer clic en el botón "Asignar Rol" junto al profesor seleccionado | • Se ejecuta la acción de asignación de rol<br>• Se abre un dropdown o modal con opciones de roles disponibles<br>• Se muestra la opción "Autoridad" entre los roles disponibles<br>• La interfaz responde inmediatamente al clic | ESTADO PRUEBA |  |  |  |  |
|  |  |  |  |  |  |  |  |  | Paso3 | Seleccionar el rol "Autoridad" del dropdown de roles disponibles | • Se puede seleccionar la opción "Autoridad"<br>• La selección se registra visualmente<br>• Se habilitan opciones para confirmar la asignación<br>• No hay errores durante la selección | ESTADO PRUEBA |  |  |  |  |
|  |  |  |  |  |  |  |  |  | Paso4 | Confirmar la asignación del rol | • Se procesa exitosamente la asignación<br>• Se muestra el mensaje de confirmación "Rol asignado correctamente"<br>• El mensaje aparece claramente visible al usuario<br>• No se presentan errores durante el proceso | ESTADO PRUEBA |  |  |  |  |
|  |  |  |  |  |  |  |  |  | Paso5 | Verificar actualización de la tabla con el nuevo rol | • La tabla se actualiza automáticamente<br>• Se muestra "Autoridad" en la columna "Rol" del profesor<br>• El profesor mantiene su estado "Activo" en color verde<br>• Los cambios son visibles inmediatamente sin necesidad de recargar | ESTADO PRUEBA |  |  |  |  |
|  |  |  |  |  |  |  |  |  | Paso6 | Confirmar registro de la acción en el historial del sistema | • Se actualiza la información de "Último Acceso" apropiadamente<br>• Se registra la acción en el historial del sistema<br>• Se mantiene la integridad de los datos históricos<br>• La acción queda documentada para auditoría | ESTADO PRUEBA |  |  |  |  |
| 2025-09-26 | Manual | Media | Media | Asignar Rol Autoridad-Escenario 2 – Restricción para profesor inactivo | • El usuario debe estar autenticado como DGIP<br>• Debe estar en la página "Gestión de Usuarios y Roles"<br>• Debe existir un profesor con estado "Inactivo" en la lista | Verificar que no se permita asignar roles a profesores inactivos | Gestión Usuarios y Roles | DGIP | Paso1 | Localizar un profesor con estado "Inactivo" en la tabla de usuarios | • Se identifica un profesor con estado "Inactivo"<br>• El estado se muestra visualmente diferente al de usuarios activos<br>• El profesor aparece en la tabla con toda su información<br>• Se confirma que el profesor está marcado como inactivo | ESTADO PRUEBA |  | Negativo | Funcional |  |
|  |  |  |  |  |  |  |  |  | Paso2 | Intentar hacer clic en el botón "Asignar Rol" junto al profesor inactivo | • El botón "Asignar Rol" está deshabilitado o no responde<br>• Se muestra el mensaje de error "No se puede asignar rol a usuario inactivo"<br>• No se abre ningún dropdown o modal de selección<br>• La acción está claramente bloqueada para usuarios inactivos | ESTADO PRUEBA |  |  |  |  |
|  |  |  |  |  |  |  |  |  | Paso3 | Verificar que el botón permanece deshabilitado | • El botón "Asignar Rol" permanece deshabilitado consistentemente<br>• No se habilita la funcionalidad de asignación<br>• La restricción se mantiene durante toda la sesión<br>• No hay formas alternativas de asignar rol a usuarios inactivos | ESTADO PRUEBA |  |  |  |  |
|  |  |  |  |  |  |  |  |  | Paso4 | Confirmar que la tabla mantiene el estado sin cambios | • La tabla mantiene el estado "Inactivo" del profesor<br>• No se realizan modificaciones en la información del usuario<br>• El estado visual del profesor permanece inalterado<br>• No hay actualizaciones inadecuadas en los datos | ESTADO PRUEBA |  |  |  |  |
| 2025-09-26 | Manual | Media | Baja | Asignar Rol Autoridad-Escenario 3 – Búsqueda de profesor inexistente | • El usuario debe estar autenticado como DGIP<br>• Debe estar en la página "Gestión de Usuarios y Roles"<br>• Los filtros de búsqueda deben estar disponibles | Verificar que se maneje correctamente la búsqueda de profesores inexistentes | Gestión Usuarios y Roles | DGIP | Paso1 | Hacer clic en el campo "Buscar usuario..." e ingresar un nombre inexistente | • El campo de búsqueda está disponible y funcional<br>• Se puede ingresar texto normalmente<br>• El texto se muestra correctamente mientras se escribe<br>• No hay restricciones de caracteres inapropiadas | ESTADO PRUEBA |  | Negativo | Funcional |  |
|  |  |  |  |  |  |  |  |  | Paso2 | Ejecutar la búsqueda usando los filtros disponibles | • Se procesa la búsqueda sin errores del sistema<br>• La tabla se actualiza para mostrar los resultados<br>• No se producen errores técnicos durante el proceso<br>• La búsqueda se ejecuta en tiempo apropiado | ESTADO PRUEBA |  |  |  |  |
|  |  |  |  |  |  |  |  |  | Paso3 | Verificar mensaje "No se encontraron resultados" | • Se muestra el mensaje "No se encontraron resultados"<br>• La tabla aparece vacía sin filas de datos<br>• No se muestran opciones de asignación de roles<br>• Los encabezados de la tabla siguen visibles | ESTADO PRUEBA |  |  |  |  |
|  |  |  |  |  |  |  |  |  | Paso4 | Confirmar que los filtros permanecen disponibles | • Los filtros de búsqueda permanecen disponibles para nueva consulta<br>• Se puede realizar una nueva búsqueda<br>• El campo de búsqueda se puede limpiar y usar nuevamente<br>• La funcionalidad de búsqueda se mantiene operativa | ESTADO PRUEBA |  |  |  |  |
| 2025-09-26 | Manual | Alta | Media | Asignar Rol Autoridad-Escenario 4 – Acceso denegado por falta de permisos | • El usuario debe estar autenticado con un rol diferente a DGIP<br>• Debe intentar acceder a funcionalidades administrativas<br>• El sistema debe controlar permisos apropiadamente | Verificar que se deniegue el acceso a usuarios sin permisos suficientes | Gestión Usuarios y Roles | Profesor | Paso1 | Autenticarse en el sistema con un rol diferente a DGIP | • Se autentica exitosamente con credenciales de rol limitado<br>• Se carga el dashboard apropiado para el rol<br>• Se confirma que el usuario no tiene rol DGIP<br>• No se muestran opciones administrativas en el menú principal | ESTADO PRUEBA |  | Negativo | Seguridad |  |
|  |  |  |  |  |  |  |  |  | Paso2 | Intentar navegar a la página "Gestión de Usuarios y Roles" | • Se intenta acceder a la funcionalidad de gestión de usuarios<br>• El sistema evalúa los permisos del usuario actual<br>• Se detecta que el usuario no tiene permisos suficientes<br>• Se bloquea el acceso a la funcionalidad | ESTADO PRUEBA |  |  |  |  |
|  |  |  |  |  |  |  |  |  | Paso3 | Verificar mensaje de error "No tiene permisos suficientes" | • Se muestra el mensaje de error "No tiene permisos suficientes para realizar esta acción"<br>• El mensaje es claro e informativo<br>• Se sugiere contactar al administrador del sistema<br>• No se accede a la página de gestión de usuarios | ESTADO PRUEBA |  |  |  |  |
|  |  |  |  |  |  |  |  |  | Paso4 | Confirmar ausencia de opciones de "Asignar Rol" | • No se muestra la opción "Asignar Rol" en ninguna interfaz<br>• Las funcionalidades administrativas están completamente ocultas<br>• Se mantiene visible información básica sin opciones de modificación<br>• La interfaz refleja apropiadamente las limitaciones del rol | ESTADO PRUEBA |  |  |  |  |
| 2025-09-26 | Manual | Alta | Media | Asignar Rol Autoridad-Escenario 5 – Acceso sin autenticación | • No debe existir sesión activa en el navegador<br>• El sistema debe estar funcionando correctamente<br>• La URL de gestión debe estar disponible | Verificar redirección automática a login cuando se accede sin autenticación | Gestión Usuarios y Roles | No autenticado | Paso1 | Intentar acceder directamente a la URL "Gestión de Usuarios y Roles" sin autenticación | • Se redirige automáticamente a la página de login<br>• Se muestra la página "Iniciar Sesión"<br>• Se presenta el texto "Introduce tus credenciales para acceder a SAGA EPN EUR-ACE"<br>• No se accede a la funcionalidad solicitada | ESTADO PRUEBA |  | Negativo | Seguridad |  |
|  |  |  |  |  |  |  |  |  | Paso2 | Verificar elementos de la página de login | • Se muestran los campos "Correo Institucional" y "Contraseña"<br>• Se presenta el botón "Iniciar Sesión" en color azul<br>• Se muestra el enlace "¿Olvidaste tu contraseña?"<br>• Se visualiza el logo POLIACREDITA en la parte superior | ESTADO PRUEBA |  |  |  |  |
|  |  |  |  |  |  |  |  |  | Paso3 | Confirmar que se debe autenticar correctamente para acceder | • Los campos de login están disponibles para entrada de datos<br>• El botón "Iniciar Sesión" está funcional<br>• Se requiere autenticación válida para proceder<br>• No hay formas de saltarse la autenticación | ESTADO PRUEBA |  |  |  |  |
| 2025-09-26 | Manual | Baja | Baja | Asignar Rol Autoridad-Escenario 1 – Persistencia de cambios | • Debe haberse completado exitosamente una asignación de rol<br>• El usuario debe mantener acceso a la página<br>• La asignación debe estar confirmada en el sistema | Verificar que los cambios persistan después de recargar la página | Gestión Usuarios y Roles | DGIP | Paso1 | Recargar la página "Gestión de Usuarios y Roles" después de asignación exitosa | • La página se recarga completamente sin errores<br>• Se mantiene la autenticación del usuario<br>• La tabla de usuarios se carga nuevamente<br>• No hay pérdida de datos durante la recarga | ESTADO PRUEBA |  | Positivo | Integridad |  |
|  |  |  |  |  |  |  |  |  | Paso2 | Verificar que el rol "Autoridad" sigue asignado al profesor | • El profesor mantiene el rol "Autoridad" en la columna "Rol"<br>• El estado "Activo" se preserva correctamente<br>• La información es consistente con la asignación previa<br>• No se han perdido los cambios realizados | ESTADO PRUEBA |  |  |  |  |