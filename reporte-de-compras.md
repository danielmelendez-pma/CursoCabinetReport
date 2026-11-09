# Reporte de Compras

Consulta cómo obtener el resumen de materiales y herrajes de una producción y cómo exportar la información a las plantillas de proveedores ilustradas en esta lección.

Cabinet Report reúne materiales y herrajes para preparar un informe que el departamento de compras puede revisar antes de gestionar pedidos con proveedores. **El Excel generado no realiza compras ni confirma existencias físicas.**

{% hint style="info" %}
**Dos recorridos:** la documentación oficial contempla **Un ambiente** y **Varios ambientes**. Las capturas originales siguientes ilustran principalmente el procedimiento histórico de un ambiente; los controles pueden variar según la versión instalada.
{% endhint %}

## Antes de empezar

1. Genera y revisa el [Reporte de Producción](reporte-de-produccion/README.md) correspondiente.
2. Comprueba **cliente, ambiente, referencia, materiales, cantidades y unidades** de los archivos de origen.
3. Ubica la carpeta del proyecto y los archivos complementarios efectivamente generados; no supongas que todas las categorías estarán presentes.
4. Define si necesitas el informe de **un ambiente** o un **consolidado de varios ambientes**.

## 1. Generar el reporte de un ambiente (capturas originales)

<figure><img src=".gitbook/assets/image (95).png" alt=""><figcaption></figcaption></figure>

**Seleccione Parámetros**

<figure><img src=".gitbook/assets/image (96).png" alt=""><figcaption></figcaption></figure>

Navegue hasta la carpeta de su proyecto y seleccione el archivo de Parámetros y haga clic en Abrir:

<figure><img src=".gitbook/assets/image (98).png" alt=""><figcaption></figcaption></figure>

Se cargan los datos de la producción

<figure><img src=".gitbook/assets/image (99).png" alt=""><figcaption></figcaption></figure>

<figure><img src=".gitbook/assets/image (100).png" alt=""><figcaption></figcaption></figure>

Seleccione Generar Reporte de Compras

En la siguiente ventana, selecciona los **archivos disponibles que correspondan a esta producción**. El ejemplo original muestra estas categorías:

1. MATERIALES
2. FERRETERÍA DE INSTALACIÓN
3. FERRETERÍA DE MONTAJE
4. ACCESORIOS

Selecciona las fuentes pertinentes y haz clic en **Abrir**. Si falta una categoría, verifica primero si se generó para ese trabajo; no sustituyas un archivo faltante por otro de distinto proyecto.

<figure><img src=".gitbook/assets/image (101).png" alt=""><figcaption></figcaption></figure>

Si todo sale bien, le sale el siguiente mensaje de éxito

<figure><img src=".gitbook/assets/image (102).png" alt=""><figcaption></figcaption></figure>

**Se le genera el archivo XLSX con el Reporte de Compras junto con los demás archivos de su producción:**

<figure><img src=".gitbook/assets/image (103).png" alt=""><figcaption></figcaption></figure>

## 2. Consolidar varios ambientes

