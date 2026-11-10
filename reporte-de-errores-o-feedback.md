---
description: >-
  Cómo informar errores o sugerencias desde Cabinet Report, preparar evidencias
  seguras y relacionar incidencias con producción, optimizadores y costos.
---

# Reporte de Errores o Feedback

Desde Cabinet Report puedes comunicar **errores de funcionamiento** y **sugerencias de mejora** mediante el formulario incluido en la aplicación. Esta lección explica cómo preparar un reporte que permita identificar qué ocurrió y reproducir el problema, cuando sea posible.

{% hint style="info" %}
**Reporte desde la aplicación y soporte técnico no son lo mismo.** Enviar una incidencia no garantiza una corrección inmediata ni un plazo de respuesta. Consulta el alcance y los canales disponibles en las [Políticas de Soporte](https://cabinet-report.gitbook.io/cabinet-report-docs/politicas-de-soporte).
{% endhint %}

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

La ubicación y la apariencia de las opciones pueden variar según la versión instalada.

## 2. Elegir el tipo y describir lo sucedido

El formulario dispone de dos tipos de reporte:

- **CORRECCIÓN:** para informar un error, comportamiento inesperado o función que no produce el resultado previsto.
- **SUGERENCIA:** para proponer una mejora o una nueva posibilidad de uso. Describe la necesidad y el beneficio esperado, sin presentarla como un fallo existente.

<figure><img src=".gitbook/assets/image (120).png" alt="Formulario de reporte de errores y sugerencias en Cabinet Report"><figcaption><p>Elige el tipo de reporte y redacta un asunto que identifique la incidencia.</p></figcaption></figure>

Escribe un **asunto específico**. Por ejemplo: `ERROR AL OPTIMIZAR TABLEROS`, en lugar de `NO FUNCIONA`.

Para una corrección, incorpora en el mensaje los datos que tengas disponibles:

1. **Versión de Cabinet Report** y área o ventana donde ocurre.
2. **Operación que intentabas realizar**, incluida la opción o comando seleccionado.
3. **Pasos para reproducirlo**, en orden y sin omitir la acción que desencadena el problema.
4. **Resultado esperado** y **resultado observado**; transcribe el aviso exacto cuando exista.
5. **Frecuencia e impacto**: si ocurre siempre o de forma intermitente y si impide continuar el trabajo.
6. **Contexto técnico mínimo**: tipo de archivo, materiales o datos relevantes para comprender el caso, sin añadir información privada innecesaria.

### Ejemplo de mensaje de corrección

El siguiente texto es **solo un ejemplo de redacción**, no la descripción de un error confirmado del programa:

```text
Versión: [versión instalada]
Área: Reporte de Producción / Optimización
Operación: Optimizar un reporte ya preparado
Pasos:
1. Abrir el reporte de prueba.
2. Ejecutar la opción de optimización.
3. Observar el resultado mostrado.
Esperado: que se genere la salida correspondiente o un aviso explicativo.
Observado: [describir el resultado y copiar el mensaje exacto].
Frecuencia: [siempre / a veces / una sola vez].
Impacto: [indicar si bloquea la preparación del trabajo].
```

Para una **SUGERENCIA**, sustituye los pasos del error por la tarea que deseas simplificar, el comportamiento que propones y un ejemplo de uso. Si detectas dos problemas independientes, descríbelos en reportes separados para que sus evidencias no se mezclen.

## 3. Adjuntar evidencias útiles

Si el problema es visible, haz una captura de pantalla y, como muestra la guía original, **pégala con Ctrl + V** en el área de imagen del formulario.

<figure><img src=".gitbook/assets/image (121).png" alt="Área del formulario destinada a pegar una captura de pantalla"><figcaption><p>Pega únicamente una captura pertinente y revisa que no muestre datos sensibles.</p></figcaption></figure>

También puedes utilizar la opción para **adjuntar archivos**, cuando el formulario y tu versión lo permitan. Adjunta solo los que sean necesarios para explicar el problema; si procede, utiliza una copia de prueba y conserva el original.

<figure><img src=".gitbook/assets/image (122).png" alt="Opción del formulario para adjuntar archivos de apoyo"><figcaption><p>Utiliza el control de adjuntos disponible en tu versión solo para evidencias necesarias.</p></figcaption></figure>

{% hint style="warning" %}
**Protege los datos antes de enviar.** Revisa las capturas y los archivos para no incluir contraseñas, claves de API, licencias completas, datos personales de clientes ni información confidencial ajena a la incidencia. Oculta o sustituye esos datos y evita compartir archivos de producción completos cuando un ejemplo reducido sea suficiente.
{% endhint %}

## 4. Revisar y enviar

Antes de utilizar la opción de envío disponible en el formulario:

1. Confirma que elegiste **CORRECCIÓN** o **SUGERENCIA** según corresponda.
2. Comprueba que el asunto, los pasos y los resultados permiten entender la solicitud.
3. Verifica que la captura se haya pegado y que los adjuntos necesarios estén seleccionados.
4. Revisa por última vez los datos sensibles que puedan aparecer en el mensaje o las evidencias.

Envía el reporte desde la propia ventana y **comprueba la confirmación o el estado que muestre la aplicación**. No interpretes el cierre de una ventana o la ausencia de un aviso como prueba de recepción.

Si no puedes confirmar el envío, conserva el texto y las evidencias, anota el mensaje mostrado e intenta comunicar la incidencia mediante los **canales oficiales de soporte** que correspondan a tu plan. Las [Políticas de Soporte](https://cabinet-report.gitbook.io/cabinet-report-docs/politicas-de-soporte) explican las condiciones generales de atención, sin garantizar una respuesta inmediata.

## 5. Localizar el origen del problema según la tarea

Antes de redactar una **CORRECCIÓN**, consulta el recorrido correspondiente. Esta comprobación evita confundir un dato de entrada incorrecto, una salida pendiente o una diferencia de unidades con un defecto del programa.

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

1. Prepara una copia de prueba de un RP revisado. Imagina que contiene **8 unidades de piezas** al sumar sus cantidades, aunque ocupen menos de ocho filas. Anota el cliente y el ambiente de prueba sin incluir datos reales innecesarios.
2. Abre el [recorrido de Optimizadores](optimizadores.md), utiliza las opciones disponibles en tu versión y registra las condiciones que afectan a la colocación. No presupongas que todas las modalidades tienen los mismos parámetros.
3. Supón que la pantalla presenta **7 piezas colocadas y 1 sin colocar**. En ese caso **no concluyas automáticamente que hay un error**: las 8 unidades están contabilizadas. Revisa primero los parámetros y la disponibilidad del material.
4. Si, en otra prueba controlada, la herramienta **indica 8 colocadas y 0 pendientes**, pero al revisar el archivo exportado encuentras **solo 7 unidades**, compara el mismo alcance y las mismas unidades. Conserva el origen y la exportación de prueba; no sobrescribas un archivo aprobado.
5. Si la diferencia persiste, redacta una **CORRECCIÓN** con versión, pasos exactos, parámetros, conteos comparables, resultado esperado y resultado observado. Adjunta únicamente un extracto o captura anonimizada que permita reproducirla.

**Ejemplo de asunto:** `DIFERENCIA ENTRE PIEZAS COLOCADAS Y ARCHIVO EXPORTADO`.

**Resultado del ejercicio:** aprender a distinguir **una pieza sin colocar** de **una posible inconsistencia entre lo mostrado y lo exportado**. Hasta confirmar el resultado y la revisión técnica, no entregues ese plan de corte para fabricación.

## 7. Precauciones cuando el error afecta a producción

Si el problema aparece durante la preparación de piezas, optimización o generación de archivos, **no des por validada la salida únicamente porque el programa la haya generado**. Comprueba medidas, materiales, cantidades, cantos y los documentos destinados a fabricación antes de autorizarlos.

Para revisar el recorrido de actualización, consulta [Instalar Actualizaciones](instalar-actualizaciones.md). Para elegir entre manual, documentación oficial y otros recursos, visita [Ver Documentación](ver-documentacion.md). Si necesitas volver al procedimiento que originó el caso, utiliza los enlaces del apartado 5.

---

[← Costos](costos.md) · [Ver Documentación →](ver-documentacion.md) · [Portada del Curso](README.md) · [🏠 Portal principal](https://danielmelendez-pma.github.io/cabinet-report-partners/)
