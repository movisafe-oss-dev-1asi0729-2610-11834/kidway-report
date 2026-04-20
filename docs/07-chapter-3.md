# **Chapter III: Requirements Specification**
## **3.1. User Stories**

# **Report Version Log**

<table style="width: 100%; border-collapse: collapse;">
  <!-- BARRA DE ARRIBA -->
  <tr>
    <th style="text-align: center;">Epic/Story ID</th>
    <th style="text-align: center;">Título</th>
    <th style="text-align: center;">Descripción</th>
    <th style="text-align: center;">Criterios de Aceptación</th>
    <th style="text-align: center;">Relacionado con (Epic ID)</th>
  </tr>

  <!-- EPICA 1 -->
  <tr>
    <td style="text-align: center;">
    EP01
    </td>
    <td style="text-align: center;">
    Registro digital de abordaje
    </td>
    <td style="text-align: center;">
    Como conductor independiente, deseo registrar de forma rápida qué estudiantes suben o faltan en cada parada, para evitar errores y optimizar mi recorrido
    </td>
    <td style="text-align: center;">
    </td>
    <td style="text-align: center;">
    </td>
  </tr>
  <!-- EPICA 2 -->
  <tr>
    <td style="text-align: center;">
    EP02
    </td>
    <td style="text-align: center;">
    Gestión de rutas
    </td>
    <td style="text-align: center;">
    Como conductor independiente, deseo visualizar y seguir una ruta organizada con paradas definidas, para reducir tiempos de espera y consumo de combustible.
    </td>
    <td style="text-align: center;">
    </td>
    <td style="text-align: center;">
    </td>
  </tr>
  <!-- EPICA 3 -->
  <tr>
    <td style="text-align: center;">
    EP03
    </td>
    <td style="text-align: center;">
    Registro de incidencias
    </td>
    <td style="text-align: center;">
    Como conductor independiente, deseo registrar eventos como retrasos, ausencias o cambios en la ruta, para mantener trazabilidad del servicio.
    </td>
    <td style="text-align: center;">
    </td>
    <td style="text-align: center;">
    </td>
  </tr>
  <!-- EPICA 4 -->
  <tr>
    <td style="text-align: center;">
    EP04
    </td>
    <td style="text-align: center;">
    Monitoreo de movilidades en tiempo real
    </td>
    <td style="text-align: center;">
    Como administrador de empresa, deseo visualizar todas mis unidades en tiempo real, para supervisar el cumplimiento de rutas.
    </td>
    <td style="text-align: center;">
    </td>
    <td style="text-align: center;">
    </td>
  </tr>

  <!-- EPICA 5 -->
  <tr>
    <td style="text-align: center;">
    EP05
    </td>
    <td style="text-align: center;">
    Reportes y trazabilidad
    </td>
    <td style="text-align: center;">
    Como administrador de empresa, deseo generar reportes históricos de recorridos y desempeño, para evaluar el servicio y tomar decisiones.
    </td>
    <td style="text-align: center;">
    </td>
    <td style="text-align: center;">
    </td>
  </tr>

  <!-- EPICA 6 -->
  <tr>
    <td style="text-align: center;">
    EP06
    </td>
    <td style="text-align: center;">
    Monitoreo institucional del transporte
    </td>
    <td style="text-align: center;">
    Como institución educativa, deseo supervisar en tiempo real el recorrido de las unidades, para garantizar la seguridad del servicio.
    </td>
    <td style="text-align: center;">
    </td>
    <td style="text-align: center;">
    </td>
  </tr>

  <!-- EPICA 7 -->
  <tr>
    <td style="text-align: center;">
    EP07
    </td>
    <td style="text-align: center;">
    Historial y evidencia de traslados
    </td>
    <td style="text-align: center;">
    Como institución educativa, deseo contar con registros históricos de rutas y eventos, para respaldar la gestión ante incidentes.
    </td>
    <td style="text-align: center;">
    </td>
    <td style="text-align: center;">
    </td>
  </tr>

  <!-- US 1 -->
  <tr>
    <td style="text-align: center;">
    US01
    </td>
    <td style="text-align: center;">
    Visualizar lista de estudiantes por ruta
    </td>
    <td style="text-align: center;">
    Como conductor, quiero ver la lista de estudiantes asignados a mi ruta, para saber a quién debo recoger.
    </td>
    <td style="text-align: center;">
    Criterios de aceptación: 
    <br>Se muestra lista ordenada por paradas. 
    <br>Se visualiza nombre del estudiante y punto de recojo. 
    <br>Solo aparecen estudiantes asignados a esa ruta
    </td>
    <td style="text-align: center;">
    EP01
    </td>
  </tr>
  <!-- US 2 -->
  <tr>
    <td style="text-align: center;">
    US02
    </td>
    <td style="text-align: center;">
    Visualizar estudiantes por parada
    </td>
    <td style="text-align: center;">
    Como conductor, quiero ver qué estudiantes corresponden a cada parada, para organizar el recojo.
    </td>
    <td style="text-align: center;">
    Criterios de aceptación: 
    <br>Agrupación por paradas. 
    <br>Indicación clara de la parada actual. 
    <br>Navegación simple entre paradas.
    </td>
    <td style="text-align: center;">
    EP01
    </td>
  </tr>
  <!-- US 3 -->
  <tr>
    <td style="text-align: center;">
    US03
    </td>
    <td style="text-align: center;">
    Registrar abordaje
    </td>
    <td style="text-align: center;">
    Como conductor, quiero marcar rápidamente cuando un estudiante sube, para llevar control del traslado.
    </td>
    <td style="text-align: center;">
    Criterios de aceptación: 
    <br>Botón simple 
    <br>Cambio visual inmediato. 
    <br>Registro guardado automáticamente
    </td>
    <td style="text-align: center;">
    EP01
    </td>
  </tr>

  <!-- US 4 -->
  <tr>
    <td style="text-align: center;">
    US04
    </td>
    <td style="text-align: center;">
    Registrar ausencia
    </td>
    <td style="text-align: center;">
    Como conductor, quiero marcar cuando un estudiante no sube, para evitar esperas innecesarias.
    </td>
    <td style="text-align: center;">
    Criterios de aceptación: 
    <br>Opción “No subió” o “Ausente”. 
    <br>Posibilidad de registrar motivo.  
    <br>Actualización en tiempo real
    </td>
    <td style="text-align: center;">
    EP01
    </td>
  </tr>

  <!-- US 5 -->
  <tr>
    <td style="text-align: center;">
    US05
    </td>
    <td style="text-align: center;">
    Edición rápida de estado
    </td>
    <td style="text-align: center;">
    Como conductor, quiero corregir el estado de un estudiante en caso de error, para mantener información precisa.
    </td>
    <td style="text-align: center;">
    Criterios de aceptación: 
    <br>Permite cambiar estado fácilmente. 
    <br>Registra última actualización. 
    <br>No requiere múltiples pasos. 
    </td>
    <td style="text-align: center;">
    EP01
    </td>
  </tr>

  <!-- US 6 -->
  <tr>
    <td style="text-align: center;">
    US06
    </td>
    <td style="text-align: center;">
    Funcionamiento offline
    </td>
    <td style="text-align: center;">
    Como conductor, quiero poder registrar abordajes sin conexión a internet, para no depender de la señal.
    </td>
    <td style="text-align: center;">
    Criterios de aceptación: 
    <br>Permite registro sin conexión. 
    <br>Sincroniza automáticamente al recuperar conexión. 
    <br>No se pierde información.
    </td>
    <td style="text-align: center;">
    EP01
    </td>
  </tr>

  <!-- US 7 -->
  <tr>
    <td style="text-align: center;">
    US07
    </td>
    <td style="text-align: center;">
    Confirmación visual rápida
    </td>
    <td style="text-align: center;">
    Como conductor, quiero identificar rápidamente quién ya subió y quién no, para tomar decisiones rápidas.
    </td>
    <td style="text-align: center;">
    Criterios de aceptación: 
    <br>Código de colores 
    <br>Vista clara y legible en movimiento. 
    <br>Interfaz optimizada para uso rápido
    </td>
    <td style="text-align: center;">
    EP01
    </td>
  </tr>

  <!-- US 8 -->
  <tr>
    <td style="text-align: center;">
    US08
    </td>
    <td style="text-align: center;">
    Visualizar ruta asignada
    </td>
    <td style="text-align: center;">
    Como conductor, quiero visualizar la ruta asignada del día, para saber el orden de recorrido.
    </td>
    <td style="text-align: center;">
    Criterios de aceptación: 
    <br>Se muestra la ruta del día al iniciar la jornada. 
    <br>Incluye lista de paradas en orden. 
    <br>Solo se muestra la ruta asignada al conductor.
    </td>
    <td style="text-align: center;">
    EP02
    </td>
  </tr>

  <!-- US 9 -->
  <tr>
    <td style="text-align: center;">
    US09
    </td>
    <td style="text-align: center;">
    Visualizar paradas en mapa
    </td>
    <td style="text-align: center;">
    Como conductor, quiero ver las paradas de mi ruta en un mapa, para ubicarme fácilmente durante el recorrido.
    </td>
    <td style="text-align: center;">
    Criterios de aceptación:
    <br>Se muestra mapa con puntos de parada. 
    <br>Se visualiza ubicación actual del conductor. 
    <br>Las paradas están claramente diferenciadas.
    </td>
    <td style="text-align: center;">
    EP02
    </td>
  </tr>

  <!-- US 10 -->
  <tr>
    <td style="text-align: center;">
    US10
    </td>
    <td style="text-align: center;">
    Navegación entre paradas
    </td>
    <td style="text-align: center;">
    Como conductor, quiero recibir indicaciones para llegar a cada parada, para optimizar mi recorrido.
    </td>
    <td style="text-align: center;">
    Criterios de aceptación: 
    <br>Se puede seleccionar la siguiente parada. 
    <br>Se muestran indicaciones de navegación. 
    <br>Se actualiza automáticamente al completar una parada.
    </td>
    <td style="text-align: center;">
    EP02
    </td>
  </tr>

  <!-- US 11 -->
  <tr>
    <td style="text-align: center;">
    US11
    </td>
    <td style="text-align: center;">
    Marcar parada como completada
    </td>
    <td style="text-align: center;">
    Como conductor, quiero marcar una parada como completada, para avanzar en mi ruta de forma ordenada.
    </td>
    <td style="text-align: center;">
    Criterios de aceptación: 
    <br>Existe opción para marcar parada completada. 
    <br>La parada cambia de estado visualmente. 
    <br>El sistema avanza a la siguiente parada.
    </td>
    <td style="text-align: center;">
    EP02
    </td>
  </tr>

  <!-- US 12 -->
  <tr>
    <td style="text-align: center;">
    US12
    </td>
    <td style="text-align: center;">
    Reordenamiento básico de ruta
    </td>
    <td style="text-align: center;">
    Como conductor, quiero ajustar el orden de paradas en caso de imprevistos, para adaptarme a cambios en el recorrido.
    </td>
    <td style="text-align: center;">
    Criterios de aceptación: 
    <br>Permite cambiar el orden de paradas. 
    <br>Se actualiza la ruta en tiempo real. 
    <br>No afecta el registro de estudiantes.
    </td>
    <td style="text-align: center;">
    EP02
    </td>
  </tr>

  <!-- US 13 -->
  <tr>
    <td style="text-align: center;">
    US13
    </td>
    <td style="text-align: center;">
    Visualizar estado de la ruta
    </td>
    <td style="text-align: center;">
    Como conductor, quiero ver el progreso de mi ruta, para saber cuánto falta completar.
    </td>
    <td style="text-align: center;">
    Criterios de aceptación: 
    <br>Se muestra porcentaje o número de paradas completadas.
    <br>Se diferencian paradas pendientes y completadas.
    <br>La información se actualiza en tiempo real.
    </td>
    <td style="text-align: center;">
    EP02
    </td>
  </tr>

  <!-- US 14 -->
  <tr>
    <td style="text-align: center;">
    US14
    </td>
    <td style="text-align: center;">
    Funcionamiento offline de ruta
    </td>
    <td style="text-align: center;">
    Como conductor, quiero acceder a mi ruta sin conexión a internet, para no depender de la señal.
    </td>
    <td style="text-align: center;">
    Criterios de aceptación: 
    <br>La ruta se carga previamente. 
    <br>Se puede visualizar sin conexión. 
    <br>Los cambios se sincronizan al recuperar conexión.
    </td>
    <td style="text-align: center;">
    EP02
    </td>
  </tr>

  <!-- US 15 -->
