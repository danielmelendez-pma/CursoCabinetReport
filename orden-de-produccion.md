---
description: >-
  Guía para preparar, conciliar y comprobar una Orden de Producción con varios RP
  en Excel: identidad, materiales, cantidades, archivo generado y asociaciones.
layout:
  width: wide
---

# Orden de Producción

**CABINET REPORT · ORGANIZACIÓN DOCUMENTAL PARA FABRICACIÓN**

Organiza en una misma orden los **reportes RP en Excel previamente revisados**. Esta lección muestra cómo preparar, generar y comprobar la OP, sin confundir el documento resultante con el seguimiento físico de fabricación. La disponibilidad de opciones debe comprobarse en la versión instalada.

<figure><img src=".gitbook/assets/image (1) (1).png" alt="Ventana inicial de la herramienta Orden de Producción"><figcaption><p>La OP agrupa reportes RP para organizar la fabricación; no acredita su ejecución.</p></figcaption></figure>

{% hint style="info" %}
**Alcance de la lección:** las capturas conservan un recorrido histórico. La documentación oficial describe la agrupación de **RP en Excel** bajo una Orden de Producción (OP), su salida Excel y el registro de asociaciones cuando procede. La disponibilidad de cada acción depende de la versión, los permisos y los archivos seleccionados. No es un seguimiento automático de la fabricación física.
{% endhint %}

La Orden de Producción reúne información para el control de procesos de fabricación y trabajo en campo.

## 1. Antes de preparar la orden

Parte de los [archivos RP revisados](reporte-de-produccion/archivos-de-reportes-generados.md). Si aún necesitas preparar la relación de materiales para abastecimiento, utiliza [Reporte de Compras](reporte-de-compras.md): **un Excel de Compras no sustituye al RP requerido para la OP**. Si necesitas encontrar una producción anterior, consulta [Explorador de Proyectos](explorador-de-proyectos.md) y recupera los archivos compatibles antes de continuar.

### RP, RC y OP: documentos diferentes

| Documento | Qué toma como referencia | Para qué se utiliza | Qué no acredita |
| --- | --- | --- | --- |
| **Reporte de Producción (RP)** | Piezas, módulos, cantidades y especificaciones del trabajo | Preparar y revisar la información de fabricación; generar el Excel RP que se incorpora a la OP | Que todas las piezas hayan sido fabricadas |
| **Reporte de Compras (RC)** | Fuentes y relaciones de materiales de uno o varios ambientes | Preparar necesidades de abastecimiento en Excel | Que se haya comprado, recibido o descontado material del almacén |
| **Orden de Producción (OP)** | Uno o varios **Excel RP** compatibles y su identificación | Agrupar trabajos bajo una orden, generar el Excel OP y comprobar sus asociaciones, cuando corresponda | Que la OP esté registrada por el solo hecho de generar Excel, ni que el taller haya ejecutado los trabajos |

Comprueba que cada **RP - *.xlsx** provenga del proyecto correcto, que se haya revisado su contenido y que conozcas su cliente, ambiente y **número RP real**. Confronta esos datos con la carpeta y la versión del Excel; si conservas varias copias de un mismo RP, identifica cuál es la autorizada. Verifica también si alguno **ya está asociado a otra OP**: no debes duplicar esa asociación sin resolverla.

## 2. Preparar la orden

Selecciona **Agregar Reporte de Producción** en la herramienta de OP:

<figure><img src=".gitbook/assets/image (2).png" alt="Opción Agregar Reporte de Producción en la OP"><figcaption><p>Incorpora un RP en Excel y verifica su procedencia antes de agruparlo.</p></figcaption></figure>

Localiza el **Excel RP** correspondiente y selecciona **Abrir**:

<figure><img src=".gitbook/assets/image (3).png" alt="Selección de archivo Excel del Reporte de Producción"><figcaption><p>Elige el Excel RP correcto, no un TXT de piezas ni un Excel de Compras.</p></figcaption></figure>

Si el archivo es admitido, el recorrido muestra un mensaje de éxito. Ese aviso de carga no sustituye la verificación del contenido del RP.

También puedes agregar otros RP del mismo cliente si corresponde prepararlos bajo una misma orden. Comprueba **ambientes, números RP y compatibilidad de materiales** antes de agruparlos. No confundas **el número de cada RP** con **el número de control de la OP**: una orden puede reunir varios RP, pero cada origen debe conservar su identidad para la conciliación.

<figure><img src=".gitbook/assets/image (4).png" alt="Vista del proceso al incorporar otros reportes RP a la orden"><figcaption><p>Antes de agregar otro RP, comprueba cliente, ambiente y asociación previa.</p></figcaption></figure>

