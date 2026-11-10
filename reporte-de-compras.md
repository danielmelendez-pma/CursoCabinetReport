---
description: >-
  Guía para generar y verificar el Reporte de Compras de uno o varios ambientes,
  conciliar materiales y unidades, y exportar plantillas de proveedores.
layout:
  width: wide
---

# Reporte de Compras

Consulta cómo obtener el resumen de materiales y herrajes de una producción y cómo exportar la información a las plantillas de proveedores ilustradas en esta lección.

Cabinet Report reúne materiales y herrajes para preparar un informe que el departamento de compras puede revisar antes de gestionar pedidos con proveedores. **El Excel generado no realiza compras ni confirma existencias físicas.**

{% hint style="info" %}
**Dos recorridos:** la documentación oficial contempla **Un ambiente** y **Varios ambientes**. Las capturas originales siguientes ilustran principalmente el procedimiento histórico de un ambiente; los controles pueden variar según la versión instalada.
{% endhint %}

## Del RP revisado a la preparación de compras

El punto de partida es el [Reporte de Producción revisado](reporte-de-produccion/README.md) junto con los **archivos de materiales y complementarios de ese mismo trabajo**. El Reporte de Compras prepara un **Excel para revisar necesidades de abastecimiento**; el pedido, la recepción y la autorización de materiales son comprobaciones externas. Si lo que necesitas es agrupar RP para fabricación, sigue [Orden de Producción](orden-de-produccion.md). Para localizar un trabajo anterior, consulta [Explorador de Proyectos](explorador-de-proyectos.md).

| Documento | Finalidad | Qué no acredita |
| --- | --- | --- |
| **Reporte de Producción (RP)** | Despiece y datos técnicos de piezas, cantidades, materiales, vetas y cantos. | Ni compra de insumos ni ejecución física de fabricación. |
| **Reporte de Compras (RC)** | Relación y consolidación de materiales y complementarios a partir de archivos admitidos. | Ni pedido emitido, ni existencias reservadas, ni recepción. |
| **Orden de Producción (OP)** | Agrupación de **RP en Excel** para organizar la fabricación. | Ni sustituye al RC, ni acredita que la orden se haya ejecutado. |

Los documentos cumplen funciones distintas. La **cantidad de piezas** del RP no equivale automáticamente a **hojas, metros, tramos, cajas o kits** de abastecimiento: cualquier conversión debe verificarse y documentarse.


## Antes de empezar

1. Genera y revisa el [Reporte de Producción](reporte-de-produccion/README.md) correspondiente.
2. Comprueba **cliente, ambiente, referencia, materiales, cantidades y unidades** de los archivos de origen.
3. Ubica la carpeta del proyecto y los archivos complementarios efectivamente generados; no supongas que todas las categorías estarán presentes.
4. Define si necesitas el informe de **un ambiente** o un **consolidado de varios ambientes**.

### Identificar materiales y unidades

| Partida | Especificación que debes reconocer | Unidad/presentación por comprobar |
| --- | --- | --- |
| **Tableros** | Material, fabricante o código, espesor, formato, acabado y veta si corresponde. | Piezas del RP frente a hojas o planchas comerciales; no son equivalentes automáticamente. |
| **Cantos** | Color/acabado, ancho, espesor, tipo y referencia. | Longitud de canteo frente a rollos, metros u otra unidad ofertada. |
| **Accesorios** | Modelo, código y función en el mueble. | Unidades, pares, juegos o kits. |
| **Ferretería de montaje** | Herrajes y fijaciones para ensamblar piezas. | Unidad o empaque real de la referencia. |
| **Ferretería de instalación** | Elementos de fijación o instalación en obra, cuando se incluyan. | Unidad o presentación comercial, separada del montaje. |
| **Tubos, golas, zócalos y perfilería** | Perfil, acabado, medidas y, si procede, condiciones del corte. | Unidades, tramos o longitud lineal. |

Las unidades indicadas son **ejemplos que el usuario debe contrastar**, no nombres de columnas garantizados en todos los Excel. Las categorías dependen de los archivos efectivamente presentes. Consulta [Creación de Tableros](creacion-de-tableros.md) y [Creación de Herrajes](creacion-de-herrajes/README.md) para comprobar las referencias.