La modalidad **Varios ambientes**, descrita en la [documentación oficial del Reporte de Compras](https://cabinet-report.gitbook.io/cabinet-report-docs/funcionalidades-de-cabinet-report/reporte-de-compras), permite reunir fuentes de varias carpetas `Materiales` bajo un cliente y una referencia de consolidación.

1. Selecciona la carpeta principal o agrega las carpetas de materiales admitidas en tu versión.
2. Identifica y marca únicamente los ambientes que deban incluirse; comprueba especialmente si aparecen **clientes distintos**.
3. Genera el Excel consolidado y comprueba la **hoja Trazabilidad**, las exclusiones y las advertencias registradas.
4. Revisa el TXT auxiliar de trazabilidad y, si corresponde, las órdenes de perfilería opcionales.

{% hint style="warning" %}
**No mezcles proyectos por coincidencia de nombres.** Revisa el cliente oficial y la referencia del consolidado. Comprueba las unidades de tubos, golas, zócalos y otros materiales: una cifra puede representar unidades, tramos o longitud. No guardes el consolidado dentro de la carpeta de origen `Materiales`.
{% endhint %}

### Archivos adicionales según las opciones seleccionadas

<figure><img src=".gitbook/assets/image (105).png" alt=""><figcaption></figcaption></figure>

**Se generan los archivos de cortes de Perfilarías con la optimización de corte lista para entregar a su departamento de perfilerías con el plan de trabajo de corte:**

<figure><img src=".gitbook/assets/image (104).png" alt=""><figcaption></figcaption></figure>

## Que más puede hacer desde la Ventaja de **Reporte de Compras?**

Exportar su producción a los archivo plantillas de su proveedor de corte y canteo preferído:

<figure><img src=".gitbook/assets/image (106).png" alt=""><figcaption></figcaption></figure>

Las capturas de esta lección muestran plantillas de:

- LMD Kitchens & Cabinets
- FD Center
- MOBY Suplies
- TANDOR Comercial
- MULTILAMINAS

Solo debe hacer clic en el proveedor con el que va a cortar y cantear su producción, seleccionar el archivo TXT de Producción y Abrir:

<figure><img src=".gitbook/assets/image (107).png" alt=""><figcaption></figcaption></figure>

En la siguiente ventana seleccione los tableros que va a cortar y cantear con el proveedor y también puede colocar el código del material.

La captura histórica describe una opción para indicar la **medida mínima de corte y canteo** del proveedor y ajustar piezas inferiores a ese límite:

<figure><img src=".gitbook/assets/image (108).png" alt=""><figcaption></figcaption></figure>

{% hint style="warning" %}
**Un mínimo de proveedor puede alterar dimensiones de corte.** No consideres una pieza ajustada como equivalente a la medida del diseño. Antes de autorizar la exportación, compara las medidas originales y las exportadas, confirma las tolerancias y coordina cualquier corrección con el responsable técnico. La disponibilidad y el comportamiento exacto de esta opción deben verificarse en la versión instalada.
{% endhint %}

Si quiere agregar otro TXT de Producción para cortar junto, puede agregarlo haciendo clic aquí:

<figure><img src=".gitbook/assets/image (110).png" alt=""><figcaption></figcaption></figure>

Cuando todo esté listo para exportar la producción a la plantilla del proveedor, haga clic en **Exportar**:

<figure><img src=".gitbook/assets/image (111).png" alt=""><figcaption></figcaption></figure>

Seleccione la carpeta de destino o la de su producción y haga clic en Guardar:

<figure><img src=".gitbook/assets/image (112).png" alt=""><figcaption></figcaption></figure>

Si todo sale bien, le sale el mensaje de éxito:

<figure><img src=".gitbook/assets/image (113).png" alt=""><figcaption></figcaption></figure>

El recorrido ilustrado finaliza con una **plantilla XLSX** del proveedor. Antes de entregarla, comprueba que se haya completado correctamente y que el formato siga siendo aceptado por el proveedor; la exportación **no representa un pedido realizado ni una aprobación técnica automática**:

<figure><img src=".gitbook/assets/image (114).png" alt=""><figcaption></figcaption></figure>

## Comprobación antes de comprar o enviar a corte

- **Procedencia:** confirma cliente, ambiente(s), referencia y archivos seleccionados.
- **Contenido:** coteja materiales, espesores, unidades, cantidades y partidas faltantes con el RP.
- **Consolidación:** si incluiste varios ambientes, revisa las advertencias y la trazabilidad de inclusiones y exclusiones.
- **Proveedor:** comprueba códigos de tablero, formato de plantilla y medidas mínimas; no aceptes ajustes de corte sin revisión técnica.
- **Gestión comercial:** confirma stock real, precios, plazos, impuestos y autorizaciones antes de enviar una orden de compra.

Para consultar el alcance actualizado de ambas modalidades, visita la [Documentación oficial — Reporte de Compras](https://cabinet-report.gitbook.io/cabinet-report-docs/funcionalidades-de-cabinet-report/reporte-de-compras).


## Ensayo reproducible: del reporte de compras a la recepción de materiales

Este ensayo complementa la generación del Excel con un **control manual de abastecimiento y entrega a fabricación**. No es una función de recepción, reserva de inventario ni liberación automática atribuida a Cabinet Report. Sirve para comprobar que lo solicitado, lo recibido y lo destinado a cada ambiente corresponden a la misma producción.

### 1. Preparar las referencias del control

1. Conserva copia de los **RP revisados**, sus archivos de materiales y el **Excel de Compras** realmente generado. Identifica cliente, ambiente, referencia, fecha, versión del archivo y responsable; si usaste **Varios ambientes**, guarda también la hoja y el TXT de trazabilidad.
2. Comprueba qué ambientes y fuentes fueron **incluidos o excluidos**. Si el Excel consolidado no desglosa las partidas por ambiente, utiliza los archivos originales para reconstruir ese reparto; **no atribuyas cantidades por suposición**.
3. Anota por partida la **descripción completa, material, espesor, formato/presentación y unidad de compra**. Convierte paquetes, hojas, metros o unidades solo cuando conozcas y puedas demostrar su equivalencia. No sumes unidades distintas.
4. Registra por separado el documento enviado al proveedor, el comprobante de recepción y la verificación física. **Un Excel de Compras no demuestra que exista un pedido emitido ni que el material haya llegado.**

### 2. Ejemplo didáctico con dos ambientes

Supón que un consolidado revisado de **un mismo cliente** requiere las siguientes cantidades. Son cifras inventadas para practicar el control, **no resultados de Cabinet Report, consumos estándar ni reglas de cálculo del RP**. «Ambiente A» y «Ambiente B» representan dos fuentes que el responsable ya comprobó.

| Insumo y especificación ilustrativa | Unidad | Ambiente A | Ambiente B | Total solicitado | Recibido conforme | Pendiente |
| --- | --- | ---: | ---: | ---: | ---: | ---: |
| Tablero blanco, **18 mm**, formato acordado | hojas | 3 | 2 | **5** | **4** | **1** |
| Canto blanco, **22 mm** de ancho | metros | 20 | 20 | **40** | **30** | **10** |
| Bisagra modelo X, referencia confirmada | unidades | 8 | 16 | **24** | **24** | **0** |

Para verificar el ejemplo:

1. Suma por ambiente **únicamente dentro de la misma partida y unidad**: tableros 3 + 2 = 5, canto 20 + 20 = 40 y bisagras 8 + 16 = 24.
2. Contrasta lo recibido **físicamente y conforme a especificación**, no solo el número de bultos de la factura. En este ejemplo llegan cuatro tableros correctos; falta uno.
3. Imagina que llegan 40 metros de cinta, pero **10 metros tienen 19 mm de ancho** en vez de los 22 mm solicitados. Por eso solo **30 metros son conformes** y permanecen pendientes 10; la coincidencia de cantidad bruta no resuelve una diferencia técnica.
4. Aunque las 24 bisagras sean conformes, **el lote completo no está apto para liberación a fabricación** por los faltantes de tablero y canto. No compenses un material con otro ni distribuyas el faltante silenciosamente entre ambientes.

### 3. Conciliar y autorizar la salida del almacén

En una hoja de control externa o acta de recepción, utiliza una fila **por especificación y unidad homogénea**, con estos campos mínimos:

| Campo del control | Evidencia que debe conservarse |
| --- | --- |
| Origen | Cliente, ambiente, RP, referencia, versión de Excel de Compras y archivos seleccionados |
| Solicitud | Partida, código o descripción del material, espesor/formato, unidad y cantidad requerida |
| Recepción | Documento de entrega, fecha, cantidad física, especificación comprobada y responsable |
| Diferencia | Cantidad pendiente, material no conforme, motivo y acción correctiva |
| Destino | Ambiente o frente de trabajo autorizado, cantidad asignada y registro de entrega |
| Aprobación | Responsable, fecha y decisión; vínculo a los documentos de respaldo |

**Criterios del ensayo:**

- **APTO PARA LIBERACIÓN:** todas las partidas requeridas para el alcance autorizado están recibidas y conformes, su unidad es comparable y la distribución por ambiente está documentada.
- **NO APTO:** hay faltantes, materiales con especificación distinta, fuentes no conciliadas o dudas sobre el cliente y el ambiente. Mantén esas partidas fuera de fabricación hasta resolverlas.
- **LIBERACIÓN PARCIAL CONTROLADA:** solo si se identifica **qué ambiente o trabajo específico** tiene todos sus insumos conformes, el responsable autoriza esa salida y queda documentado lo que sigue pendiente. No equivale a dar por completado el consolidado.

Si cambia el RP, la selección de ambientes o la especificación aprobada, conserva las versiones anteriores y **repite la conciliación** antes de continuar. La prueba se considera reproducible cuando otra persona puede seguir cada cantidad desde su fuente hasta la recepción y el destino, sin depender de una suma global ni de confirmaciones verbales.

Para enlazar el control con las etapas siguientes, consulta [Orden de Producción](orden-de-produccion.md), [Optimizadores](optimizadores.md) y el [índice del Reporte de Producción](reporte-de-produccion/README.md). Antes de entregar una plantilla al proveedor de corte y canteo, conserva adicionalmente la comparación entre dimensiones aprobadas y exportadas explicada en esta misma lección.


---

[← Reporte de Producción](reporte-de-produccion/README.md) · [Orden de Producción →](orden-de-produccion.md) · [🏠 Portal principal](https://danielmelendez-pma.github.io/cabinet-report-partners/)