La pantalla ilustrada presenta el resumen de **materiales y RP seleccionados** para la orden. Comprueba que pertenezcan al mismo trabajo autorizado:

<figure><img src=".gitbook/assets/image (5).png" alt="Resumen de materiales y reportes seleccionados para la orden"><figcaption><p>Concilia cada material y RP con los archivos originales.</p></figcaption></figure>

Antes de generar, revisa los datos que muestran las capturas siguientes:

<figure><img src=".gitbook/assets/image (6).png" alt="Área informativa del número de control y resumen de la OP"><figcaption><p>Registra el número de control OP y verifica las unidades efectivas.</p></figcaption></figure>

El **número de control de OP** y las **cantidades de piezas** aportadas por los RP. Concilia esas cantidades con los Excel de origen:

<figure><img src=".gitbook/assets/image (7).png" alt="Detalle de la cantidad de piezas de los RP agrupados"><figcaption><p>El total debe conciliarse con las cantidades de piezas de origen.</p></figcaption></figure>

La lista de **aglomerados y cantos**, que debes contrastar con las fuentes:

<figure><img src=".gitbook/assets/image (8).png" alt="Listado de aglomerados y cantos en Orden de Producción"><figcaption><p>Comprueba referencias de materiales, espesores y cantos.</p></figcaption></figure>

La lista de **RP seleccionados**, sin duplicaciones o archivos de otro cliente:

<figure><img src=".gitbook/assets/image (9).png" alt="Listado de reportes de producción asociados a la OP"><figcaption><p>Verifica los RP incluidos y descarta incorporaciones duplicadas.</p></figcaption></figure>

Después de conciliar los RP, utiliza la acción **Generar Reporte de Producción** indicada en la captura histórica de esta herramienta. Verifica que la salida corresponda a la **Orden de Producción**, no a un nuevo RP:

<figure><img src=".gitbook/assets/image (11).png" alt="Acción Generar Reporte de Producción dentro de la herramienta OP"><figcaption><p>En este recorrido histórico, la acción prepara la salida de la orden.</p></figcaption></figure>

Selecciona una carpeta de destino donde puedas identificar la OP y relacionarla con sus archivos RP originales:

<figure><img src=".gitbook/assets/image (12).png" alt="Selección de carpeta para guardar el archivo de Orden de Producción"><figcaption><p>Utiliza una ubicación que permita relacionar la OP con sus RP de origen.</p></figcaption></figure>