### Reglas de agrupación y cantidades

- **Agrupa solo partidas equivalentes:** contrasta código o referencia, fabricante, material, acabado, espesor, medidas, veta cuando aplique, ancho de canto y unidad. Si hay dudas o campos ausentes, separa las partidas hasta confirmar.
- **No confundas catálogo con inventario:** una referencia registrada o un código de proveedor no demuestran existencias, reservas, precio vigente ni aceptación comercial.
- **Documenta conversiones:** pasar del RP a hojas, metros o paquetes requiere conocer formato, rendimiento, merma contemplada, longitudes útiles y contenido del embalaje. No sumes unidades heterogéneas ni supongas redondeos universales.
- **Conserva la procedencia:** registra archivo y ambiente de origen para detectar duplicados, versiones antiguas y diferencias al consolidar.


## 1. Generar el reporte de un ambiente (capturas originales)

La [documentación oficial](https://cabinet-report.gitbook.io/cabinet-report-docs/funcionalidades-de-cabinet-report/reporte-de-compras) describe la modalidad **Un ambiente**: seleccionar la modalidad, identificar **cliente, ambiente y referencia**, elegir las fuentes admitidas y generar el Excel. Las capturas de este curso conservan un procedimiento histórico mediante **archivo de Parámetros**; no presupongas que ese paso aparece igual en todas las versiones instaladas.


<figure><img src=".gitbook/assets/image (95).png" alt="Pantalla inicial del recorrido de Reporte de Compras"><figcaption><p>Inicio del procedimiento de compras mostrado en la versión ilustrada.</p></figcaption></figure>

**Seleccione Parámetros**

<figure><img src=".gitbook/assets/image (96).png" alt="Opción para seleccionar los parámetros de producción"><figcaption><p>El recorrido comienza identificando los parámetros del trabajo correcto.</p></figcaption></figure>

Navegue hasta la carpeta de su proyecto y seleccione el archivo de Parámetros y haga clic en Abrir:

<figure><img src=".gitbook/assets/image (98).png" alt="Selección del archivo de parámetros dentro de la carpeta del proyecto"><figcaption><p>Comprueba la carpeta, el cliente y el ambiente antes de abrir el archivo.</p></figcaption></figure>

Se cargan los datos de la producción

<figure><img src=".gitbook/assets/image (99).png" alt="Vista de los datos de la producción cargados desde parámetros"><figcaption><p>Revisa que la información cargada pertenezca a esta producción.</p></figcaption></figure>

<figure><img src=".gitbook/assets/image (100).png" alt="Continuación de la vista de producción previa al reporte de compras"><figcaption><p>Confirma los datos de origen antes de solicitar el reporte.</p></figcaption></figure>

Seleccione Generar Reporte de Compras

En la siguiente ventana, selecciona los **archivos disponibles que correspondan a esta producción**. El ejemplo original muestra estas categorías:

1. MATERIALES
2. FERRETERÍA DE INSTALACIÓN
3. FERRETERÍA DE MONTAJE
4. ACCESORIOS

Selecciona las fuentes pertinentes y haz clic en **Abrir**. Si falta una categoría, verifica primero si se generó para ese trabajo; no sustituyas un archivo faltante por otro de distinto proyecto.

<figure><img src=".gitbook/assets/image (101).png" alt="Selección de archivos de materiales, ferretería y accesorios"><figcaption><p>Selecciona únicamente los archivos disponibles de la misma producción.</p></figcaption></figure>

Si la generación termina correctamente, el recorrido ilustrado muestra un mensaje de éxito. **Ese aviso no demuestra que el archivo esté completo:**

<figure><img src=".gitbook/assets/image (102).png" alt="Mensaje de confirmación de la generación del Reporte de Compras"><figcaption><p>Un mensaje de éxito no sustituye la revisión del Excel producido.</p></figcaption></figure>

**El recorrido histórico muestra el XLSX del Reporte de Compras junto con otros archivos de producción.** Verifica el destino y abre el archivo para comprobarlo:

<figure><img src=".gitbook/assets/image (103).png" alt="Ejemplo del archivo XLSX de compras junto a otros archivos del proyecto"><figcaption><p>Comprueba el archivo XLSX generado y su ubicación real.</p></figcaption></figure>

## 2. Consolidar varios ambientes

La modalidad **Varios ambientes**, descrita en la [documentación oficial del Reporte de Compras](https://cabinet-report.gitbook.io/cabinet-report-docs/funcionalidades-de-cabinet-report/reporte-de-compras), permite reunir fuentes de varias carpetas `Materiales` bajo un cliente y una referencia de consolidación.

1. Selecciona la carpeta principal o agrega las carpetas de materiales admitidas en tu versión.
2. Identifica y marca únicamente los ambientes que deban incluirse; comprueba especialmente si aparecen **clientes distintos**.
3. Genera el Excel consolidado y comprueba la **hoja Trazabilidad**, las exclusiones y las advertencias registradas.
4. Revisa el TXT auxiliar de trazabilidad y, si corresponde, las órdenes de perfilería opcionales.

### Control del consolidado

- Contrasta los **ambientes seleccionados** con los **incluidos y excluidos** en la hoja **Trazabilidad** y, cuando exista, en el TXT auxiliar. Revisa las advertencias y órdenes registradas.
- Busca **carpetas repetidas, copias antiguas y dos versiones de un mismo ambiente**. No presupongas que la aplicación elimina automáticamente una fuente duplicada.
- Si faltan parámetros complementarios en algún ambiente pero existen archivos válidos, la documentación oficial señala que la consolidación **puede continuar con advertencias**. Comprueba manualmente qué partidas quedaron afectadas.
- Mantén el consolidado separado de las carpetas de origen y registra la selección exacta para poder reproducir la suma.


{% hint style="warning" %}
**No mezcles proyectos por coincidencia de nombres.** Revisa el cliente oficial y la referencia del consolidado. Comprueba las unidades de tubos, golas, zócalos y otros materiales: una cifra puede representar unidades, tramos o longitud. No guardes el consolidado dentro de la carpeta de origen `Materiales`.
{% endhint %}

### Archivos adicionales según las opciones seleccionadas

<figure><img src=".gitbook/assets/image (105).png" alt="Opciones históricas de archivos adicionales de compras"><figcaption><p>La disponibilidad de salidas adicionales depende de las opciones utilizadas.</p></figcaption></figure>

**Si los archivos y las opciones disponibles lo permiten, pueden generarse salidas de corte de perfilería.** Antes de remitirlas, comprueba perfiles, longitudes, unidades y restricciones del proceso:

<figure><img src=".gitbook/assets/image (104).png" alt="Ejemplo de archivos con plan de corte de perfilería"><figcaption><p>Revisa las unidades y las condiciones de corte antes de remitir a perfilería.</p></figcaption></figure>

## 3. Exportar a plantillas de corte y canteo

Además del Excel de compras, las capturas históricas ilustran la exportación a plantillas de proveedores de corte y canteo. **Comprueba primero la opción disponible en tu versión y el formato solicitado por el proveedor.**

<figure><img src=".gitbook/assets/image (106).png" alt="Opciones para exportar a plantillas de proveedores de corte y canteo"><figcaption><p>Selecciona un formato de proveedor solo tras comprobar su compatibilidad vigente.</p></figcaption></figure>

Las capturas de esta lección muestran plantillas de:

- LMD Kitchens & Cabinets
- FD Center
- MOBY Suplies
- TANDOR Comercial
- MULTILAMINAS

Estos nombres se muestran como **referencias de las capturas históricas**. No confirman convenios vigentes, compatibilidad de toda versión ni aceptación actual del formato por parte de esos proveedores.


Selecciona la plantilla del proveedor correspondiente y localiza el **TXT de producción revisado**. Confirma cliente, ambiente y referencia antes de abrirlo:

<figure><img src=".gitbook/assets/image (107).png" alt="Selección del TXT de producción destinado a la plantilla del proveedor"><figcaption><p>El TXT seleccionado debe corresponder a la producción revisada.</p></figcaption></figure>

En el paso ilustrado, selecciona los tableros destinados al proveedor y, cuando corresponda, indica sus códigos de material. Comprueba que coincidan con la referencia acordada.

La captura histórica describe una opción para indicar la **medida mínima de corte y canteo** del proveedor y ajustar piezas inferiores a ese límite:

<figure><img src=".gitbook/assets/image (108).png" alt="Selección de tableros, códigos y medida mínima de corte del proveedor"><figcaption><p>Verifica los códigos y cualquier cambio de medida antes de aprobar la exportación.</p></figcaption></figure>

{% hint style="warning" %}
**Un mínimo de proveedor puede alterar dimensiones de corte.** No consideres una pieza ajustada como equivalente a la medida del diseño. Antes de autorizar la exportación, compara las medidas originales y las exportadas, confirma las tolerancias y coordina cualquier corrección con el responsable técnico. La disponibilidad y el comportamiento exacto de esta opción deben verificarse en la versión instalada.
{% endhint %}

Si tu trabajo requiere incluir otro TXT en la misma exportación, la captura muestra dónde incorporarlo. Concilia ambas producciones antes de continuar:

<figure><img src=".gitbook/assets/image (110).png" alt="Opción de incorporar otro TXT de producción en la exportación"><figcaption><p>Añadir un segundo TXT requiere conciliar ambos orígenes.</p></figcaption></figure>

Una vez verificadas las fuentes, los materiales y las dimensiones, selecciona **Exportar**:

<figure><img src=".gitbook/assets/image (111).png" alt="Acción de exportar la producción a la plantilla de proveedor"><figcaption><p>Exportar el documento no confirma un pedido ni una aprobación de fabricación.</p></figcaption></figure>

Elige una carpeta de destino identificable y guarda la plantilla, sin sobrescribir la fuente aprobada:

<figure><img src=".gitbook/assets/image (112).png" alt="Selección de la carpeta de destino para guardar la plantilla"><figcaption><p>Guarda el resultado en una ubicación identificable y conserva el archivo original.</p></figcaption></figure>

El recorrido muestra un mensaje de confirmación. Después, **abre el XLSX y revisa su contenido**:

<figure><img src=".gitbook/assets/image (113).png" alt="Mensaje de confirmación del proceso de exportación"><figcaption><p>Comprueba el archivo creado aunque el sistema confirme la exportación.</p></figcaption></figure>

El recorrido ilustrado finaliza con una **plantilla XLSX** del proveedor. Antes de entregarla, comprueba que se haya completado correctamente y que el formato siga siendo aceptado por el proveedor; la exportación **no representa un pedido realizado ni una aprobación técnica automática**:

<figure><img src=".gitbook/assets/image (114).png" alt="Ejemplo de plantilla XLSX obtenida para el proveedor"><figcaption><p>Antes de enviarla, revisa contenido, formato y dimensiones con el responsable técnico.</p></figcaption></figure>

### Información comercial y plantillas de proveedores

- Antes de exportar, confirma con el proveedor la **versión vigente de su plantilla**, columnas obligatorias, unidades, formato de entrega y códigos comerciales. No alteres sus encabezados o fórmulas sin una validación técnica.
- Distingue **código interno** de **código comercial**; si cambia espesor, formato, color, fabricante o presentación, vuelve a comprobar la equivalencia. Una referencia histórica puede estar desactualizada.
- Comparte solo los datos necesarios y autorizados. **No incluyas contraseñas, licencias, precios internos no aprobados ni datos personales ajenos al propósito de la solicitud**.
- Conserva la fuente y el Excel exportado con identificación de versión, acceso restringido y canal de entrega autorizado. Exportar un fichero no equivale a autorizar su distribución.

## 4. Comprobación antes de comprar o enviar a corte

- **Procedencia:** confirma cliente, ambiente(s), referencia y archivos seleccionados.
- **Contenido:** coteja materiales, espesores, unidades, cantidades y partidas faltantes con el RP.
- **Consolidación:** si incluiste varios ambientes, revisa las advertencias y la trazabilidad de inclusiones y exclusiones.
- **Proveedor:** comprueba códigos de tablero, formato de plantilla y medidas mínimas; no aceptes ajustes de corte sin revisión técnica.
- **Gestión comercial:** confirma stock real, precios, plazos, impuestos y autorizaciones antes de enviar una orden de compra.

### Conciliar el RP con el RC

La comparación siguiente es un **control manual recomendado**, no un comprobador automático atribuido a Cabinet Report. **No compares directamente las cantidades de piezas del RP con las unidades comerciales del RC** sin justificar la conversión.

| Control | Comparación | Si existe diferencia |
| --- | --- | --- |
| **Origen** | Cliente, ambiente, referencia, versión y archivos seleccionados. | Detén el envío y recupera la fuente correcta. |
| **Tableros** | Material, espesor, veta, formato y piezas del RP frente a la relación de materiales resultante. | Revisa cambios de material, rendimiento, corte y unidad de compra. |
| **Cantos** | Lados canteados del RP, tipo/ancho y longitud frente a las partidas del RC. | Localiza lados omitidos, repetidos o convertidos con otra unidad. |
| **Accesorios y herrajes** | Referencia, montaje/instalación y cantidades en archivos complementarios. | Comprueba multiplicadores, categorías ausentes o partidas duplicadas. |
| **Perfilería** | Perfil, longitud y requisitos del RP frente a tramos o unidades exportados. | Reconcilia medidas, restricciones y órdenes de corte cuando existan. |
| **Varios ambientes** | Fuentes seleccionadas, exclusiones y hoja **Trazabilidad**. | Descarta versiones repetidas y reconstruye el reparto por origen. |
| **Excel** | Pestañas esperadas según opción, filas, unidades, totales y celdas requeridas. | No autorices un archivo vacío, truncado o inconsistente. |

**Registro sugerido:** partida, archivo/ambiente de origen, especificación, unidad original, regla de conversión, cantidad esperada, cantidad exportada, diferencia y aprobación del responsable. Si cambias el RP o una fuente complementaria, conserva la versión anterior, **regenera el RC y repite la conciliación**. Si el consolidado no presenta reparto por ambiente, recupéralo de los archivos originales; no lo estimes.

### Integridad del Excel y diagnóstico de problemas

1. Abre el **XLSX generado en esta ejecución** y comprueba que sea legible, que incluya las hojas y categorías previstas para esa opción y que las filas y los totales no estén vacíos.
2. Verifica **rutas, archivos fuente, cliente, ambiente, permisos de lectura/escritura y carpeta de destino**. Comprueba que no se haya utilizado otra versión del trabajo.
3. Revisa el número de partidas, referencias, unidades y subtotales **por especificación homogénea**. No ocultes una diferencia editando solamente el total del Excel.
4. En una plantilla de corte y canteo, compara las **dimensiones originales y exportadas**, incluidos ajustes por medida mínima, y solicita aprobación técnica antes de enviarla.

| Situación | Qué revisar primero | Decisión segura |
| --- | --- | --- |
| **No aparece el archivo** | Ruta de salida, mensajes visibles, archivos seleccionados y permisos. | Conserva fuentes y error; corrige la causa verificada antes de repetir. |
| **XLSX vacío o incompleto** | Hojas, categorías, fuentes y advertencias. | No utilizar para pedido; reconstruir los datos faltantes. |
| **Totales duplicados o inesperados** | Repetición de ambientes, versiones, referencias y unidades. | Revisar la trazabilidad y conciliar cada partida antes de aprobar. |
| **Plantilla rechazada o medidas alteradas** | Versión de formato, código del proveedor, medida mínima y dimensiones de origen. | Solicitar confirmación comercial y validación técnica. |

Estos son **pasos de diagnóstico sugeridos**, no causas automáticas demostradas por el sistema. Para soporte, conserva el mensaje exacto, versión instalada y una copia protegida de los archivos, sin compartir información sensible.

Para consultar el alcance actualizado de ambas modalidades, visita la [Documentación oficial — Reporte de Compras](https://cabinet-report.gitbook.io/cabinet-report-docs/funcionalidades-de-cabinet-report/reporte-de-compras).


## 5. Ensayo reproducible: del reporte de compras a la recepción de materiales

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

**Ejercicio adicional — duplicidad y referencia desactualizada:** si en un control externo alguien suma dos veces el Ambiente B, el total de bisagras sería **8 + 16 + 16 = 40** en lugar de 24. Revisa las fuentes y la trazabilidad del consolidado, cuando exista; **no supongas que la aplicación detecta o corrige sola esa duplicación**. Si las 16 bisagras del segundo ambiente tienen un código o una versión técnica distinta, registra la referencia por separado hasta confirmar equivalencia. Aplica el mismo criterio a tableros de diferente espesor o a cantos de diferente ancho.


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