|US15|||EP03|
  <tr>
    <td style="text-align: center;">
    US15
    </td>
    <td style="text-align: center;">
    Registrar incidencia rápida
    </td>
    <td style="text-align: center;">
    Como conductor, quiero registrar una incidencia en pocos pasos, para no distraerme durante el recorrido.
    </td>
    <td style="text-align: center;">
    Criterios de aceptación: 
    <br>Existe botón visible de “Registrar incidencia”. 
    <br>Permite seleccionar tipo de incidencia en 1–2 toques. 
    <br>No requiere escribir obligatoriamente.|
    <td style="text-align: center;">
    EP03
    </td>
  </tr>

  <!-- US 16 -->
  <tr>
    <td style="text-align: center;">
    US16
    </td>
    <td style="text-align: center;">
    Seleccionar tipo de incidencia
    </td>
    <td style="text-align: center;">
    Como conductor, quiero elegir el tipo de incidencia, para clasificar correctamente el evento.
    </td>
    <td style="text-align: center;">
    Criterios de aceptación: 
    <br>Lista predefinida de tipos de incidencia. 
    <br>Opciones claras y entendibles. 
    <br>Permite seleccionar solo una opción principal.
    </td>
    <td style="text-align: center;">
    EP03
    </td>
  </tr>

  <!-- US 17 -->
  <tr>
    <td style="text-align: center;">
    US17
    </td>
    <td style="text-align: center;">
    Registrar detalle opcional
    </td>
    <td style="text-align: center;">
    Como conductor, quiero añadir un comentario opcional, para dar más contexto si es necesario.
    </td>
    <td style="text-align: center;">
    Criterios de aceptación: 
    <br>Campo de texto opcional. 
    <br>No bloquea el registro si está vacío. 
    <br>Guarda el comentario junto a la incidencia.
    </td>
    <td style="text-align: center;">
    EP03
    </td>
  </tr>
  
  <!-- US 18 -->
  <tr>
    <td style="text-align: center;">
    US18
    </td>
    <td style="text-align: center;">
    Asociar incidencia a parada o estudiante
    </td>
    <td style="text-align: center;">
    Como conductor, quiero vincular la incidencia a una parada o estudiante, para mayor precisión en el registro.
    </td>
    <td style="text-align: center;">
    Criterios de aceptación:
    <br>Permite seleccionar parada o estudiante relacionado. 
    <br>La asociación queda registrada. 
    <br>Es opcional si no aplica.
    </td>
    <td style="text-align: center;">
    EP03
    </td>
  </tr>

  <!-- US 19 -->
  <tr>
    <td style="text-align: center;">
    US19
    </td>
    <td style="text-align: center;">
    Registro automático de hora y ubicación
    </td>
    <td style="text-align: center;">
    Como conductor, quiero que el sistema registre automáticamente la hora y ubicación, para no tener que hacerlo manualmente.
    </td>
    <td style="text-align: center;">
    Criterios de aceptación: 
    <br>Se guarda timestamp automático. 
    <br>Se registra ubicación GPS. 
    <br>No requiere intervención del usuario.
    </td>
    <td style="text-align: center;">
    EP03
    </td>
  </tr>
  
  <!-- US 20 -->
  <tr>
    <td style="text-align: center;">
    US20
    </td>
    <td style="text-align: center;">
    Visualizar historial de incidencias
    </td>
    <td style="text-align: center;">
    Como conductor, quiero ver las incidencias registradas, para hacer seguimiento del recorrido.
    </td>
    <td style="text-align: center;">
    Criterios de aceptación: 
    <br>Lista de incidencias del día. 
    <br>Muestra tipo, hora y estado. 
    <br>Ordenadas cronológicamente.
    </td>
    <td style="text-align: center;">
    EP03
    </td>
  </tr>

  <!-- US 21 -->
  <tr>
    <td style="text-align: center;">
    US21
    </td>
    <td style="text-align: center;">
    Editar o corregir incidencia
    </td>
    <td style="text-align: center;">
    Como conductor, quiero corregir una incidencia en caso de error, para mantener información precisa.
    </td>
    <td style="text-align: center;">C
    riterios de aceptación: 
    <br>Permite editar tipo o comentario. 
    <br>Guarda cambios correctamente. 
    <br>Mantiene registro actualizado.
    </td>
    <td style="text-align: center;">
    EP01
    </td>
  </tr>

  <!-- US 22 -->
  <tr>
    <td style="text-align: center;">
    US22
    </td>
    <td style="text-align: center;">
    Funcionamiento offline de incidencias
    </td>
    <td style="text-align: center;">
    Como conductor, quiero registrar incidencias sin conexión, para no depender de la red.
    </td>
    <td style="text-align: center;">
    Criterios de aceptación: 
    <br>Permite registrar sin internet. 
    <br>Almacena localmente. 
    <br>Sincroniza al recuperar conexión.
    </td>
    <td style="text-align: center;">
    EP03
    </td>
  </tr>

  <!-- US 23 -->
  <tr>
    <td style="text-align: center;">
    US023
    </td>
    <td style="text-align: center;">
    Visualizar movilidades en mapa
    </td>
    <td style="text-align: center;">
    Como administrador, quiero ver todas mis unidades en un mapa en tiempo real, para supervisar su ubicación.
    </td>
    <td style="text-align: center;">
    Criterios de aceptación: 
    <br>Se muestra mapa con todas las unidades activas. 
    <br>Cada unidad tiene un identificador visible. 
    <br>La ubicación se actualiza automáticamente.
    </td>
    <td style="text-align: center;">
    EP04
    </td>
  </tr>

  <!-- US 24 -->
  <tr>
    <td style="text-align: center;">
    US24
    </td>
    <td style="text-align: center;">
    Visualizar detalle de unidad
    </td>
    <td style="text-align: center;">
    Como administrador, quiero seleccionar una unidad y ver su información, para conocer su estado actual.
    </td>
    <td style="text-align: center;">
    Criterios de aceptación: 
    <br>Al seleccionar una unidad se muestra su información. 
    <br>Incluye conductor, ruta asignada y estado.
    <br>La información está actualizada.
    </td>
    <td style="text-align: center;">
    EP04
    </td>
  </tr>

  <!-- US 25 -->
  <tr>
    <td style="text-align: center;">
    US25
    </td>
    <td style="text-align: center;">
    Visualizar estado de unidades
    </td>
    <td style="text-align: center;">
    Como administrador, quiero identificar el estado de cada unidad, para detectar problemas rápidamente.
    </td>
    <td style="text-align: center;">
    Criterios de aceptación: 
    <br>Estados visibles (en ruta, detenido, retrasado). 
    <br>Código de colores para diferenciación. 
    <br>Actualización en tiempo real.
    </td>
    <td style="text-align: center;">
    EP04
    </td>
  </tr>

  <!-- US 26 -->
  <tr>
    <td style="text-align: center;">
    US26
    </td>
    <td style="text-align: center;">
    Filtrar unidades
    </td>
    <td style="text-align: center;">
    Como administrador, quiero filtrar las unidades por estado o ruta, para enfocarme en lo relevante.
    <td style="text-align: center;">
    Criterios de aceptación: 
    <br>Permite filtrar por estado. 
    <br>Permite filtrar por ruta. 
    <br>La vista se actualiza al aplicar filtros.
    </td>
    <td style="text-align: center;">
    EP04
    </td>
  </tr>

  <!-- US 27 -->
  <tr>
    <td style="text-align: center;">
    US27
    </td>
    <td style="text-align: center;">
    Alertas de desviación
    </td>
    <td style="text-align: center;">
    Como administrador, quiero recibir alertas cuando una unidad se desvíe de su ruta, para tomar acciones oportunas.
    </td>
    <td style="text-align: center;">
    Criterios de aceptación: 
    <br>Detecta desviaciones de ruta. 
    <br>Genera alerta visual o notificación. 
    <br>Indica qué unidad presenta el problema.
    </td>
    <td style="text-align: center;">
    EP04
    </td>
  </tr>

  <!-- US 28 -->
  <tr>
    <td style="text-align: center;">
    US28
    </td>
    <td style="text-align: center;">
    Visualizar recorrido en tiempo real
    </td>
    <td style="text-align: center;">
    Como administrador, quiero ver el recorrido que está realizando cada unidad, para validar el cumplimiento de la ruta.
    </td>
    <td style="text-align: center;">
    Criterios de aceptación: 
    <br>Se muestra trayectoria en el mapa. 
    <br>Se actualiza conforme avanza la unidad. 
    <br>Permite identificar el progreso.
    </td>
    <td style="text-align: center;">
    EP04
    </td>
  </tr>

  <!-- US 29 -->
  <tr>
    <td style="text-align: center;">
    US29
    </td>
    <td style="text-align: center;">
    Historial reciente de ubicación
    </td>
    <td style="text-align: center;">
    Como administrador, quiero consultar las ubicaciones recientes de una unidad, para analizar su comportamiento.
    </td>
    <td style="text-align: center;">
    Criterios de aceptación: 
    <br>Se muestran ubicaciones recientes. 
    <br>Orden cronológico. 
    <br>Accesible desde el detalle de la unidad.
    </td>
    <td style="text-align: center;">
    EP04
    </td>
  </tr>

  <!-- US 30 -->
  <tr>
    <td style="text-align: center;">
    US30
    </td>
    <td style="text-align: center;">
    Actualización automática de datos
    </td>
    <td style="text-align: center;">
    Como administrador, quiero que la información se actualice automáticamente, para no tener que recargar manualmente.
    </td>
    <td style="text-align: center;">
    Criterios de aceptación: 
    <br>Actualización en intervalos cortos. 
    <br>No requiere recarga manual. 
    <br>Se mostrará la hora donde fue la última actualización. 
    <br>No interrumpe la navegación.
    </td>
    <td style="text-align: center;">
    EP04
    </td>
  </tr>

  <!-- US 31 -->
  <tr>
    <td style="text-align: center;">
    US31
    </td>
    <td style="text-align: center;">
    Generar reporte de recorridos
    </td>
    <td style="text-align: center;">
    Como administrador, quiero generar reportes de recorridos realizados, para analizar el cumplimiento de rutas.
    </td>
    <td style="text-align: center;">
    Criterios de aceptación: 
    <br>Permite generar reporte por rango de fechas. 
    <br>Incluye rutas realizadas por unidad. 
    <br>Se puede visualizar en pantalla.
    </td>
    <td style="text-align: center;">
    EP05
    </td>
  </tr>

  <!-- US 32 -->
