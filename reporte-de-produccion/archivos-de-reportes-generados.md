# Archivos de Reportes Generados

Identifica los archivos de salida que aparecen en el recorrido documentado después de generar la producción. Cada elemento incluye su captura original y la función descrita en el curso.

Después de generar la producción, revisa los archivos disponibles en la carpeta del proyecto. **No todos los tipos enumerados tienen que generarse en cada trabajo:** las salidas dependen del contenido de la producción, las opciones seleccionadas y las integraciones disponibles. Las capturas siguientes muestran las categorías descritas en el recorrido original:

## Identifica la salida según la tarea

Usa los enlaces de esta tabla para ir a la captura de la categoría que necesitas. Los archivos ilustrados son **ejemplos históricos**: verifica los nombres y formatos realmente producidos en tu instalación. Para la entrega, ve directamente a la [comprobación final](#comprobación-de-los-archivos-antes-de-entregar).

| Necesitas… | Abre esta sección | Comprueba antes de utilizar el archivo |
| --- | --- | --- |
| **Retomar un trabajo de piezas** | [TXT de producción](#archivo-txt-de-producción) | No sustituye el Excel RP imprimible ni demuestra que las piezas estén aprobadas. |
| **Revisar, imprimir o entregar el reporte** | [Excel RP (.xlsx)](#archivo-xlsx-de-reporte-de-producción) | El RP generado debe revisarse; **no equivale** a una Orden de Producción (OP) registrada. |
| **Consultar complementos del trabajo** | [Zócalos](#archivo-txt-de-zócalos), [accesorios](#archivo-txt-de-accesorios), [ferretería de montaje](#archivo-txt-de-ferretería-de-montaje), [ferretería de instalación](#archivo-txt-de-ferretería-de-instalación), [tubos](#archivos-txt-de-tubos) y [golas](#archivo-txt-de-golas) | No presupongas que todas las categorías existen ni que sus cantidades están conciliadas. |
| **Preparar materiales o intercambio con corte** | [Materiales de producción](#archivos-de-materiales-de-producción) y [archivos para la seccionadora](#archivos-del-optimizador-de-la-seccionadora) | El listado no acredita inventario físico; el archivo de máquina requiere comprobar formato y lectura en destino. |
| **Conservar parámetros y trazabilidad** | [TXT de parámetros](#archivos-txt-de-parámetros-de-producción) y [archivos de apoyo](#archivos-de-apoyo-y-trazabilidad) | No son equivalentes al TXT de piezas ni al RP, y su recuperación debe verificarse por separado. |
| **Documentar una entrega de herrajes** | [Órdenes de Entregas de Herrajes](#órdenes-de-entregas-de-herrajes) | Revisa las partidas y su correspondencia con el trabajo antes de distribuirlas. |

Los nombres de archivo, las ubicaciones y las salidas disponibles pueden variar. Identifica siempre el **archivo concreto generado**, en lugar de depender solo de la captura de este curso.

<figure><img src="../.gitbook/assets/image (4) (1) (1).png" alt="Vista histórica de ejemplo de los archivos de salida de producción"><figcaption><p>Vista ilustrativa de una generación: la lista real depende del trabajo y de las opciones utilizadas.</p></figcaption></figure>

### Archivo TXT de Zócalos

Archivo donde se guardan los Zócalos que se crearon para esta producción.

<figure><img src="../.gitbook/assets/image (5) (1) (1).png" alt="Captura histórica del TXT de zócalos de producción"><figcaption><p>Ejemplo de TXT de zócalos; comprueba que corresponde al proyecto antes de usarlo.</p></figcaption></figure>

### Archivo TXT de Accesorios

Archivo donde se guardan los Accesorios que se crearon para esta producción.

<figure><img src="../.gitbook/assets/image (6) (1).png" alt="Captura histórica del TXT de accesorios de producción"><figcaption><p>Ejemplo de TXT de accesorios; concilia sus cantidades con el RP.</p></figcaption></figure>

### Archivo TXT de Ferretería de Montaje

Archivo donde se guardan las Ferreterías de Montaje que se crearon para esta producción.

<figure><img src="../.gitbook/assets/image (7) (1).png" alt="Captura histórica del TXT de ferretería de montaje"><figcaption><p>Ejemplo de ferretería de montaje; confirma que sus partidas corresponden a esta producción.</p></figcaption></figure>

### Archivo TXT de Ferretería de Instalación

Archivo donde se guardan las Ferreterías de Instalación que se crearon para esta producción.

<figure><img src="../.gitbook/assets/image (8) (1).png" alt="Captura histórica del TXT de ferretería de instalación"><figcaption><p>Ejemplo de ferretería de instalación; verifica cantidades y destino.</p></figcaption></figure>

### Archivos TXT de Tubos

Archivo donde se guardan los Tubos que se crearon para esta producción.

<figure><img src="../.gitbook/assets/image (9) (1).png" alt="Captura histórica de los archivos TXT de tubos de producción"><figcaption><p>Ejemplo de tubos; su presencia depende de los componentes del trabajo.</p></figcaption></figure>

### Archivo TXT de Golas

Archivo donde se guardan los Golas que se crearon para esta producción.

<figure><img src="../.gitbook/assets/image (16).png" alt="Captura histórica del TXT de golas de producción"><figcaption><p>Ejemplo de golas; revisa referencias y cantidades de la producción.</p></figcaption></figure>

### Archivo TXT de Producción

Copia de la producción donde se guarda la lista de piezas, para poder continuar trabajando más adelante.

**Conserva este archivo junto con los datos del proyecto.** Antes de volver a importarlo, verifica cliente, ambiente, columnas y contenido; no lo confundas con el RP imprimible. Consulta el procedimiento [Cargar TXT](cargar-txt.md).

<figure><img src="../.gitbook/assets/image (1) (1) (1) (1).png" alt="Captura histórica del TXT de piezas de producción"><figcaption><p>El TXT de piezas sirve para retomar datos compatibles; no sustituye la revisión del Excel RP.</p></figcaption></figure>

### Archivos del Optimizador de la Seccionadora

Archivo destinado al intercambio con el optimizador de una seccionadora, **cuando existe un formato compatible**. Antes de importarlo, revisa las exigencias del proveedor, la orientación de las piezas, el espesor de sierra y las restricciones del corte; no presupongas compatibilidad universal.

<figure><img src="../.gitbook/assets/image (2) (1).png" alt="Captura histórica del archivo destinado al optimizador de seccionadora"><figcaption><p>La compatibilidad del archivo de corte debe confirmarse con el operador o proveedor de la máquina.</p></figcaption></figure>

### Archivos de Materiales de Producción

Listado de tableros y cantos asociados a la producción y sus cantidades documentadas. **No equivale a un inventario físico ni acredita existencias disponibles para corte o compra.**

<figure><img src="../.gitbook/assets/image (3) (1).png" alt="Captura histórica del archivo de materiales utilizados en producción"><figcaption><p>El listado de materiales es una referencia de producción, no una certificación de existencias.</p></figcaption></figure>

### Archivo XLSX de Reporte de Producción

Reporte de Producción en Excel, destinado a revisar, imprimir y entregar a los responsables de fabricación **después de su aprobación técnica**.

Puede circular entre las áreas de Maquinaria, Montaje, Instalación e Inspección según el flujo de cada empresa. **No lo confundas con una OP registrada**: para agrupar reportes en una orden se sigue otro proceso.

<figure><img src="../.gitbook/assets/image (4) (1).png" alt="Captura histórica del reporte de producción en Excel XLSX"><figcaption><p>El Excel RP es el reporte para revisión y entrega; generarlo no registra automáticamente una OP.</p></figcaption></figure>

### Archivos TXT de Parámetros de Producción

Guarda datos de parámetros de la producción para su posible reutilización por Cabinet Report al volver a abrir el trabajo. Evita editar estos archivos manualmente sin respaldo y verifica que pertenecen al mismo proyecto.

<figure><img src="../.gitbook/assets/image (93).png" alt="Captura histórica de los archivos TXT de parámetros de producción"><figcaption><p>Estos TXT conservan parámetros técnicos; verifica su pertenencia al proyecto antes de reutilizarlos.</p></figcaption></figure>

### Órdenes de Entregas de Herrajes

Son los documentos de Entregas de Herrajes (Accesorios, Ferretería de Montaje y Ferretería de Instalación), que va a entregar a su Almacén y administre los herrajes de manera eficiente y planificada.

<figure><img src="../.gitbook/assets/image (94).png" alt="Captura histórica de las órdenes de entrega de herrajes"><figcaption><p>Documentos de entrega de herrajes: confirma destinatario, partidas y cantidades.</p></figcaption></figure>

## Archivos de apoyo y trazabilidad

Además de las salidas ilustradas, la [Documentación oficial del RP](https://cabinet-report.gitbook.io/cabinet-report-docs/funcionalidades-de-cabinet-report/reporte-de-produccion) describe **metadatos técnicos XML** y un **XML de Auditoría RP** relacionados con la producción y las decisiones de revisión. Son registros con propósitos distintos del TXT de piezas, los parámetros y el Excel imprimible; su presencia o ubicación no debe darse por supuesta para toda instalación.

Si necesitas agrupar varios RP para fabricación, sigue el proceso independiente de [Orden de Producción](../orden-de-produccion.md). Para cortes, consulta los [Optimizadores](../optimizadores.md) y confirma el formato admitido por tu maquinaria. Para revisiones y recuperación, consulta [Auditoría RP y persistencia](https://cabinet-report.gitbook.io/cabinet-report-docs/funcionalidades-de-cabinet-report/reporte-de-produccion/auditoria-rp-persistencia).

## Ensayo reproducible: conciliación del paquete de corte

Este ensayo aporta una prueba práctica para contrastar el **RP aprobado**, el **TXT de producción** y el **archivo destinado a la seccionadora o al proveedor de corte**, cuando ese último archivo se haya generado. Es un **control documental y operativo realizado por personas**, no una función de conciliación automática atribuida a Cabinet Report.

### 1. Preparar una referencia inalterada

1. Identifica **cliente, ambiente, número RP (si existe), fecha y responsable** de la revisión. Conserva una copia del RP aprobado, del TXT de origen y de la salida de corte realmente seleccionada; evita comparar archivos de generaciones diferentes.
2. Asegúrate de que el RP contiene las modificaciones aprobadas. Si se cambia alguna pieza después, **no reutilices la aprobación anterior**: vuelve a contrastar las salidas de esa nueva generación.
3. Abre cada archivo con una herramienta compatible y registra su **nombre, ruta y fecha de generación**. La existencia del archivo no demuestra que su contenido se haya importado correctamente en la maquinaria.

### 2. Caso de prueba: el total coincide, pero el material no

Usa los siguientes datos **únicamente como ejemplo didáctico de conciliación**; no son fórmulas de Cabinet Report, valores obligatorios ni un despiece listo para fabricar.

| Referencia del RP aprobado | Pieza | Material | Espesor | Ancho × largo | Cantidad |
| --- | --- | --- | --- | --- | --- |
| M-01 | COSTADO | Tablero A | 18 mm | 400 × 700 mm | 2 |
| M-02 | COSTADO | Tablero B | 18 mm | 400 × 700 mm | 2 |
| **Total** | | | | | **4** |

Supón que el TXT reproduce las cantidades aprobadas, pero que en el archivo preparado para corte aparecen **3 piezas del Tablero A y 1 del Tablero B**. El total sigue siendo **4**, aunque la distribución correcta es **2 del Tablero A y 2 del Tablero B**.

**Resultado esperado:** **NO APTO PARA CORTE**. Registra una pieza excedente del Tablero A y una faltante del Tablero B, identifica el origen del desajuste y vuelve a generar o corregir la salida por el procedimiento autorizado. No compenses materiales distintos solo porque las dimensiones coincidan.

### 3. Repetir la conciliación sobre una producción real

1. **Cruza las partidas, no solo los totales:** compara por pieza o por agrupación demostrablemente equivalente el material, espesor, ancho, largo y cantidad. Revisa también **veta, sentido y cantos por lado** donde figuren en las fuentes; una salida de máquina puede no conservar todos los campos del RP.
2. **Comprueba la agrupación:** si el formato de corte agrupa piezas idénticas y omite el módulo, compara la suma por material y dimensiones **sin inventar una asignación por módulo**. Conserva el RP para justificar la procedencia de cada cantidad.
3. **Distingue medidas de diseño y de corte:** si aparecen diferencias por resane, sierra, canteo, mínimos de máquina u otros ajustes, solicita la regla aplicable y la autorización técnica antes de aceptarlas. No presupongas que dos medidas diferentes son intercambiables.
4. **Valida el destino:** consulta con el operador o proveedor el formato admitido, unidades, codificación de material, orientación y cantidad que su sistema **interpreta tras la importación**. Una exportación exitosa por sí sola no acredita esa lectura.
5. **Cierra las discrepancias:** registra partida afectada, diferencia observada, corrección, archivo regenerado y nueva comprobación. No remitas a corte una versión anterior mezclada con archivos actualizados.

### 4. Registrar la liberación o la detención

| Evidencia mínima | Qué anotar |
| --- | --- |
| Identificación | Cliente, ambiente, número RP si corresponde y versión o fecha del paquete |
| Fuentes verificadas | Nombres y rutas del RP, TXT y salida(s) para corte efectivamente usadas |
| Conciliación | Cantidades por material y espesor, diferencias de medidas, veta o cantos que deban revisarse |
| Lectura de destino | Máquina o proveedor, formato comprobado y resultado de la importación, si aplica |
| Decisión | **APTO / NO APTO**, responsable, fecha y detalle de correcciones y nueva revisión |

**Criterio de aceptación:** el contenido aprobado y las salidas destinadas a fabricación son conciliables; las transformaciones de medidas y orientaciones están justificadas; no quedan diferencias de material o cantidad sin resolver; y el destinatario confirmó la lectura de los archivos que realmente utilizará. **Si falla cualquiera de estos controles, detén la entrega a corte** hasta obtener una nueva versión revisada.

Para continuar, consulta el procedimiento de [Optimizadores](../optimizadores.md) y, cuando corresponda, la revisión de plantillas y mínimos de proveedor del [Reporte de Compras](../reporte-de-compras.md). Los XML de metadatos, auditoría y parámetros deben conservarse para trazabilidad según su finalidad; **no son automáticamente parte del paquete que se envía a una máquina**.

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
