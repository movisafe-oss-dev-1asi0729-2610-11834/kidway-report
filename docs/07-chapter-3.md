# **Chapter III: Requirements Specification**
## **3.1. User Stories**


|Epic/Story ID|Título|Descripción|Criterios de Aceptación|Relacionado con (Epic ID)|
|-------------|------|-----------|-----------------------|-------------------------|
|EP01|Registro digital de abordaje|Como conductor independiente, deseo registrar de forma rápida qué estudiantes suben o faltan en cada parada, para evitar errores y optimizar mi recorrido||
|EP02|Gestión de rutas|Como conductor independiente, deseo visualizar y seguir una ruta organizada con paradas definidas, para reducir tiempos de espera y consumo de combustible.||
|EP03|Registro de incidencias|Como conductor independiente, deseo registrar eventos como retrasos, ausencias o cambios en la ruta, para mantener trazabilidad del servicio.||
|EP04|Monitoreo de movilidades en tiempo real|Como administrador de empresa, deseo visualizar todas mis unidades en tiempo real, para supervisar el cumplimiento de rutas.||
|EP05|Reportes y trazabilidad|Como administrador de empresa, deseo generar reportes históricos de recorridos y desempeño, para evaluar el servicio y tomar decisiones.||
|EP06|Monitoreo institucional del transporte|Como institución educativa, deseo supervisar en tiempo real el recorrido de las unidades, para garantizar la seguridad del servicio.||
|EP07|Historial y evidencia de traslados|Como institución educativa, deseo contar con registros históricos de rutas y eventos, para respaldar la gestión ante incidentes.||
|US01|Visualizar lista de estudiantes por ruta|Como conductor, quiero ver la lista de estudiantes asignados a mi ruta, para saber a quién debo recoger.|Criterios de aceptación: <br>Se muestra lista ordenada por paradas. <br>Se visualiza nombre del estudiante y punto de recojo. <br>Solo aparecen estudiantes asignados a esa ruta|EP01|
|US02|Visualizar estudiantes por parada|Como conductor, quiero ver qué estudiantes corresponden a cada parada, para organizar el recojo.|Criterios de aceptación: <br>Agrupación por paradas. <br>Indicación clara de la parada actual. <br>Navegación simple entre paradas|EP01|
|US03|Registrar abordaje|Como conductor, quiero marcar rápidamente cuando un estudiante sube, para llevar control del traslado. |Criterios de aceptación: <br>Botón simple <br>Cambio visual inmediato. <br>Registro guardado automáticamente|EP01|
|US04|Registrar ausencia|Como conductor, quiero marcar cuando un estudiante no sube, para evitar esperas innecesarias. |Criterios de aceptación: <br>Opción “No subió” o “Ausente”. <br>Posibilidad de registrar motivo.  <br>Actualización en tiempo real|EP01|
|US05|Edición rápida de estado|Como conductor, quiero corregir el estado de un estudiante en caso de error, para mantener información precisa.|Criterios de aceptación: <br>Permite cambiar estado fácilmente. <br>Registra última actualización. <br>No requiere múltiples pasos. |EP01|
|US06|Funcionamiento offline|Como conductor, quiero poder registrar abordajes sin conexión a internet, para no depender de la señal.|Criterios de aceptación: <br>Permite registro sin conexión. <br>Sincroniza automáticamente al recuperar conexión. <br>No se pierde información.|EP01|
|US07|Confirmación visual rápida|Como conductor, quiero identificar rápidamente quién ya subió y quién no, para tomar decisiones rápidas.|Criterios de aceptación: <br>Código de colores <br>Vista clara y legible en movimiento. <br>Interfaz optimizada para uso rápido|EP01|
|US08|Visualizar ruta asignada|Como conductor, quiero visualizar la ruta asignada del día, para saber el orden de recorrido.|Criterios de aceptación: <br>Se muestra la ruta del día al iniciar la jornada. <br>Incluye lista de paradas en orden. <br>Solo se muestra la ruta asignada al conductor.|EP02|
|US09|Visualizar paradas en mapa|Como conductor, quiero ver las paradas de mi ruta en un mapa, para ubicarme fácilmente durante el recorrido.|Criterios de aceptación: <br>Se muestra mapa con puntos de parada. <br>Se visualiza ubicación actual del conductor. <br>Las paradas están claramente diferenciadas.|EP02|
|US10|Navegación entre paradas|Como conductor, quiero recibir indicaciones para llegar a cada parada, para optimizar mi recorrido.|Criterios de aceptación: <br>Se puede seleccionar la siguiente parada. <br>Se muestran indicaciones de navegación. <br>Se actualiza automáticamente al completar una parada.|EP02|
|US11|Marcar parada como completada|Como conductor, quiero marcar una parada como completada, para avanzar en mi ruta de forma ordenada.|Criterios de aceptación: <br>Existe opción para marcar parada completada. <br>La parada cambia de estado visualmente. <br>El sistema avanza a la siguiente parada.|EP02|
|US12|Reordenamiento básico de ruta|Como conductor, quiero ajustar el orden de paradas en caso de imprevistos, para adaptarme a cambios en el recorrido.|Criterios de aceptación: <br>Permite cambiar el orden de paradas. <br>Se actualiza la ruta en tiempo real. <br>No afecta el registro de estudiantes.|EP02|
|US13|Visualizar estado de la ruta|Como conductor, quiero ver el progreso de mi ruta, para saber cuánto falta completar.|Criterios de aceptación: <br>Se muestra porcentaje o número de paradas completadas. <br>Se diferencian paradas pendientes y completadas. <br>La información se actualiza en tiempo real.|EP02|
|US14|Funcionamiento offline de ruta|Como conductor, quiero acceder a mi ruta sin conexión a internet, para no depender de la señal.|Criterios de aceptación: <br>La ruta se carga previamente. <br>Se puede visualizar sin conexión. <br>Los cambios se sincronizan al recuperar conexión.|EP02|
|US15|Registrar incidencia rápida|Como conductor, quiero registrar una incidencia en pocos pasos, para no distraerme durante el recorrido.|Criterios de aceptación: <br>Existe botón visible de “Registrar incidencia”. <br>Permite seleccionar tipo de incidencia en 1–2 toques. <br>No requiere escribir obligatoriamente.|EP03|
|US16|Seleccionar tipo de incidencia|Como conductor, quiero elegir el tipo de incidencia, para clasificar correctamente el evento.|Criterios de aceptación: <br>Lista predefinida de tipos de incidencia. <br>Opciones claras y entendibles. <br>Permite seleccionar solo una opción principal.|EP03|
|US17|Registrar detalle opcional|Como conductor, quiero añadir un comentario opcional, para dar más contexto si es necesario.|Criterios de aceptación: <br>Campo de texto opcional. <br>No bloquea el registro si está vacío. <br>Guarda el comentario junto a la incidencia.|EP03|
|US18|Asociar incidencia a parada o estudiante|Como conductor, quiero vincular la incidencia a una parada o estudiante, para mayor precisión en el registro.|Criterios de aceptación: <br>Permite seleccionar parada o estudiante relacionado. <br>La asociación queda registrada. <br>Es opcional si no aplica.|EP03|
|US19|Registro automático de hora y ubicación|Como conductor, quiero que el sistema registre automáticamente la hora y ubicación, para no tener que hacerlo manualmente.|Criterios de aceptación: <br>Se guarda timestamp automático. <br>Se registra ubicación GPS. <br>No requiere intervención del usuario.|EP03|
|US20|Visualizar historial de incidencias|Como conductor, quiero ver las incidencias registradas, para hacer seguimiento del recorrido.|Criterios de aceptación: <br>Lista de incidencias del día. <br>Muestra tipo, hora y estado. <br>Ordenadas cronológicamente.|EP03|
|US21|Editar o corregir incidencia|Como conductor, quiero corregir una incidencia en caso de error, para mantener información precisa.|Criterios de aceptación: <br>Permite editar tipo o comentario. <br>Guarda cambios correctamente. <br>Mantiene registro actualizado.|EP03|
|US22|Funcionamiento offline de incidencias|Como conductor, quiero registrar incidencias sin conexión, para no depender de la red.|Criterios de aceptación: <br>Permite registrar sin internet. <br>Almacena localmente. <br>Sincroniza al recuperar conexión.|EP03|
|US23|Visualizar movilidades en mapa|Como administrador, quiero ver todas mis unidades en un mapa en tiempo real, para supervisar su ubicación.|Criterios de aceptación: <br>Se muestra mapa con todas las unidades activas. <br>Cada unidad tiene un identificador visible. <br>La ubicación se actualiza automáticamente.|EP04|
|US24|Visualizar detalle de unidad|Como administrador, quiero seleccionar una unidad y ver su información, para conocer su estado actual.|Criterios de aceptación: <br>Al seleccionar una unidad se muestra su información. <br>Incluye conductor, ruta asignada y estado. <br>La información está actualizada.|EP04|
|US25|Visualizar estado de unidades|Como administrador, quiero identificar el estado de cada unidad, para detectar problemas rápidamente.|Criterios de aceptación: <br>Estados visibles (en ruta, detenido, retrasado). <br>Código de colores para diferenciación. <br>Actualización en tiempo real.|EP04|
|US26|Filtrar unidades|Como administrador, quiero filtrar las unidades por estado o ruta, para enfocarme en lo relevante.|Criterios de aceptación: <br>Permite filtrar por estado. <br>Permite filtrar por ruta. <br>La vista se actualiza al aplicar filtros.|EP04|
|US27|Alertas de desviación|Como administrador, quiero recibir alertas cuando una unidad se desvíe de su ruta, para tomar acciones oportunas.|Criterios de aceptación: <br>Detecta desviaciones de ruta. <br>Genera alerta visual o notificación. <br>Indica qué unidad presenta el problema.|EP04|
|US28|Visualizar recorrido en tiempo real|Como administrador, quiero ver el recorrido que está realizando cada unidad, para validar el cumplimiento de la ruta.|Criterios de aceptación: <br>Se muestra trayectoria en el mapa. <br>Se actualiza conforme avanza la unidad. <br>Permite identificar el progreso.|EP04|
|US29|Historial reciente de ubicación|Como administrador, quiero consultar las ubicaciones recientes de una unidad, para analizar su comportamiento.|Criterios de aceptación: <br>Se muestran ubicaciones recientes. <br>Orden cronológico. <br>Accesible desde el detalle de la unidad.|EP04|
|US30|Actualización automática de datos|Como administrador, quiero que la información se actualice automáticamente, para no tener que recargar manualmente.|Criterios de aceptación: <br>Actualización en intervalos cortos. <br>No requiere recarga manual. <br>Se mostrará la hora donde fue la última actualización. <br>No interrumpe la navegación.|EP04||1|2|3|4|5|
|US31|Generar reporte de recorridos|Como administrador, quiero generar reportes de recorridos realizados, para analizar el cumplimiento de rutas.|Criterios de aceptación: <br>Permite generar reporte por rango de fechas. <br>Incluye rutas realizadas por unidad. <br>Se puede visualizar en pantalla.|EP05|
|US32|Generar reporte de desempeño|Como administrador, quiero visualizar métricas de desempeño de conductores y unidades, para evaluar la eficiencia operativa.|Criterios de aceptación: <br>Muestra métricas clave (tiempos, paradas completadas). <br>Información agrupada por conductor o unidad. <br>Datos claros y comprensibles.|EP05|
|US33|Exportar reportes|Como administrador, quiero exportar reportes, para compartirlos o analizarlos externamente.|Criterios de aceptación: <br>Permite exportar en formato PDF o Excel. <br>Descarga rápida del archivo. <br>Incluye la información seleccionada.|EP05|
|US34|Filtrar reportes|Como administrador, quiero aplicar filtros a los reportes, para enfocarme en información específica.|Criterios de aceptación: <br>Permite filtrar por fecha. <br>Permite filtrar por conductor o unidad. <br>La información se actualiza según filtros.|EP05|
|US35|Visualizar incidencias en reportes|Como administrador, quiero incluir incidencias en los reportes, para tener contexto completo del servicio.|Criterios de aceptación: <br>Se muestran incidencias registradas. <br>Asociadas a rutas o unidades. <br>Incluidas en reportes generados.|EP05|
|US36|Resumen general |Como administrador, quiero ver un resumen general del desempeño, para tomar decisiones rápidas.|Criterios de aceptación: <br>Muestra indicadores clave resumidos. <br>Vista simple y clara. <br>Actualización periódica.|EP05|
|US37|Descarga rápida de reportes recientes|Como administrador, quiero acceder rápidamente a reportes recientes, para ahorrar tiempo en consultas frecuentes.|Criterios de aceptación: <br>Lista de reportes recientes. <br>Acceso con un clic. <br>No requiere volver a generarlos.|EP05|
|US38|Visualizar unidades en tiempo real|Como institución educativa, quiero ver las unidades en un mapa en tiempo real, para supervisar su ubicación.|Criterios de aceptación: <br>Se muestra mapa con todas las unidades activas. <br>Cada unidad tiene identificación visible. <br>La ubicación se actualiza automáticamente.|EP06|
|US39|Visualizar detalle de unidad|Como institución educativa, quiero ver la información de cada unidad, para conocer su estado operativo.|Criterios de aceptación: <br>Se muestra conductor, ruta y estado. <br>Acceso al seleccionar una unidad. <br>Información actualizada en tiempo real.|EP06|
|US40|Visualizar cumplimiento de rutas|Como institución educativa, quiero verificar si las rutas se están cumpliendo, para asegurar el correcto servicio.|Criterios de aceptación: <br>Se muestra progreso de cada ruta. <br>Indica paradas completadas y pendientes. <br>Actualización en tiempo real.|EP06|
|US41|Alertas de retraso|Como institución educativa, quiero recibir alertas cuando una unidad presente retrasos, para tomar acciones oportunas.|Criterios de aceptación: <br>Detecta retrasos respecto a la ruta. <br>Genera alerta visual o notificación. <br>Identifica la unidad afectada.|EP06|
|US42|Visualizar incidencias en tiempo real|Como institución educativa, quiero ver incidencias registradas durante el recorrido, para tener control del servicio.|Criterios de aceptación: <br>Se muestran incidencias activas. <br>Asociadas a unidades o rutas. <br>Actualización inmediata.|EP06|
|US43|Filtrar unidades y rutas|Como institución educativa, quiero filtrar unidades o rutas, para enfocarme en información específica.|Criterios de aceptación: <br>Permite filtrar por ruta. <br>Permite filtrar por estado. <br>Vista se actualiza dinámicamente.|EP06|
|US44|Visualizar historial reciente|Como institución educativa, quiero consultar el historial reciente de recorridos, para validar el servicio.|Criterios de aceptación: <br>Acceso a recorridos recientes. <br>Orden cronológico. <br>Incluye información básica.|EP06|
|US45|Actualización automática del monitoreo|Como institución educativa, quiero que la información se actualice automáticamente, para no recargar manualmente.|Criterios de aceptación: <br>Actualización en tiempo real. <br>No requiere interacción del usuario. <br>No interrumpe la visualización.|EP06|
|US46|Visualizar historial de recorridos|Como institución educativa, quiero consultar el historial de recorridos realizados, para verificar el cumplimiento del servicio.|Criterios de aceptación: <br>Se muestra lista de recorridos pasados. <br>Ordenados por fecha. <br>Incluye información básica (ruta, unidad, conductor).|EP07|
|US47|Visualizar detalle de recorrido|Como institución educativa, quiero ver el detalle de un recorrido específico, para analizar lo sucedido.|Criterios de aceptación: <br>Muestra ruta completa realizada. <br>Incluye paradas y tiempos. <br>Información clara y organizada.|EP07|
|US48|Visualizar incidencias históricas|Como institución educativa, quiero consultar incidencias registradas en recorridos pasados, para tener contexto ante problemas.|Criterios de aceptación: <br>Lista de incidencias por recorrido. <br>Incluye tipo, hora y descripción. <br>Asociadas correctamente a rutas.|EP07|
|US49|Filtrar historial|Como institución educativa, quiero filtrar el historial por fechas, rutas o unidades, para encontrar información específica.|Criterios de aceptación: <br>Permite filtrar por fecha. <br>Permite filtrar por ruta o unidad. <br>Resultados se actualizan dinámicamente.|EP07|
|US50|Exportar historial|Como institución educativa, quiero exportar registros históricos, para respaldar información ante incidentes o auditorías.|Criterios de aceptación: <br>Permite exportar en PDF o Excel. <br>Incluye datos filtrados. <br>Descarga rápida del archivo.|EP07|
|US51|Registro de evidencia automática|Como institución educativa, quiero que el sistema registre automáticamente datos de cada recorrido, para no depender de procesos manuales.|Criterios de aceptación: <br>Se guarda información de rutas automáticamente. <br>Incluye hora, ubicación y eventos. <br>No requiere intervención del usuario.|EP07|
|US52|Consulta rápida de eventos|Como institución educativa, quiero acceder rápidamente a eventos relevantes, para responder ante incidentes.|Criterios de aceptación: <br>Lista de eventos importantes. <br>Acceso rápido desde panel. <br>Información clara y resumida.|EP07|