|US32|Generar reporte de desempeño|Como administrador, quiero visualizar métricas de desempeño de conductores y unidades, para evaluar la eficiencia operativa.|Criterios de aceptación: <br>Muestra métricas clave (tiempos, paradas completadas). <br>Información agrupada por conductor o unidad. <br>Datos claros y comprensibles.|EP05|
  <tr>
    <td style="text-align: center;">
    US32
    </td>
    <td style="text-align: center;">
    Confirmación visual rápida
    </td>
    <td style="text-align: center;">
    Como conductor, quiero identificar rápidamente quién ya subió y quién no, para tomar decisiones rápidas.
    </td>
    <td style="text-align: center;">
    Criterios de aceptación: 
    <br>Código de colores 
    <br>Vista clara y legible en movimiento. 
    <br>Interfaz optimizada para uso rápido
    </td>
    <td style="text-align: center;">
    EP05
    </td>
  </tr>

  <!-- US 33 -->
|US33|Exportar reportes|Como administrador, quiero exportar reportes, para compartirlos o analizarlos externamente.|Criterios de aceptación: <br>Permite exportar en formato PDF o Excel. <br>Descarga rápida del archivo. <br>Incluye la información seleccionada.|EP05|
  <tr>
    <td style="text-align: center;">
    US33
    </td>
    <td style="text-align: center;">
    Confirmación visual rápida
    </td>
    <td style="text-align: center;">
    Como conductor, quiero identificar rápidamente quién ya subió y quién no, para tomar decisiones rápidas.
    </td>
    <td style="text-align: center;">
    Criterios de aceptación: 
    <br>Código de colores 
    <br>Vista clara y legible en movimiento. 
    <br>Interfaz optimizada para uso rápido
    </td>
    <td style="text-align: center;">
    EP05
    </td>
  </tr>

  <!-- US 34 -->
