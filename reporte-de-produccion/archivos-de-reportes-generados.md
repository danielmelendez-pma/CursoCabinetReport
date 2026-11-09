# Archivos de Reportes Generados

Identifica los archivos de salida que aparecen en el recorrido documentado después de generar la producción. Cada elemento incluye su captura original y la función descrita en el curso.

Después de generar la producción, revisa los archivos disponibles en la carpeta del proyecto. **No todos los tipos enumerados tienen que generarse en cada trabajo:** las salidas dependen del contenido de la producción, las opciones seleccionadas y las integraciones disponibles. Las capturas siguientes muestran las categorías descritas en el recorrido original:

## Identifica el propósito de cada salida

| Grupo de archivos | Para qué se utiliza | Qué no debes asumir |
| --- | --- | --- |
| **TXT de producción** | Conservar los datos de piezas para retomar o reutilizar el trabajo con un formato compatible. | No reemplaza el Excel RP ni acredita que las piezas ya estén aprobadas. |
| **Excel RP (.xlsx)** | Revisar, imprimir y distribuir el reporte tras la validación técnica. | Crear este Excel **no significa** crear o registrar una Orden de Producción (OP). |
| **TXT de herrajes y perfilerías** | Consultar zócalos, tubos, golas, accesorios y ferretería que correspondan. | No todas estas categorías existen en todos los proyectos. |
| **Materiales y optimización** | Consultar materiales utilizados y preparar intercambios con una herramienta de corte compatible. | El listado no acredita stock físico ni garantiza importación en cualquier seccionadora. |
| **Parámetros y otros registros técnicos** | Facilitar la recuperación y trazabilidad según la función y versión. | No deben confundirse con los reportes para fabricación ni editarse manualmente sin respaldo. |

Los nombres de archivo, las ubicaciones y las salidas disponibles pueden variar. Identifica siempre el **archivo concreto generado**, en lugar de depender solo de la captura de este curso.

<figure><img src="../.gitbook/assets/image (4) (1) (1).png" alt=""><figcaption></figcaption></figure>

### Archivo TXT de Zócalos

Archivo donde se guardan los Zócalos que se crearon para esta producción.

<figure><img src="../.gitbook/assets/image (5) (1) (1).png" alt=""><figcaption></figcaption></figure>

### Archivo TXT de Accesorios

Archivo donde se guardan los Accesorios que se crearon para esta producción.

<figure><img src="../.gitbook/assets/image (6) (1).png" alt=""><figcaption></figcaption></figure>

### Archivo TXT de Ferretería de Montaje

Archivo donde se guardan las Ferreterías de Montaje que se crearon para esta producción.

<figure><img src="../.gitbook/assets/image (7) (1).png" alt=""><figcaption></figcaption></figure>

### Archivo TXT de Ferretería de Instalación

Archivo donde se guardan las Ferreterías de Instalación que se crearon para esta producción.

<figure><img src="../.gitbook/assets/image (8) (1).png" alt=""><figcaption></figcaption></figure>

### Archivos TXT de Tubos

Archivo donde se guardan los Tubos que se crearon para esta producción.

<figure><img src="../.gitbook/assets/image (9) (1).png" alt=""><figcaption></figcaption></figure>

### Archivo TXT de Golas

Archivo donde se guardan los Golas que se crearon para esta producción.

<figure><img src="../.gitbook/assets/image (16).png" alt=""><figcaption></figcaption></figure>

### Archivo TXT de Producción

Copia de la producción donde se guarda la lista de piezas, para poder continuar trabajando más adelante.

**Conserva este archivo junto con los datos del proyecto.** Antes de volver a importarlo, verifica cliente, ambiente, columnas y contenido; no lo confundas con el RP imprimible. Consulta el procedimiento [Cargar TXT](cargar-txt.md).

<figure><img src="../.gitbook/assets/image (1) (1) (1) (1).png" alt=""><figcaption></figcaption></figure>

### Archivos del Optimizador de la Seccionadora

Archivo destinado al intercambio con el optimizador de una seccionadora, **cuando existe un formato compatible**. Antes de importarlo, revisa las exigencias del proveedor, la orientación de las piezas, el espesor de sierra y las restricciones del corte; no presupongas compatibilidad universal.

