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

---

[← Reporte de Producción](reporte-de-produccion/README.md) · [Orden de Producción →](orden-de-produccion.md) · [🏠 Portal principal](https://danielmelendez-pma.github.io/cabinet-report-partners/)