|US34|Filtrar reportes|Como administrador, quiero aplicar filtros a los reportes, para enfocarme en información específica.|Criterios de aceptación: <br>Permite filtrar por fecha. <br>Permite filtrar por conductor o unidad. <br>La información se actualiza según filtros.|EP05|
  <tr>
    <td style="text-align: center;">
    US34
    </td>
    <td style="text-align: center;">
    Confirmación visual rápida
    </td>
    <td style="text-align: center;">
    Como conductor, quiero identificar rápidamente quién ya subió y quién no, para tomar decisiones rápidas.
    </td>
    <td style="text-align: center;">
    Criterios de aceptación: 
    <br>Código de colores 
    <br>Vista clara y legible en movimiento. 
    <br>Interfaz optimizada para uso rápido
    </td>
    <td style="text-align: center;">
    EP05
    </td>
  </tr>

  <!-- US 35 -->
|US35|Visualizar incidencias en reportes|Como administrador, quiero incluir incidencias en los reportes, para tener contexto completo del servicio.|Criterios de aceptación: <br>Se muestran incidencias registradas. <br>Asociadas a rutas o unidades. <br>Incluidas en reportes generados.|EP05|
  <tr>
    <td style="text-align: center;">
    US35
    </td>
    <td style="text-align: center;">
    Confirmación visual rápida
    </td>
    <td style="text-align: center;">
    Como conductor, quiero identificar rápidamente quién ya subió y quién no, para tomar decisiones rápidas.
    </td>
    <td style="text-align: center;">
    Criterios de aceptación: 
    <br>Código de colores 
    <br>Vista clara y legible en movimiento. 
    <br>Interfaz optimizada para uso rápido
    </td>
    <td style="text-align: center;">
    EP05
    </td>
  </tr>

  <!-- US 36 -->
