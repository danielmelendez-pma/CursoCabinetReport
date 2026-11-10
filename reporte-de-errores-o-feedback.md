---
description: >-
  Cómo comunicar correcciones y sugerencias desde Cabinet Report, documentar
  incidencias reproducibles y preparar evidencias seguras sin confundir el envío
  de un reporte con su recepción o resolución.
---

# Reporte de Errores o Feedback

Desde Cabinet Report puedes comunicar **errores de funcionamiento** y **sugerencias de mejora** mediante el formulario incluido en la aplicación. Esta lección explica cómo preparar un reporte que permita identificar qué ocurrió y reproducir el problema, cuando sea posible.

**Alcance de esta guía:** es un procedimiento para reunir información y comunicar una incidencia, no un diagnóstico técnico certificado ni una garantía de que se haya identificado un defecto. La corrección del software, si procede, exige una evaluación posterior y pruebas de la solución.

{% hint style="info" %}
**Reporte desde la aplicación y soporte técnico no son lo mismo.** Enviar una incidencia no garantiza una corrección inmediata ni un plazo de respuesta. Consulta el alcance y los canales disponibles en las [Políticas de Soporte](https://cabinet-report.gitbook.io/cabinet-report-docs/politicas-de-soporte).
{% endhint %}

Las políticas oficiales contemplan **canales digitales habilitados, documentación y sesiones remotas previamente coordinadas**. El canal disponible, la prioridad y el tiempo de respuesta dependen del plan contratado; el horario general es el laboral de Panamá, salvo acuerdo previo y con exclusión de feriados nacionales. No equivale a soporte incluido la capacitación integral en fabricación, el diseño personalizado ni la corrección de errores humanos externos al programa.

{% hint style="info" %}
**Una incidencia por reporte.** Antes de notificar un fallo, revisa la lección del proceso afectado y distingue un resultado pendiente de comprobar de un comportamiento realmente inesperado. La información de esta página te ayuda a describir el caso; no confirma que exista un defecto en una versión concreta.
{% endhint %}

## 1. Abrir el formulario

1. En la parte superior derecha de Cabinet Report, localiza el acceso de ayuda mostrado en la captura.
2. Selecciona el ícono correspondiente.
3. En la ventana que se abre, elige la opción ilustrada para acceder al formulario de reportes.

<figure><img src=".gitbook/assets/image (116).png" alt="Ubicación del acceso de ayuda en la parte superior de Cabinet Report"><figcaption><p>Localiza primero el acceso de ayuda en la parte superior de la ventana.</p></figcaption></figure>

<figure><img src=".gitbook/assets/IcoAyuda2.png" alt="Ícono de ayuda utilizado para acceder a las opciones de asistencia" width="128"><figcaption><p>Identifica el ícono de ayuda antes de desplegar las opciones disponibles.</p></figcaption></figure>

<figure><img src=".gitbook/assets/image (118).png" alt="Ventana de opciones disponible desde el acceso de ayuda"><figcaption><p>Desde el acceso de ayuda, revisa las opciones de asistencia de tu versión.</p></figcaption></figure>

<figure><img src=".gitbook/assets/image (119).png" alt="Opción para abrir el formulario de errores y sugerencias"><figcaption><p>Selecciona la opción de errores o sugerencias para abrir el formulario.</p></figcaption></figure>

**Secuencia de las capturas:** acceso superior (imagen 116), ícono de ayuda (IcoAyuda2), opciones de asistencia (imagen 118), entrada al formulario (imagen 119) y formulario de captura (imagen 120). Las imágenes son referencias históricas, no prueba de que todos los rótulos y posiciones sean idénticos en tu instalación.

La ubicación y la apariencia de las opciones pueden variar según la versión instalada. Si no aparece el acceso, **no improvises cambios de configuración**: registra la versión que ves, conserva la captura disponible y consulta el canal oficial de soporte habilitado para tu plan. Si la aplicación no permite iniciar sesión, utiliza el canal externo habilitado; no presupongas que el formulario sea accesible sin ingresar.

## 2. Elegir el tipo y describir lo sucedido

El formulario dispone de dos tipos de reporte:

- **CORRECCIÓN:** para informar un posible defecto, comportamiento inesperado o función que no produce el resultado previsto. El tipo de reporte **no confirma** por sí mismo que la causa sea un error del software.
- **SUGERENCIA:** para proponer una mejora o una nueva posibilidad de uso. Describe la necesidad y el beneficio esperado, sin presentarla como un fallo existente. La propuesta puede evaluarse sin obligación de implementarse inmediatamente, según las Políticas de Soporte.

<figure><img src=".gitbook/assets/image (120).png" alt="Formulario de reporte de errores y sugerencias en Cabinet Report"><figcaption><p>Elige el tipo de reporte y redacta un asunto que identifique la incidencia.</p></figcaption></figure>

Escribe un **asunto específico** que identifique el módulo y el síntoma; por ejemplo: `OPTIMIZADOR DE TABLEROS — DIFERENCIA AL EXPORTAR`, en lugar de `NO FUNCIONA`. Evita incluir el nombre completo del cliente, identificadores de licencia o información confidencial en el asunto.

Para una **CORRECCIÓN**, incorpora en la descripción los datos disponibles:

1. **Versión realmente instalada** de Cabinet Report, copiada tal como se muestra en la aplicación (por ejemplo, en la pantalla o en su indicador de versión, si está visible). No confundas la versión publicada para descargar con la que ejecutaste al ocurrir el problema.
2. **Área y operación:** ventana, módulo, comando y momento aproximado (fecha, hora y zona horaria); sistema Windows, modalidad o conectividad **solo si influyen**. No adjuntes información identificativa del equipo que no sea necesaria.
3. **Entrada y condiciones previas:** archivo o copia de prueba utilizada, cliente/ambiente **ficticios o anonimizados**, configuración, parámetros, unidades y cantidades relevantes. Señala lo que no conoces en vez de adivinarlo.
4. **Pasos para reproducirlo:** acciones numeradas desde un estado inicial definido, con la decisión o comando que desencadena el resultado; indica si otra persona puede repetirlos con la misma entrada.
5. **Resultado esperado frente al observado:** describe qué resultado correspondía según los datos y qué apareció realmente. Copia el mensaje exacto **sin secretos**, o indica si no hubo aviso. Distingue pantalla, archivo guardado y exportación.
6. **Frecuencia, alcance e impacto:** siempre / intermitente / una vez; número aproximado de intentos, si ocurre con un caso o varios, y si bloquea, retrasa o permite continuar con comprobación manual.
7. **Evidencia conservada:** capturas y comparaciones anonimizadas de entrada/salida; registra si hiciste una prueba aislada y qué cambió entre intentos.

Si el origen puede ser una **entrada incorrecta**, un cálculo todavía pendiente o una restricción del optimizador, expón esa hipótesis como **pendiente de verificar**, no como defecto probado.

### Ejemplo de mensaje de corrección

El siguiente texto es **solo un ejemplo de redacción**, no la descripción de un error confirmado del programa:

```text
Versión instalada: [copiar el número visible en la aplicación]
Fecha/hora: [aproximada; indicar zona horaria]
Área / operación: Reporte de Producción / Optimizar
Entrada: [RP de prueba anonimizado; versión y unidades]
Condiciones: [modalidad, material, parámetros y cantidades]
Pasos:
1. Abrir la copia de prueba identificada.
2. Verificar las cantidades y ejecutar la opción indicada.
3. Registrar la salida en pantalla y el archivo exportado, si existe.
Esperado: [resultado concreto y comprobable con esa entrada].
Observado: [resultado real, aviso literal o ausencia de aviso].
Frecuencia: [número de intentos; siempre / a veces / una vez].
Impacto: [bloquea / retrasa / permite continuar tras verificar].
Evidencia: [captura anonimizada y comparación de entrada/salida].
```

Para una **SUGERENCIA**, sustituye los pasos del error por la **tarea actual**, la **limitación o necesidad**, el **cambio propuesto**, su **beneficio esperado** y un **ejemplo de uso**. Identifica si se trata de una mejora opcional y no afirmes que una función inexistente debería estar disponible en tu plan. Si detectas dos problemas independientes, descríbelos en reportes separados para que sus evidencias no se mezclen.

## 3. Adjuntar evidencias útiles

Si el problema es visible, haz una captura de pantalla y, como muestra la guía original, **pégala con Ctrl + V** en el área de imagen del formulario. Puedes preparar la captura con una herramienta de Windows disponible en tu equipo; antes de copiarla, **recorta u oculta** datos sensibles fuera de la aplicación. Comprueba visualmente que la captura correcta aparece en el área prevista: copiarla al portapapeles o pulsar Ctrl + V no demuestra por sí solo que haya quedado incluida en el reporte.

<figure><img src=".gitbook/assets/image (121).png" alt="Área del formulario destinada a pegar una captura de pantalla"><figcaption><p>Pega únicamente una captura pertinente y revisa que no muestre datos sensibles.</p></figcaption></figure>

También puedes utilizar la opción para **adjuntar archivos**, cuando el formulario y tu versión lo permitan. Adjunta solo los que sean necesarios para explicar el problema; si procede, utiliza una copia de prueba y conserva el original. **No se acreditan aquí extensiones admitidas, cantidad máxima, límites de tamaño, transferencia efectiva ni retención de adjuntos:** comprueba lo que muestra tu versión y, si el archivo no es aceptado, registra el mensaje sin cambiar extensiones artificialmente. No envíes archivos completos de clientes o producciones cuando baste una muestra autorizada.

<figure><img src=".gitbook/assets/image (122).png" alt="Opción del formulario para adjuntar archivos de apoyo"><figcaption><p>Utiliza el control de adjuntos disponible en tu versión solo para evidencias necesarias.</p></figcaption></figure>

{% hint style="warning" %}
**Protege los datos antes de enviar.** Revisa asunto, texto, capturas, rutas de archivo, propiedades de documentos y adjuntos para excluir **contraseñas, códigos completos de licencia, tokens, claves API, cadenas de conexión, datos de usuarios o clientes y valores comerciales privados** ajenos al caso. Usa alias como «Cliente de prueba / Ambiente A», recorta imágenes y, si es necesario, prepara un extracto anonimizado. No publiques evidencias en canales abiertos ni consideres suficiente ocultar únicamente una parte visible si el documento conserva otros datos.
{% endhint %}

## 4. Revisar y enviar

Antes de utilizar la opción de envío disponible en el formulario:

1. Confirma que elegiste **CORRECCIÓN** o **SUGERENCIA** según corresponda.
2. Comprueba que el asunto, los pasos y los resultados permiten entender la solicitud.
3. Verifica que la captura se haya pegado y que los adjuntos necesarios estén seleccionados **si la versión lo permite**.
4. Revisa por última vez los datos sensibles que puedan aparecer en el mensaje o las evidencias.
5. Conserva por separado el asunto, la descripción y la prueba anonimizada **antes** de pulsar Enviar, para no perder la información si falla la ventana.

Usa el control de envío que muestre tu versión y **observa el mensaje o estado concreto**. Distingue tres situaciones que no son equivalentes:

- **Intento de envío:** pulsaste el control, pero todavía no existe evidencia de que se completara la operación.
- **Confirmación visible en la aplicación:** guarda fecha, hora y texto o captura del aviso, si aparece. Confirma **lo que informa la interfaz**, no por sí solo la recepción efectiva por una persona ni la creación de un ticket.
- **Recepción, diagnóstico y atención:** solo se acreditan cuando existe comunicación o evidencia específica del soporte. Un reporte enviado no significa causa identificada, corrección implementada, disponibilidad de actualización ni plazo comprometido.

Si el envío muestra un error, queda pendiente o se cierra sin confirmación, **no asumas recepción**. Guarda el texto y las evidencias anonimizadas, apunta el momento, evita insistir indefinidamente sobre la misma operación y consulta los **canales oficiales habilitados** para tu plan. No se documenta un número de ticket, acuse automático ni reintento automático garantizado. Las [Políticas de Soporte](https://cabinet-report.gitbook.io/cabinet-report-docs/politicas-de-soporte) fijan el marco general de atención, sin prometer respuesta inmediata.

## 5. Localizar el origen del problema según la tarea

Antes de redactar una **CORRECCIÓN**, consulta el recorrido correspondiente. Esta comprobación evita confundir un dato de entrada incorrecto, una salida pendiente o una diferencia de unidades con un defecto del programa.

**Clasificación previa recomendada (manual, no automática):** «ENTRADA POR CORREGIR» cuando falta o se introduce un valor incompatible; «RESULTADO PENDIENTE» cuando la salida aún no se ha conciliado, contiene piezas sin colocar o no tiene precio validado; «POSIBLE DEFECTO REPRODUCIBLE» cuando el comportamiento inesperado persiste con una entrada conocida, pasos repetibles y evidencia comparable. Esta clasificación orienta el reporte y **no sustituye el diagnóstico del soporte**.

| Si ocurre en… | Comprueba primero | Evidencia útil para el reporte |
| --- | --- | --- |
| [Reporte de Producción](reporte-de-produccion/README.md) | Cliente, ambiente, referencia, versión del RP, piezas, cantidades, medidas, materiales, veta y cantos. Consulta también [Archivos de Reportes Generados](reporte-de-produccion/archivos-de-reportes-generados.md). | Pasos ejecutados, aviso exacto y comparación entre las filas relevantes del RP y el archivo resultante, si existe. |
| [Optimizadores](optimizadores.md) | Modalidad de corte, origen del listado, formatos de tablero o longitud de perfil, cantidad total de piezas, giro, resane y piezas sin colocar. | Parámetros utilizados, total de piezas de entrada, piezas colocadas, pendientes y resultado exportado, sin compartir más datos de los necesarios. |
| [Reporte de Compras](reporte-de-compras.md) | Origen de materiales, ambientes incluidos, unidad de cada partida, consolidación y exclusiones. | Archivo de prueba o extracto de la partida, unidad esperada, unidad observada y trazabilidad aplicable. |
| [Costos](costos.md) | Ambiente seleccionado, origen de cantidades, unidades, precio unitario realmente cargado, partidas repetidas y ajustes de cotización. | Partida concreta, cálculo manual comparable, importe mostrado y punto del recorrido en que aparece la diferencia; oculta precios confidenciales si no son imprescindibles. |

{% hint style="warning" %}
**No mezcles un fallo con una revisión técnica pendiente.** Si las piezas no caben en las planchas, si un material no se ha comprado o si un precio está ausente, primero determina si se trata de una entrada, restricción o decisión pendiente. Solo reporta un defecto cuando puedas describir el comportamiento inesperado y su evidencia.
{% endhint %}

## 6. Ejercicio práctico: investigar una diferencia en la optimización

Este caso es **didáctico y ficticio**; no describe un error confirmado de Cabinet Report.

1. Prepara **fuera de una producción en curso** una copia autorizada de prueba de un RP revisado. Imagina que contiene **8 unidades de piezas** al sumar las cantidades de cada referencia, aunque ocupen menos de ocho filas. Anota una identificación ficticia, la versión instalada y una lista de referencias con sus unidades; **no alteres un RP real aprobado ni sobrescribas sus exportaciones**.
2. Abre el [recorrido de Optimizadores](optimizadores.md), utiliza las opciones disponibles en tu versión y registra el método y las condiciones que afectan a la colocación: formatos y material, espesor, veta/giro, restricciones y resane **cuando correspondan**. Identifica el archivo fuente y sus unidades; no presupongas que todas las modalidades tienen los mismos parámetros.
3. Supón que la pantalla presenta **7 unidades colocadas y 1 pendiente**. En ese caso **no concluyas automáticamente que hay un error**: 7 + 1 = 8 unidades contabilizadas. Comprueba que el desglose **por referencia**, las unidades y las restricciones son comparables, y revisa primero los parámetros y la disponibilidad del material; «pendiente» no significa «perdida» ni «exportada».
4. Si, en otra prueba controlada, la pantalla **indica 8 unidades colocadas y 0 pendientes**, pero el archivo exportado contiene **solo 7 unidades**, comprueba primero que abriste la **exportación de esa misma ejecución**, que no se ha aplicado un filtro, que las referencias no se agruparon en filas de cantidad mayor y que la unidad de conteo es equivalente. Compara **requeridas = colocadas + pendientes**, referencia por referencia, con el total efectivamente exportado. Conserva la entrada, parámetros, pantalla y salida de prueba sin sobrescribir archivos aprobados.
5. Si la diferencia persiste tras repetir **sin modificar la entrada ni la configuración**, redacta una **CORRECCIÓN** con versión, fecha, pasos exactos, parámetros, conteos por referencia, resultado esperado y observado, frecuencia e impacto. Adjunta solo una captura o extracto anonimizado. Si **no puedes reproducirla**, indícalo expresamente y conserva la evidencia del evento único en vez de presentar un defecto confirmado.

**Ejemplo de asunto:** `DIFERENCIA ENTRE PIEZAS COLOCADAS Y ARCHIVO EXPORTADO`.

**Resultado del ejercicio:** distinguir **una unidad pendiente de colocar** de **una posible inconsistencia entre lo mostrado y lo exportado**. Registra externamente el resultado como «CONFORME», «DIFERENCIA OBSERVADA» o «NO VERIFICADO»; son categorías para el ejercicio, **no estados del programa**. Hasta confirmar el resultado y la revisión técnica, no entregues ese plan de corte para fabricación.

## 7. Precauciones cuando el error afecta a producción

Si el problema aparece durante la preparación de piezas, optimización o generación de archivos, **no des por validada la salida únicamente porque el programa la haya generado**. Comprueba medidas, materiales, cantidades, cantos y los documentos destinados a fabricación antes de autorizarlos.

**Recuperación y trazabilidad manual:** conserva copias identificadas de la **última entrada válida**, la **salida observada**, la **versión**, los **parámetros**, el **aviso** y la **fecha del intento**. Marca el archivo problemático como **pendiente de revisión** y, si una versión ya fue distribuida al taller, coordina expresamente su suspensión o sustitución con los responsables; generar otro archivo no revoca automáticamente el anterior. No reproduzcas incidencias peligrosas o destructivas sobre trabajos activos.

Mantén un registro privado por caso con **asunto, fecha, canal utilizado, estado de confirmación, evidencia enviada y comunicaciones posteriores**. Distingue **reporte de incidencia** (hechos aportados), **diagnóstico técnico** (causa corroborada) y **corrección implementada y validada** (cambio probado en versión concreta). No atribuyas a la aplicación un seguimiento de tickets o historial automático que no se haya demostrado.

Para revisar el recorrido de actualización, consulta [Instalar Actualizaciones](instalar-actualizaciones.md). Para elegir entre manual, documentación oficial y otros recursos, visita [Ver Documentación](ver-documentacion.md). Si necesitas volver al procedimiento que originó el caso, utiliza los enlaces del apartado 5.

---

[← Costos](costos.md) · [Ver Documentación →](ver-documentacion.md) · [Portada del Curso](README.md) · [🏠 Portal principal](https://danielmelendez-pma.github.io/cabinet-report-partners/)
