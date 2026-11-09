# Orden de Producción

Esta lección conserva el recorrido documentado para reunir reportes de producción, consultar materiales y generar una orden. La disponibilidad concreta de opciones debe comprobarse en la versión instalada.

<figure><img src=".gitbook/assets/image (1) (1).png" alt=""><figcaption></figcaption></figure>

{% hint style="info" %}
**Alcance de la lección:** las capturas conservan un recorrido histórico. La documentación oficial describe la agrupación de **RP en Excel** bajo una Orden de Producción (OP), su salida Excel y el registro de asociaciones cuando procede. La disponibilidad de cada acción depende de la versión, los permisos y los archivos seleccionados. No es un seguimiento automático de la fabricación física.
{% endhint %}

La Orden de Producción reúne información para el control de procesos de fabricación y trabajo en campo.

## 1. Antes de preparar la orden

Comprueba que cada **RP - *.xlsx** provenga del proyecto correcto, que se haya revisado su contenido y que conozcas su cliente, ambiente y número RP. Verifica también si alguno **ya está asociado a otra OP**: no debes duplicar esa asociación sin resolverla.

## 2. Preparar la orden

Haga clic en 

Agregar Reporte de Producción

<figure><img src=".gitbook/assets/image (2).png" alt=""><figcaption></figcaption></figure>

Seleccione el archivo XLSX de Producción - RP y haga clic en Abrir:

<figure><img src=".gitbook/assets/image (3).png" alt=""><figcaption></figcaption></figure>

Si el archivo es admitido, el recorrido muestra un mensaje de éxito. Ese aviso de carga no sustituye la verificación del contenido del RP.

También puedes agregar otros RP del mismo cliente si corresponde prepararlos bajo una misma orden. Comprueba **ambientes, números RP y compatibilidad de materiales** antes de agruparlos.

<figure><img src=".gitbook/assets/image (4).png" alt=""><figcaption></figcaption></figure>

Le aparecerán la lista de materiales y la lista de RP seleccionados que va a cortar juntos bajo una misma Orden de Producción.

<figure><img src=".gitbook/assets/image (5).png" alt=""><figcaption></figcaption></figure>

Entre la informacion puede destacar:

<figure><img src=".gitbook/assets/image (6).png" alt=""><figcaption></figcaption></figure>

El Número de Control de OP

La cantidad de piezas que contiene la Producción entre todos los RP

<figure><img src=".gitbook/assets/image (7).png" alt=""><figcaption></figcaption></figure>

La lista de Aglomerados y Cantos:

<figure><img src=".gitbook/assets/image (8).png" alt=""><figcaption></figcaption></figure>

Y la lista de RPs seleccionados:

<figure><img src=".gitbook/assets/image (9).png" alt=""><figcaption></figcaption></figure>

Haga Clic en

Generar Reporte de Producción

<figure><img src=".gitbook/assets/image (11).png" alt=""><figcaption></figcaption></figure>

Seleccione la ubicación donde guardará la Orden de Producción, preferiblemente dentro de la misma carpeta donde estan los archivos de su producción:

<figure><img src=".gitbook/assets/image (12).png" alt=""><figcaption></figcaption></figure>

Si todo sale bien le sale el mensaje de éxito

<figure><img src=".gitbook/assets/image (13).png" alt=""><figcaption></figcaption></figure>

## 3. Verificar el archivo y el registro de la OP

{% hint style="warning" %}
**Un archivo Excel no equivale por sí solo a una orden registrada.** La creación del documento puede depender de la plantilla local y del guardado de las asociaciones entre RP y OP. Si falla la plantilla, el archivo está bloqueado o la aplicación informa un error de registro, no distribuyas la orden como definitiva.
{% endhint %}

Después de generar, verifica el **número de control OP**, el cliente, los RP incluidos, los totales de piezas y el destino del Excel. Si trabajaste sin conexión, vuelve a comprobar los vínculos y el estado del registro cuando recuperes la conectividad; no des por hecha la sincronización.

## 4. Herramientas relacionadas

También puede convertir archivos entre Optimizadores, por ahora entre los 2 optimizadores creados

<figure><img src=".gitbook/assets/image (14).png" alt=""><figcaption></figcaption></figure>

Por ultimo puede fusionar o seprar optimizaciones:

<figure><img src=".gitbook/assets/image (15).png" alt=""><figcaption></figcaption></figure>

Esto por si va a cortar 2 producciones con el mismo material, desde aquí Cabinet Report con un solo clic le unifica las piezas en un solo archivo.

## 5. Comprobación antes de entregar a fabricación

1. Confirma que **cliente, ambientes, RP y número OP** sean correctos y estén asociados de forma coherente.
2. Contrasta piezas, cantidades y tableros/cantos con los reportes originales.
3. Revisa la existencia y apertura del Excel generado y el estado del registro de la OP.
4. Si utilizas las herramientas de conversión o fusión de optimizaciones, verifica por separado la compatibilidad del formato y el listado de piezas resultante.
5. Obtén la autorización correspondiente antes de entregar documentos a corte, montaje o instalación: la OP no acredita la ejecución física.

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