|US36|Resumen general |Como administrador, quiero ver un resumen general del desempeño, para tomar decisiones rápidas.|Criterios de aceptación: <br>Muestra indicadores clave resumidos. <br>Vista simple y clara. <br>Actualización periódica.|EP05|
  <tr>
    <td style="text-align: center;">
    US36
    </td>
    <td style="text-align: center;">
    Confirmación visual rápida
    </td>
    <td style="text-align: center;">
    Como conductor, quiero identificar rápidamente quién ya subió y quién no, para tomar decisiones rápidas.
    </td>
    <td style="text-align: center;">
    Criterios de aceptación: 
    <br>Código de colores 
    <br>Vista clara y legible en movimiento. 
    <br>Interfaz optimizada para uso rápido
    </td>
    <td style="text-align: center;">
    EP05
    </td>
  </tr>

  <!-- US 37 -->
|US37|Descarga rápida de reportes recientes|Como administrador, quiero acceder rápidamente a reportes recientes, para ahorrar tiempo en consultas frecuentes.|Criterios de aceptación: <br>Lista de reportes recientes. <br>Acceso con un clic. <br>No requiere volver a generarlos.|EP05|
  <tr>
    <td style="text-align: center;">
    US37
    </td>
    <td style="text-align: center;">
    Confirmación visual rápida
    </td>
    <td style="text-align: center;">
    Como conductor, quiero identificar rápidamente quién ya subió y quién no, para tomar decisiones rápidas.
    </td>
    <td style="text-align: center;">
    Criterios de aceptación: 
    <br>Código de colores 
    <br>Vista clara y legible en movimiento. 
    <br>Interfaz optimizada para uso rápido
    </td>
    <td style="text-align: center;">
    EP05
    </td>
  </tr>

  <!-- US 38 -->
