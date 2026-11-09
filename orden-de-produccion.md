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

Consulta los detalles del alcance, registro y continuidad en la [Documentación oficial — Orden de Producción](https://cabinet-report.gitbook.io/cabinet-report-docs/funcionalidades-de-cabinet-report/orden-de-produccion).

---

[← Reporte de Compras](reporte-de-compras.md) · [Optimizadores →](optimizadores.md) · [🏠 Portal principal](https://danielmelendez-pma.github.io/cabinet-report-partners/)