## **3.2. Impact Mapping**

![Impact Mapping](../assets/chapter-3/impact-mapping.jpg)

## **3.3. Product Backlog**

|Orden|User Story Id|Título|Descripción|Story Points|
|-----|-------------|------|-----------|------------|
|1|US08|Visualizar ruta asignada|Como conductor, quiero visualizar la ruta asignada del día, para saber el orden de recorrido.|3|
|2|US03|Registrar abordaje|Como conductor, quiero marcar rápidamente cuando un estudiante sube, para llevar control del traslado.|3|
|3|US23|Visualizar movilidades en mapa|Como administrador, quiero ver todas mis unidades en un mapa en tiempo real, para supervisar su ubicación.|5|
|4|US11|Marcar parada como completada|Como conductor, quiero marcar una parada como completada, para avanzar en mi ruta de forma ordenada.|2|
|5|US15|Registrar incidencia rápida|Como conductor, quiero registrar una incidencia en pocos pasos, para no distraerme durante el recorrido.|2|
|6|US25|Visualizar estado de unidades|Como administrador, quiero identificar el estado de cada unidad, para detectar problemas rápidamente.|3|
|7|US40|Visualizar cumplimiento de rutas|Como institución educativa, quiero verificar si las rutas se están cumpliendo, para asegurar el correcto servicio.|5|
|8|US31|Generar reporte de recorridos|Como administrador, quiero generar reportes de recorridos realizados, para analizar el cumplimiento de rutas.|5|
|9|US46|Visualizar historial de recorridos|Como institución educativa, quiero consultar el historial de recorridos realizados, para verificar el cumplimiento del servicio.|3|
|10|US33|Exportar reportes|Como administrador, quiero exportar reportes, para compartirlos o analizarlos externamente.|2|
|11|US09|Visualizar paradas en mapa|Como conductor, quiero ver las paradas de mi ruta en un mapa, para ubicarme fácilmente durante el recorrido.|3|
|12|US13|Visualizar estado de la ruta|Como conductor, quiero ver el progreso de mi ruta, para saber cuánto falta completar.|2|
|13|US24|Visualizar detalle de unidad|Como administrador, quiero seleccionar una unidad y ver su información, para conocer su estado actual.|3|
|14|US38|Visualizar unidades en tiempo real|Como institución educativa, quiero ver las unidades en un mapa en tiempo real, para supervisar su ubicación.|5|
|15|US42|Visualizar incidencias en tiempo real|Como institución educativa, quiero ver incidencias registradas durante el recorrido, para tener control del servicio.|3|
|16|US19|Registro automático de hora y ubicación|Como conductor, quiero que el sistema registre automáticamente la hora y ubicación, para no tener que hacerlo manualmente.|3|
|17|US16|Seleccionar tipo de incidencia|Como conductor, quiero elegir el tipo de incidencia, para clasificar correctamente el evento.|2|
|18|US18|Asociar incidencia a parada o estudiante|Como conductor, quiero vincular la incidencia a una parada o estudiante, para mayor precisión en el registro.|3|
|19|US20|Visualizar historial de incidencias|Como conductor, quiero ver las incidencias registradas, para hacer seguimiento del recorrido.|2|
|20|US30|Actualización automática de datos|Como administrador, quiero que la información se actualice automáticamente, para no tener que recargar manualmente.|3|
|21|US26|Filtrar unidades|Como administrador, quiero filtrar las unidades por estado o ruta, para enfocarme en lo relevante.|2|
|22|US41|Alertas de retraso|Como institución educativa, quiero recibir alertas cuando una unidad presente retrasos, para tomar acciones oportunas.|3|
|23|US28|Visualizar recorrido en tiempo real|Como administrador, quiero ver el recorrido que está realizando cada unidad, para validar el cumplimiento de la ruta.|5|
|24|US29|Historial reciente de ubicación|Como administrador, quiero consultar las ubicaciones recientes de una unidad, para analizar su comportamiento.|3|
|25|US32|Generar reporte de desempeño|Como administrador, quiero visualizar métricas de desempeño de conductores y unidades, para evaluar la eficiencia operativa.|5|
|26|US34|Filtrar reportes|Como administrador, quiero aplicar filtros a los reportes, para enfocarme en información específica.|2|
|27|US35|Visualizar incidencias en reportes|Como administrador, quiero incluir incidencias en los reportes, para tener contexto completo del servicio.|3|
|28|US36|Resumen general |Como administrador, quiero ver un resumen general del desempeño, para tomar decisiones rápidas.|3|
|29|US37|Descarga rápida de reportes recientes|Como administrador, quiero acceder rápidamente a reportes recientes, para ahorrar tiempo en consultas frecuentes.|3|
|30|US01|Visualizar lista de estudiantes por ruta|Como conductor, quiero ver la lista de estudiantes asignados a mi ruta, para saber a quién debo recoger.|3|
|31|US44|Visualizar historial reciente|Como institución educativa, quiero consultar el historial reciente de recorridos, para validar el servicio.|3|
|32|US45|Actualización automática del monitoreo|Como institución educativa, quiero que la información se actualice automáticamente, para no recargar manualmente.|2|
|39|US02|Visualizar estudiantes por parada|Como conductor, quiero ver qué estudiantes corresponden a cada parada, para organizar el recojo.|2|
|33|US47|Visualizar detalle de recorrido|Como institución educativa, quiero ver el detalle de un recorrido específico, para analizar lo sucedido.|3|
|34|US48|Visualizar incidencias históricas|Como institución educativa, quiero consultar incidencias registradas en recorridos pasados, para tener contexto ante problemas.|3|
|35|US49|Filtrar historial|Como institución educativa, quiero filtrar el historial por fechas, rutas o unidades, para encontrar información específica.|2|
|36|US50|Exportar historial|Como institución educativa, quiero exportar registros históricos, para respaldar información ante incidentes o auditorías.|2|
|37|US51|Registro de evidencia automática|Como institución educativa, quiero que el sistema registre automáticamente datos de cada recorrido, para no depender de procesos manuales.|5|
|38|US52|Consulta rápida de eventos|Como institución educativa, quiero acceder rápidamente a eventos relevantes, para responder ante incidentes.|2|
|40|US04|Registrar ausencia|Como conductor, quiero marcar cuando un estudiante no sube, para evitar esperas innecesarias.|2|
|41|US05|Edición rápida de estado|Como conductor, quiero corregir el estado de un estudiante en caso de error, para mantener información precisa.|2|
|42|US06|Funcionamiento offline|Como conductor, quiero poder registrar abordajes sin conexión a internet, para no depender de la señal.|5|
|43|US07|Confirmación visual rápida|Como conductor, quiero identificar rápidamente quién ya subió y quién no, para tomar decisiones rápidas.|2|
|44|US10|Navegación entre paradas|Como conductor, quiero recibir indicaciones para llegar a cada parada, para optimizar mi recorrido.|5|
|45|US12|Reordenamiento básico de ruta|Como conductor, quiero ajustar el orden de paradas en caso de imprevistos, para adaptarme a cambios en el recorrido.|5|
|46|US43|Filtrar unidades y rutas|Como institución educativa, quiero filtrar unidades o rutas, para enfocarme en información específica.|2|
|47|US14|Funcionamiento offline de ruta|Como conductor, quiero acceder a mi ruta sin conexión a internet, para no depender de la señal.|3|
|48|US17|Registrar detalle opcional|Como conductor, quiero añadir un comentario opcional, para dar más contexto si es necesario.|2|
|49|US21|Editar o corregir incidencia|Como conductor, quiero corregir una incidencia en caso de error, para mantener información precisa.|2|
|50|US22|Funcionamiento offline de incidencias|Como conductor, quiero registrar incidencias sin conexión, para no depender de la red.|2|
|51|US27|Alertas de desviación|Como administrador, quiero recibir alertas cuando una unidad se desvíe de su ruta, para tomar acciones oportunas.|5|
|52|US39|Visualizar detalle de unidad|Como institución educativa, quiero ver la información de cada unidad, para conocer su estado operativo.|2|