|US38|Visualizar unidades en tiempo real|Como institución educativa, quiero ver las unidades en un mapa en tiempo real, para supervisar su ubicación.|Criterios de aceptación: <br>Se muestra mapa con todas las unidades activas. <br>Cada unidad tiene identificación visible. <br>La ubicación se actualiza automáticamente.|EP06|
  <tr>
    <td style="text-align: center;">
    US38
    </td>
    <td style="text-align: center;">
    Confirmación visual rápida
    </td>
    <td style="text-align: center;">
    Como conductor, quiero identificar rápidamente quién ya subió y quién no, para tomar decisiones rápidas.
    </td>
    <td style="text-align: center;">
    Criterios de aceptación: 
    <br>Código de colores 
    <br>Vista clara y legible en movimiento. 
    <br>Interfaz optimizada para uso rápido
    </td>
    <td style="text-align: center;">
    EP06
    </td>
  </tr>

  <!-- US 39 -->
|US39|Visualizar detalle de unidad|Como institución educativa, quiero ver la información de cada unidad, para conocer su estado operativo.|Criterios de aceptación: <br>Se muestra conductor, ruta y estado. <br>Acceso al seleccionar una unidad. <br>Información actualizada en tiempo real.|EP06|
  <tr>
    <td style="text-align: center;">
    US39
    </td>
    <td style="text-align: center;">
    Confirmación visual rápida
    </td>
    <td style="text-align: center;">
    Como conductor, quiero identificar rápidamente quién ya subió y quién no, para tomar decisiones rápidas.
    </td>
    <td style="text-align: center;">
    Criterios de aceptación: 
    <br>Código de colores 
    <br>Vista clara y legible en movimiento. 
    <br>Interfaz optimizada para uso rápido
    </td>
    <td style="text-align: center;">
    EP06
    </td>
  </tr>

  <!-- US 40 -->