La [documentación oficial](https://cabinet-report.gitbook.io/cabinet-report-docs/funcionalidades-de-cabinet-report/orden-de-produccion) describe como referencia el nombre de salida `OP-[número] - [cliente].xlsx` y una plantilla ubicada en `Plantillas`. **Confirma el nombre real, la disponibilidad de la plantilla y los permisos de lectura/escritura en tu instalación**; no cambies manualmente el identificador para ocultar un conflicto. Si el selector no admite una ruta de red, utiliza una **copia local autorizada** del RP y verifica que coincida con el original antes de continuar.

El recorrido muestra un mensaje de éxito. **Abre y comprueba el Excel** antes de distribuirlo:

<figure><img src=".gitbook/assets/image (13).png" alt="Mensaje de éxito al generar el archivo de Orden de Producción"><figcaption><p>Abre el Excel generado y comprueba por separado el registro de asociaciones.</p></figcaption></figure>

## 3. Verificar el archivo y el registro de la OP

{% hint style="warning" %}
**Un archivo Excel no equivale por sí solo a una orden registrada.** La creación del documento puede depender de la plantilla local y del guardado de las asociaciones entre RP y OP. Si falla la plantilla, el archivo está bloqueado o la aplicación informa un error de registro, no distribuyas la orden como definitiva.
{% endhint %}

Después de generar, verifica el **número de control OP**, el cliente, los RP incluidos, los totales de piezas y el destino del Excel. Las comprobaciones de archivo y registro se realizan **por separado**:

| Comprobación | Evidencia que debes obtener | Si no concuerda |
| --- | --- | --- |
| **Excel OP generado** | Existe en la carpeta elegida, abre correctamente, identifica la orden y contiene el resumen esperado | Revisa plantilla local, ruta, permisos y posibles bloqueos del archivo; no lo distribuyas |
| **Identidad de la OP** | Número OP identificado y no reutilizado indebidamente, cliente correcto, relación verificable con los números RP | Detén el proceso y comprueba si existe otra orden o una versión previa |
| **Asociación RP ↔ OP** | Los RP seleccionados figuran vinculados a la OP en el registro o consulta disponible, cuando la función lo permite | No presentes el Excel como prueba de registro; investiga el error antes de repetir la operación |
| **Integridad de materiales** | Cantidades efectivas, materiales, espesores y cantos conciliados con cada Excel RP | Localiza la fila o partida de origen, corrige la fuente autorizada y vuelve a verificar |

La documentación oficial contempla registro de vínculos y consulta de órdenes según el contexto, pero **no garantiza que la creación del Excel, la persistencia y la recuperación funcionen como una sola operación**. Si trabajaste sin conexión, vuelve a comprobar los vínculos y el estado del registro cuando recuperes la conectividad; **no des por hecha una sincronización automática**.

Ante un error, conserva los **Excel RP originales**, el nombre y ubicación del Excel OP, el identificador de orden, el mensaje mostrado y, cuando sea posible, una captura sin datos sensibles. No crees una segunda OP ni cambies su número solo para eludir un fallo de guardado: primero comprueba si la anterior llegó a registrarse.

## 4. Herramientas relacionadas

Las capturas históricas incluyen una opción de **conversión entre optimizadores**. Comprueba qué formatos están disponibles en tu instalación:

<figure><img src=".gitbook/assets/image (14).png" alt="Herramienta histórica de conversión entre formatos de optimizadores"><figcaption><p>Comprueba los formatos disponibles y verifica la salida antes de mecanizar.</p></figcaption></figure>

También se ilustran opciones para **fusionar o separar optimizaciones**:

<figure><img src=".gitbook/assets/image (15).png" alt="Opciones históricas para fusionar o separar optimizaciones"><figcaption><p>Después de combinar o separar, revisa material y cantidades por RP de origen.</p></figcaption></figure>

Estas operaciones requieren volver a comprobar las piezas y materiales del resultado contra cada RP de origen. No presupongas que la combinación conserva todas las condiciones del corte; consulta [Optimizadores](optimizadores.md).

## 5. Comprobación antes de entregar a fabricación

1. Confirma que **cliente, ambientes, RP y número OP** sean correctos y estén asociados de forma coherente.
2. Contrasta piezas, cantidades y tableros/cantos con los reportes originales.
3. Revisa la existencia y apertura del Excel generado y, **por separado**, el estado del registro y las asociaciones de la OP.
4. Comprueba que no falte ningún RP previsto, que un mismo origen no se haya incluido dos veces y que el número OP no corresponda a otra orden.
5. Si utilizas las herramientas de conversión o fusión de optimizaciones, verifica por separado la compatibilidad del formato y el listado de piezas resultante, incluidas las **piezas no colocadas**.
6. Obtén la autorización correspondiente antes de entregar documentos a corte, montaje o instalación: la OP no acredita la ejecución física.

## 6. Ejercicio verificable: conciliar dos RP en una OP

Este ejercicio complementa las capturas anteriores con un **control manual de trazabilidad**. Se parte de dos Excel RP revisados del **mismo cliente**, pertenecientes a ambientes distintos. Las referencias «RP-A» y «RP-B» son etiquetas didácticas: **no son números reales, formatos de archivo ni datos que debas escribir en Cabinet Report**.

### Hoja de control antes de agrupar

Supón que el RP-A (Cocina) contiene dos módulos iguales con **dos costados, una base y una tapa por módulo**, y que el RP-B (Clóset) contiene un módulo con esa misma composición. Los números son un ejemplo de conteo, **no reglas de despiece ni dimensiones de fabricación**.

| Origen | Ambiente | Módulos del ejemplo | Costados | Bases | Tapas | Piezas efectivas |
| --- | --- | ---: | ---: | ---: | ---: | ---: |
| RP-A | Cocina | 2 | 4 | 2 | 2 | **8** |
| RP-B | Clóset | 1 | 2 | 1 | 1 | **4** |
| **Total esperado** | **2 ambientes** | **3** | **6** | **3** | **3** | **12** |

**Control de unidades:** el total esperado es **12 unidades de piezas**, no 12 filas ni 12 módulos. Un RP puede agrupar varias unidades en una sola fila; comprueba las cantidades efectivas de cada tipo y su pertenencia al RP. El ejercicio no presupone que la OP muestre las mismas columnas ni que la aplicación calcule automáticamente esta tabla.

### Ejecución y comparación paso a paso

1. **Identifica la fuente autorizada.** Anota para cada Excel RP el cliente, ambiente, **número RP real**, fecha o versión del archivo y ubicación. Conserva una copia del original; no trabajes con dos copias que parezcan ser la versión definitiva.
2. **Valida cada RP por separado.** En los Excel de origen, confirma las unidades de costados, bases y tapas del ejemplo; en una producción real revisa también **pieza, módulo, medidas, espesor, material, veta y canto por lado**. Si hay piezas sueltas, añádelas a la conciliación sin atribuirlas a un módulo inexistente.
3. **Comprueba la elegibilidad.** Confirma que ambos RP pertenecen al mismo cliente, que deben integrarse en una misma OP y que **no están asignados a otra orden**. No continúes si hay un vínculo anterior sin resolver o materiales incompatibles para la operación prevista.
4. **Agrega los archivos individualmente.** Selecciona primero el Excel del RP-A y después el RP-B mediante el recorrido ilustrado. Contrasta la lista de RP cargados con tu hoja de control: deben aparecer **los dos orígenes correctos, sin duplicación**.
5. **Concilia antes de generar.** Para este caso, comprueba que la información de la orden represente **8 + 4 = 12 piezas efectivas**. Si la pantalla agrupa filas o materiales de otra manera, compara el detalle con los dos Excel: no deduzcas equivalencia solo de un total general.
6. **Genera y vuelve a abrir el Excel OP.** Confirma número de control OP, cliente, RP incluidos, contenido y carpeta de destino. Comprueba por separado, cuando corresponda, que **la asociación RP ↔ OP esté registrada**; el archivo creado y la persistencia de la orden son dos verificaciones distintas.
7. **Prepara la salida por área.** Entrega a corte únicamente las listas y optimizaciones verificadas; remite a montaje los RP y complementarios pertinentes, y a instalación la información autorizada. Registra manualmente qué versión recibió cada responsable.

### Prueba de discrepancia: detecta una duplicación

Si en tu **hoja de conciliación** cuentas por equivocación el RP-A dos veces, obtendrías **8 + 8 + 4 = 20** piezas, frente a las **12** aprobadas. La diferencia de **8** indica que debes revisar el origen de cada partida, no aceptar una suma mayor por parecer más completa. **Este ejemplo no afirma que Cabinet Report permita ni detecte automáticamente archivos repetidos.**

Si, por el contrario, omites RP-B, el total quedaría en **8** piezas: faltarían **4**. En ambos casos compara **la lista de números RP y sus cantidades de origen**, no solo el total, porque dos errores opuestos podrían compensarse. Una coincidencia numérica tampoco valida que materiales, espesores, vetas o cantos sean compatibles.

Si las cantidades no coinciden, detén la entrega, identifica cuál RP, fila o pieza produce la diferencia, corrige la fuente autorizada y repite la conciliación. No «arregles» la OP editando totales sin rastrear su procedencia.

### Matriz manual de entrega: de la orden al taller

| Documento o etapa | Comprobación de procedencia y contenido | Criterio para avanzar |
| --- | --- | --- |
| **Excel RP-A y RP-B** | Cliente, ambiente, número RP, versión, unidades de piezas, materiales y cantos | Ambos orígenes revisados y sin duplicados |
| **Excel OP** | Número OP, lista de los dos RP, resumen contrastado y archivo que abre correctamente | **12 piezas en el ejemplo**, o diferencia justificada y corregida antes de autorizar |
| **Asociación de la orden** | Registro y recuperación de los vínculos RP ↔ OP, cuando la función los gestione | No dar por registrada la OP solo por tener el Excel |
| **Corte / optimización** | Identificación de cada material, piezas colocadas y pendientes, restricciones y formatos de máquina | Conservar correspondencia con los RP; no omitir pendientes |
| **Compras / almacén** | [Reporte de Compras](reporte-de-compras.md), existencias, descripciones, cantidades y **unidades** de tableros, perfilería y herrajes | No confundir unidades, tramos o longitudes ni el reporte con una compra |
| **Montaje e instalación** | RP aprobado, identificación del ambiente, complementarios e instrucciones del proyecto | Entrega registrada por el equipo; la OP no certifica ejecución física |

{% hint style="warning" %}
**Criterio de aceptación del ejercicio:** no entregues la OP si falta un RP esperado, aparece un RP duplicado, no se justifican las unidades efectivas, difieren los materiales o el Excel y la asociación no se pueden comprobar según corresponda. Una optimización fusionada **tampoco sustituye** la conciliación por RP de origen. El estado «aprobado» es una **decisión documentada por el responsable**, no una nueva función o etiqueta del programa.
{% endhint %}

Para continuar, consulta [Archivos de Reportes Generados](reporte-de-produccion/archivos-de-reportes-generados.md), [Optimizadores](optimizadores.md) y [Reporte de Compras](reporte-de-compras.md). Estas herramientas producen entregables diferentes: **RP, OP, optimización y compras no son documentos intercambiables**.

Consulta los detalles del alcance, registro y continuidad en la [Documentación oficial — Orden de Producción](https://cabinet-report.gitbook.io/cabinet-report-docs/funcionalidades-de-cabinet-report/orden-de-produccion).

---

[← Reporte de Compras](reporte-de-compras.md) · [Optimizadores →](optimizadores.md) · [🏠 Portal principal](https://danielmelendez-pma.github.io/cabinet-report-partners/)