<figure><img src="../.gitbook/assets/image (2) (1).png" alt=""><figcaption></figcaption></figure>

### Archivos de Materiales de Producción

Listado de tableros y cantos asociados a la producción y sus cantidades documentadas. **No equivale a un inventario físico ni acredita existencias disponibles para corte o compra.**

<figure><img src="../.gitbook/assets/image (3) (1).png" alt=""><figcaption></figcaption></figure>

### Archivo XLSX de Reporte de Producción

Reporte de Producción en Excel, destinado a revisar, imprimir y entregar a los responsables de fabricación **después de su aprobación técnica**.

Puede circular entre las áreas de Maquinaria, Montaje, Instalación e Inspección según el flujo de cada empresa. **No lo confundas con una OP registrada**: para agrupar reportes en una orden se sigue otro proceso.

<figure><img src="../.gitbook/assets/image (4) (1).png" alt=""><figcaption></figcaption></figure>

### Archivos TXT de Parámetros de Producción

Guarda datos de parámetros de la producción para su posible reutilización por Cabinet Report al volver a abrir el trabajo. Evita editar estos archivos manualmente sin respaldo y verifica que pertenecen al mismo proyecto.

<figure><img src="../.gitbook/assets/image (93).png" alt=""><figcaption></figcaption></figure>

### Órdenes de Entregas de Herrajes

Son los documentos de Entregas de Herrajes (Accesorios, Ferretería de Montaje y Ferretería de Instalación), que va a entregar a su Almacén y administre los herrajes de manera eficiente y planificada.

<figure><img src="../.gitbook/assets/image (94).png" alt=""><figcaption></figcaption></figure>

## Archivos de apoyo y trazabilidad

Además de las salidas ilustradas, la [Documentación oficial del RP](https://cabinet-report.gitbook.io/cabinet-report-docs/funcionalidades-de-cabinet-report/reporte-de-produccion) describe **metadatos técnicos XML** y un **XML de Auditoría RP** relacionados con la producción y las decisiones de revisión. Son registros con propósitos distintos del TXT de piezas, los parámetros y el Excel imprimible; su presencia o ubicación no debe darse por supuesta para toda instalación.

Si necesitas agrupar varios RP para fabricación, sigue el proceso independiente de [Orden de Producción](../orden-de-produccion.md). Para cortes, consulta los [Optimizadores](../optimizadores.md) y confirma el formato admitido por tu maquinaria. Para revisiones y recuperación, consulta [Auditoría RP y persistencia](https://cabinet-report.gitbook.io/cabinet-report-docs/funcionalidades-de-cabinet-report/auditoria-rp-persistencia).

## Comprobación de los archivos antes de entregar

1. Localiza la **carpeta y destino reales** de esta generación. Comprueba que los nombres de archivo y los documentos abiertos correspondan al **cliente, ambiente y número RP** correctos.
2. Confirma que estén presentes los formatos realmente seleccionados; la lista de capturas **no constituye un conjunto obligatorio**. Si falta una salida esperada, revisa la operación ejecutada antes de distribuir los demás archivos.
3. Abre el **Excel RP y los archivos que vas a entregar**; contrasta cantidades, materiales, piezas, espesores, vetas y cantos con el RP y los planos de fabricación.
4. Comprueba que los complementarios (herrajes, zócalos, tubos y golas) pertenezcan a la misma producción y que sus unidades y cantidades sean adecuadas.
5. Si entregas archivos a una seccionadora o herramienta externa, valida con el operador el formato, el sentido de veta, las restricciones y las condiciones de corte.
6. Conserva un respaldo del origen y de las salidas aprobadas para poder identificar qué versión se envió a fabricación.

{% hint style="warning" %}
**Generar un archivo no equivale a validar su contenido.** Revisa la salida final antes de autorizar fabricación o entrega.
{% endhint %}

---

[← Reporte de Producción](reporte-de-produccion.md) · [Reporte de Compras →](../reporte-de-compras.md) · [🏠 Portal principal](https://danielmelendez-pma.github.io/cabinet-report-partners/)