|US40|Visualizar cumplimiento de rutas|Como institución educativa, quiero verificar si las rutas se están cumpliendo, para asegurar el correcto servicio.|Criterios de aceptación: <br>Se muestra progreso de cada ruta. <br>Indica paradas completadas y pendientes. <br>Actualización en tiempo real.|EP06|
  <tr>
    <td style="text-align: center;">
    US40
    </td>
    <td style="text-align: center;">
    Confirmación visual rápida
    </td>
    <td style="text-align: center;">
    Como conductor, quiero identificar rápidamente quién ya subió y quién no, para tomar decisiones rápidas.
    </td>
    <td style="text-align: center;">
    Criterios de aceptación: 
    <br>Código de colores 
    <br>Vista clara y legible en movimiento. 
    <br>Interfaz optimizada para uso rápido
    </td>
    <td style="text-align: center;">
    EP06
    </td>
  </tr>

  <!-- US 41 -->
|US41|Alertas de retraso|Como institución educativa, quiero recibir alertas cuando una unidad presente retrasos, para tomar acciones oportunas.|Criterios de aceptación: <br>Detecta retrasos respecto a la ruta. <br>Genera alerta visual o notificación. <br>Identifica la unidad afectada.|EP06|
  <tr>
    <td style="text-align: center;">
    US41
    </td>
    <td style="text-align: center;">
    Confirmación visual rápida
    </td>
    <td style="text-align: center;">
    Como conductor, quiero identificar rápidamente quién ya subió y quién no, para tomar decisiones rápidas.
    </td>
    <td style="text-align: center;">
    Criterios de aceptación: 
    <br>Código de colores 
    <br>Vista clara y legible en movimiento. 
    <br>Interfaz optimizada para uso rápido
    </td>
    <td style="text-align: center;">
    EP06
    </td>
  </tr>

  <!-- US 42 -->
|US42|Visualizar incidencias en tiempo real|Como institución educativa, quiero ver incidencias registradas durante el recorrido, para tener control del servicio.|Criterios de aceptación: <br>Se muestran incidencias activas. <br>Asociadas a unidades o rutas. <br>Actualización inmediata.|EP06|
  <tr>
    <td style="text-align: center;">
    US42
    </td>
    <td style="text-align: center;">
    Confirmación visual rápida
    </td>
    <td style="text-align: center;">
    Como conductor, quiero identificar rápidamente quién ya subió y quién no, para tomar decisiones rápidas.
    </td>
    <td style="text-align: center;">
    Criterios de aceptación: 
    <br>Código de colores 
    <br>Vista clara y legible en movimiento. 
    <br>Interfaz optimizada para uso rápido
    </td>
    <td style="text-align: center;">
    EP06
    </td>
  </tr>

  <!-- US 43 -->
|US43|Filtrar unidades y rutas|Como institución educativa, quiero filtrar unidades o rutas, para enfocarme en información específica.|Criterios de aceptación: <br>Permite filtrar por ruta. <br>Permite filtrar por estado. <br>Vista se actualiza dinámicamente.|EP06|
  <tr>
    <td style="text-align: center;">
    US43
    </td>
    <td style="text-align: center;">
    Confirmación visual rápida
    </td>
    <td style="text-align: center;">
    Como conductor, quiero identificar rápidamente quién ya subió y quién no, para tomar decisiones rápidas.
    </td>
    <td style="text-align: center;">
    Criterios de aceptación: 
    <br>Código de colores 
    <br>Vista clara y legible en movimiento. 
    <br>Interfaz optimizada para uso rápido
    </td>
    <td style="text-align: center;">
    EP06
    </td>
  </tr>

  <!-- US 44 -->
|US44|Visualizar historial reciente|Como institución educativa, quiero consultar el historial reciente de recorridos, para validar el servicio.|Criterios de aceptación: <br>Acceso a recorridos recientes. <br>Orden cronológico. <br>Incluye información básica.|EP06|
  <tr>
    <td style="text-align: center;">
    US44
    </td>
    <td style="text-align: center;">
    Confirmación visual rápida
    </td>
    <td style="text-align: center;">
    Como conductor, quiero identificar rápidamente quién ya subió y quién no, para tomar decisiones rápidas.
    </td>
    <td style="text-align: center;">
    Criterios de aceptación: 
    <br>Código de colores 
    <br>Vista clara y legible en movimiento. 
    <br>Interfaz optimizada para uso rápido
    </td>
    <td style="text-align: center;">
    EP06
    </td>
  </tr>

  <!-- US 45 -->
|US45|Actualización automática del monitoreo|Como institución educativa, quiero que la información se actualice automáticamente, para no recargar manualmente.|Criterios de aceptación: <br>Actualización en tiempo real. <br>No requiere interacción del usuario. <br>No interrumpe la visualización.|EP06|
  <tr>
    <td style="text-align: center;">
    US45
    </td>
    <td style="text-align: center;">
    Confirmación visual rápida
    </td>
    <td style="text-align: center;">
    Como conductor, quiero identificar rápidamente quién ya subió y quién no, para tomar decisiones rápidas.
    </td>
    <td style="text-align: center;">
    Criterios de aceptación: 
    <br>Código de colores 
    <br>Vista clara y legible en movimiento. 
    <br>Interfaz optimizada para uso rápido
    </td>
    <td style="text-align: center;">
    EP06
    </td>
  </tr>

  <!-- US 46 -->
|US46|||Criterios de aceptación: <br>Se muestra lista de recorridos pasados. <br>Ordenados por fecha. <br>Incluye información básica (ruta, unidad, conductor).|EP07|
  <tr>
    <td style="text-align: center;">
    US046
    </td>
    <td style="text-align: center;">
    Confirmación visual rápida
    </td>
    <td style="text-align: center;">
    Como conductor, quiero identificar rápidamente quién ya subió y quién no, para tomar decisiones rápidas.
    </td>
    <td style="text-align: center;">
    Criterios de aceptación: 
    <br>Código de colores 
    <br>Vista clara y legible en movimiento. 
    <br>Interfaz optimizada para uso rápido
    </td>
    <td style="text-align: center;">
    EP07
    </td>
  </tr>

  <!-- US 47 -->
  <tr>
    <td style="text-align: center;">
    US47
    </td>
    <td style="text-align: center;">
    Visualizar detalle de recorrido
    </td>
    <td style="text-align: center;">
    Como institución educativa, quiero ver el detalle de un recorrido específico, para analizar lo sucedido.
    </td>
    <td style="text-align: center;">
    Criterios de aceptación: 
    <br>Muestra ruta completa realizada. 
    <br>Incluye paradas y tiempos. 
    <br>Información clara y organizada.
    </td>
    <td style="text-align: center;">
    EP07
    </td>
  </tr>

  <!-- US 48 -->
  <tr>
    <td style="text-align: center;">
    US48
    </td>
    <td style="text-align: center;">
    Visualizar incidencias históricas
    </td>
    <td style="text-align: center;">
    Como institución educativa, quiero consultar incidencias registradas en recorridos pasados, para tener contexto ante problemas.
    </td>
    <td style="text-align: center;">
    Criterios de aceptación: 
    <br>Lista de incidencias por recorrido. 
    <br>Incluye tipo, hora y descripción. 
    <br>Asociadas correctamente a rutas.
    </td>
    <td style="text-align: center;">
    EP07
    </td>
  </tr>

  <!-- US 49 -->
  <tr>
    <td style="text-align: center;">
    US49
    </td>
    <td style="text-align: center;">
    Filtrar historial
    </td>
    <td style="text-align: center;">
    Como institución educativa, quiero filtrar el historial por fechas, rutas o unidades, para encontrar información específica.
    </td>
    <td style="text-align: center;">
    Criterios de aceptación:
    <br>Permite filtrar por fecha.
    <br>Permite filtrar por ruta o unidad.
    <br>Resultados se actualizan dinámicamente.
    </td>
    <td style="text-align: center;">
    EP07
    </td>
  </tr>

  <!-- US 50 -->
  <tr>
    <td style="text-align: center;">
    US50
    </td>
    <td style="text-align: center;">
    Exportar historial
    </td>
    <td style="text-align: center;">
    Como institución educativa, quiero exportar registros históricos, para respaldar información ante incidentes o auditorías.
    </td>
    <td style="text-align: center;">
    Criterios de aceptación: 
    <br>Permite exportar en PDF o Excel. 
    <br>Incluye datos filtrados. 
    <br>Descarga rápida del archivo.
    </td>
    <td style="text-align: center;">
    EP07
    </td>
  </tr>

  <!-- US 51 -->
  <tr>
    <td style="text-align: center;">
    US51
    </td>
    <td style="text-align: center;">
    Registro de evidencia automática
    </td>
    <td style="text-align: center;">
    Como institución educativa, quiero que el sistema registre automáticamente datos de cada recorrido, para no depender de procesos manuales.
    </td>
    <td style="text-align: center;">
    Criterios de aceptación: 
    <br>Se guarda información de rutas automáticamente. 
    <br>Incluye hora, ubicación y eventos. 
    <br>No requiere intervención del usuario.
    </td>
    <td style="text-align: center;">
    EP07
    </td>
  </tr>

  <!-- US 52 -->
  <tr>
    <td style="text-align: center;">
    US52
    </td>
    <td style="text-align: center;">
    Consulta rápida de eventos
    </td>
    <td style="text-align: center;">
    Como institución educativa, quiero acceder rápidamente a eventos relevantes, para responder ante incidentes.
    </td>
    <td style="text-align: center;">
    Criterios de aceptación: 
    <br>Lista de eventos importantes. 
    <br>Acceso rápido desde panel. 
    <br>Información clara y resumida.
    </td>
    <td style="text-align: center;">
    EP07
    </td>
  </tr>
 
</table>

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