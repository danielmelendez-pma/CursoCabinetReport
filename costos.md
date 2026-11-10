---
description: >-
  Lección práctica de Costos: importar materiales, comprobar precios, distinguir
  cliente y proyecto, administrar márgenes y revisar cotizaciones antes de exportarlas.
---

# Costos

El módulo **Costos** permite organizar la materia prima, los importes y las condiciones comerciales de un proyecto por ambientes, para preparar **cuadros de costos y cotizaciones**. Esta lección parte de los controles y capturas históricos del Curso y los relaciona con el [Reporte de Compras](reporte-de-compras.md) y la [documentación oficial de Costos](https://cabinet-report.gitbook.io/cabinet-report-docs/funcionalidades-de-cabinet-report/costos-en-desarrollo).

<figure><img src=".gitbook/assets/image (123).png" alt="Vista original del módulo Costos de Cabinet Report"><figcaption><p>Vista general de Costos: comprueba el proyecto y el ambiente antes de valorar materiales.</p></figcaption></figure>

{% hint style="info" %}
**Alcance de la lección:** Costos es una funcionalidad existente, no una función en desarrollo. Los nombres y controles ilustrados pueden variar según la versión instalada y los permisos. Las reglas históricas sobre archivos y ambientes son referencias para verificar en el programa; no constituyen pruebas funcionales de la versión actual.
{% endhint %}

## Ruta de aprendizaje

**Del RP a la cotización:** comienza con el [Reporte de Producción revisado](reporte-de-produccion/README.md), continúa con el [Reporte de Compras](reporte-de-compras.md) y concilia aquí las partidas de cada ambiente antes de exportar. Si detectas una discrepancia de funcionamiento, consulta [Reporte de Errores o Feedback](reporte-de-errores-o-feedback.md).

Esta lección incluye un **ensayo de trazabilidad** para practicar el control sin cambiar datos comerciales reales. Las capturas son referencias de la interfaz; comprueba qué opciones ofrece tu instalación.

## Antes de comenzar

1. Prepara el [Reporte de Producción](reporte-de-produccion/README.md) y el [Reporte de Compras](reporte-de-compras.md) que correspondan al trabajo. Confirma **cliente, proyecto, ambiente, materiales, cantidades y unidades**.
2. Ubica el **Excel XLSX de compras** o, si continúas un presupuesto anterior, su **XML de Costos**. Conserva una copia del archivo original antes de cargar o reemplazar datos.
3. Reúne precios comprobables del proveedor, unidades de compra y condiciones comerciales. No consideres vigente un precio solo porque figure en el catálogo.
4. Define qué ambientes incluirá el presupuesto y cuáles partidas son compartidas, para evitar omisiones o dobles conteos.

**Distingue tres conceptos:** el *cliente activo* identifica la instalación y sirve de referencia para los catálogos privados; el *proyecto* identifica el trabajo que se está cotizando; y cada *ambiente* agrupa las partidas que corresponden a un espacio del proyecto. La [especificación técnica histórica](https://github.com/danielmelendez-pma/DocumetacionTecnicaCabinetReport/blob/main/modulo-costos.md) indica que un nombre de cliente leído de Excel, XML o PDF no debe sustituir al cliente activo. Comprueba esta separación al importar.

## 1. Conocer el menú Opciones

<figure><img src=".gitbook/assets/image (126).png" alt="Menú Opciones de Costos en la interfaz documentada"><figcaption><p>Desde Opciones se seleccionan los archivos de entrada y se revisan las configuraciones disponibles.</p></figcaption></figure>

El menú documentado reúne estas acciones:

| Opción | Para qué se utiliza | Qué debes verificar |
| --- | --- | --- |
| **Cargar reportes de compra XLSX** | Incorporar materiales desde los Excel generados en Reporte de Compras. | Proyecto, ambiente, descripciones, cantidades y unidades del archivo elegido. |
| **Cargar archivos de Costos XML** | Recuperar un presupuesto previamente trabajado en Costos. | Que corresponda al proyecto esperado y que no sustituya datos de otro ambiente. |
| **Agregar archivo Promob PDF** | Procesar un PDF de materiales procedente de Promob, cuando su formato sea compatible. | Importación real de partidas; no se garantiza compatibilidad con todos los PDF. |
| **Cargar Precios Unitarios** | Buscar coincidencias de materia prima en los catálogos registrados. | Unidad, identificación y costo resultantes, además de las coincidencias no encontradas. |
| **Márgenes** y **Notas Globales** | Guardar o limpiar configuraciones reutilizables. | Diferenciar ajustes del cliente de referencias particulares de cada proyecto. |
| **Limpiar** | Reiniciar el formulario según el recorrido histórico. | Respaldar cualquier trabajo que aún no se haya guardado. |

{% hint style="warning" %}
**Importar no equivale a validar.** Un XLSX, XML o PDF puede contener materiales o importes desactualizados, cantidades duplicadas y referencias de otro proyecto. Contrasta siempre la tabla que aparece después de la carga.
{% endhint %}

## 2. Cargar y comprobar la materia prima

1. En **Opciones**, elige la carga compatible con el archivo que preparaste.
2. Después de importar, revisa el listado de **Materia Prima**: **DESCRIPCION, UND, ID, TIPO y COST-UNIT**, además de las cantidades e importes que muestre tu versión.
3. Compara las descripciones y unidades con el [Reporte de Compras](reporte-de-compras.md). Si hay tableros, cantos o herrajes con nombres parecidos, no los declares equivalentes sin comprobar la referencia.
4. Comprueba el ambiente al que se asignaron las partidas y evita cargar dos veces la misma fuente.
5. Antes de avanzar, identifica los renglones sin precio, con cantidad inesperada o con unidad incompatible con la compra real.

### Catálogos públicos y privados

<figure><img src=".gitbook/assets/image.png" alt="Filtros de materia prima pública y privada en Costos"><figcaption><p>Los filtros Pública y Privada ayudan a distinguir la procedencia de las referencias y sus costos.</p></figcaption></figure>

La interfaz histórica incluye filtros **Pública** y **Privada** para las referencias de tableros y herrajes. La documentación del Curso indica que pueden estar ambos activos, pero no los dos desactivados; filtrar las listas de selección no debería reemplazar por sí solo las partidas ya cargadas.

- **Pública:** referencias generales visibles según los permisos y el catálogo.
- **Privada:** referencias asociadas al cliente activo, no a un supuesto cliente leído del archivo importado.
- **Ambas:** revisar de cuál catálogo procede la referencia seleccionada y cuál precio se está utilizando.

Si una referencia no aparece, comprueba permisos, visibilidad, cliente activo y descripción antes de crear o elegir otra. Consulta [Creación de Tableros](creacion-de-tableros.md) y [Creación de Herrajes](creacion-de-herrajes/README.md).

### Buscar precios unitarios

La descripción histórica de **Cargar Precios Unitarios** especifica una búsqueda por coincidencia de texto entre la columna **DESCRIPCION** de Materia Prima y los registros de las tablas de herrajes (`TblAccHerrajes`) y tableros (`TblAglomerados`).

| Origen histórico | Campos consultados | Resultado esperado en la tabla |
| --- | --- | --- |
| **Herrajes**: descripción coincidente | `IdAccesorio`, `Tipo`, `Costo`, `Unidad` | Completar **ID**, **TIPO**, **COST-UNIT** y **UND**. |
| **Tableros**: nombre de aglomerado coincidente | `IdAglomerado`, `PrecioProveedor` | Completar **ID** y **COST-UNIT**; tipo **Tablero** y unidad **UND** según el ejemplo original. |

{% hint style="warning" %}
**Coincidencia no es equivalencia técnica ni precio confirmado.** El texto original describe comparación de descripciones tal como están escritas, sin normalización del texto. Si no hay coincidencia, si existen nombres similares o si el costo parece incorrecto, revisa manualmente la referencia, su unidad, proveedor, moneda, impuestos y vigencia. No inventes un costo para completar la tabla.
{% endhint %}

### Agregar o revisar una partida manualmente

<figure><img src=".gitbook/assets/image (1).png" alt="Listado de Materia Prima con campos para selección o entrada manual"><figcaption><p>La tabla de Materia Prima permite cotejar la descripción, la unidad y los costos con la fuente.</p></figcaption></figure>

La lección original permite **seleccionar una descripción del listado o escribir una nueva**. Cuando una referencia coincide con el catálogo, la interfaz documentada puede completar **UND, ID, TIPO y COST-UNIT**. Para una partida escrita manualmente, verifica esos campos por separado: el texto ingresado no demuestra que exista un registro ni que tenga precio.

## 3. Administrar márgenes y notas

### Márgenes de producción y operación

<figure><img src=".gitbook/assets/image (127).png" alt="Opciones históricas para guardar o limpiar márgenes"><figcaption><p>Antes de guardar o limpiar márgenes, comprueba la configuración que corresponde al trabajo.</p></figcaption></figure>

El recorrido documentado distingue **margen de producción** y **margen operativo**. La acción **Guardar Márgenes** utiliza los archivos `MargenProduccion.xml` y `MargenOperativo.xml` en la carpeta `ArchivosCliente` de la instalación. La acción **Limpiar Márgenes**, según esa documentación, elimina los archivos almacenados.

**Antes de limpiar:** conserva un respaldo de esos XML si necesitas recuperar la configuración. Después de guardar o cargar, comprueba en pantalla que las condiciones realmente corresponden a la cotización actual.

### Notas globales y notas del proyecto

<figure><img src=".gitbook/assets/image (128).png" alt="Opciones documentadas para guardar o limpiar Notas Globales"><figcaption><p>Las Notas Globales reúnen condiciones reutilizables; la referencia debe corresponder al proyecto actual.</p></figcaption></figure>

Las **Notas Globales** recogen condiciones reutilizables del cliente, como forma de pago, suministro, instalación, exclusiones y observaciones. La acción **Guardar Notas Globales** utiliza `ArchivosCliente/NotasGlobales.xml`; **Limpiar Notas Globales** se describe históricamente como eliminación de ese archivo.

La **referencia del proyecto**, en cambio, pertenece al presupuesto de ese proyecto. La especificación técnica histórica la sitúa en su propio XML y no en `NotasGlobales.xml`. Evita arrastrar la referencia de un cliente o proyecto anterior al cotizar un trabajo nuevo.

{% hint style="info" %}
**Diferencia entre limpiar acciones:** **Limpiar** el formulario, **Limpiar Márgenes** y **Limpiar Notas Globales** se describen como operaciones distintas. Antes de ejecutar una de ellas, verifica el alcance en tu versión y conserva copia de los archivos que deseas recuperar.
{% endhint %}

## 4. Organizar los ambientes

La [especificación técnica del módulo Costos](https://github.com/danielmelendez-pma/DocumetacionTecnicaCabinetReport/blob/main/modulo-costos.md) describe cada ambiente como una unidad con lista de materiales, cantidades y costos propios. No se debe dar por hecho que ese comportamiento histórico haya sido validado en todas las versiones.

Para una cotización con varios ambientes:

1. Identifica cada ambiente del proyecto y comprueba que su listado contiene únicamente las partidas correspondientes.
2. Al cambiar de ambiente, revisa qué partidas se muestran; no presupongas que un elemento visible en un ambiente pertenece a todos.
3. Si importas varios archivos, comprueba que no se repitan materiales ni se sobrescriban las referencias o cantidades de otro ambiente.
4. Revisa por separado el resumen global del proyecto y los subtotales por ambiente antes de presentar una cifra consolidada.

## 5. Comprobar importes y preparar la cotización

La [documentación oficial de Costos](https://cabinet-report.gitbook.io/cabinet-report-docs/funcionalidades-de-cabinet-report/costos-en-desarrollo) describe materia prima, márgenes de producción y operación, precio de venta, ITBMS, resumen de ambientes, notas y condiciones.

1. Revisa **cantidad, unidad y costo unitario** de cada partida; un valor en una unidad distinta puede alterar todo el presupuesto.
2. Contrasta los importes de **materia prima**, **márgenes** y **precio de venta**, sin tratar sus conceptos como intercambiables.
3. Comprueba el **ITBMS** aplicable y las condiciones reales de la operación; no presupongas una tasa universal.
4. Verifica que las notas, exclusiones, forma de pago y referencia correspondan al proyecto actual.
5. Comprueba si las partidas comunes se han incluido una sola vez y si existen materiales o herrajes sin costear.

### Guardar y exportar

La documentación oficial indica que Costos contempla **Exportar costos** y salidas a **Excel (.xlsx)**, además de cotización en **Word (.docx) tipo carta** o **Excel (.xlsx) tipo tabla**. Para esas dos presentaciones de cotización, se requiere primero disponer de un **Excel de costos exportado**.

Después de exportar, abre el documento generado y contrasta proyecto, ambientes, partidas, márgenes, impuestos y total con la vista revisada en Costos. Conserva el XML de Costos y el Excel fuente cuando corresponda para facilitar la recuperación.

{% hint style="warning" %}
**El archivo exportado no certifica que el presupuesto sea correcto ni que haya sido aceptado.** Valida la cotización con los precios actuales y las condiciones comerciales antes de entregarla al cliente. Tampoco confundas esta cotización con la estimación económica de hallazgos del Revisor IA, que tiene otra finalidad.
{% endhint %}

## 6. Si algo no coincide

| Situación | Comprobación recomendada |
| --- | --- |
| **No se cargó una partida** | Verifica formato de origen, contenido del archivo y ambiente seleccionado. |
| **No aparece un precio unitario** | Comprueba descripción, catálogo público/privado, cliente activo y vigencia del precio; registra el faltante sin inventar el importe. |
| **El total cambió al importar otro ambiente** | Revisa duplicados, unidades y asignación de materiales por ambiente. |
| **Aparecen notas o márgenes anteriores** | Identifica los archivos globales de `ArchivosCliente` y diferencia sus datos de los propios del proyecto. |
| **No se genera la cotización** | Comprueba que exista el Excel de Costos exportado requerido y revisa los mensajes de la aplicación. |

## 7. Ensayo reproducible: de Compras a cotización

Este ejercicio conecta la [conciliación del Reporte de Compras](reporte-de-compras.md) con la valoración en **Costos**. Es una **prueba documental y manual**, no una función nueva de Cabinet Report ni un resultado verificado en Windows. Usa archivos compatibles con tu versión y un proyecto de prueba que puedas descartar.

{% hint style="warning" %}
**Protege los presupuestos reales:** conserva copias de los RP, Excel de Compras, XML de Costos y archivos de configuración global. No cambies precios, márgenes ni datos de producción vigentes para completar este ejercicio.
{% endhint %}

### A. Preparar dos ambientes con fuentes identificables

Parte de dos RP previamente revisados del mismo proyecto de práctica, por ejemplo **COCINA-ENSAYO** y **CLÓSET-ENSAYO**, y sus Excel de Compras. Los siguientes números son **datos didácticos ficticios**: no representan una salida del software, un despiece estándar ni cantidades reales.

| Partida con una misma especificación | Unidad | Cocina | Clóset | Total esperado |
| --- | --- | ---: | ---: | ---: |
| Tablero de melamina, mismo espesor y formato | hojas | 3 | 2 | **5** |
| Canto, misma referencia y ancho | metros | 20 | 20 | **40** |
| Bisagra, mismo modelo y referencia | unidades | 8 | 16 | **24** |

1. Anota el **cliente activo de la instalación**, el **nombre del proyecto**, el **ambiente**, el número o referencia del RP y la versión de cada archivo. El cliente activo no debe confundirse con el nombre del proyecto importado.
2. Para cada partida, registra su **descripción técnica, unidad y cantidad** según el RP y el Excel de Compras correspondiente. No asignes un total consolidado a un ambiente por suposición.
3. Si una fuente usa cajas y la otra unidades individuales, consigue la equivalencia de presentación documentada por el proveedor antes de sumar. **Hojas, metros y unidades no se suman entre sí.**

### B. Cargar y revisar el aislamiento de los ambientes

1. En una instalación de prueba autorizada, utiliza la opción documentada **Cargar reportes de compra XLSX** con archivos compatibles. Comprueba la identificación y las partidas que efectivamente se importaron; no presupongas que la aplicación detecta duplicados.
2. Selecciona **COCINA-ENSAYO**, registra sus partidas visibles y repite en **CLÓSET-ENSAYO**. Vuelve a Cocina y contrasta cada ambiente con su origen. Si tu versión no dispone de este recorrido, consigna el paso como **NO EJECUTADO**.
3. Comprueba **DESCRIPCION, UND, ID, TIPO, COST-UNIT**, cantidades y cualquier importe mostrado. Revisa también la **procedencia pública o privada** de las referencias seleccionadas.
4. Distingue **Notas Globales**, márgenes reutilizables y **referencia propia del proyecto**. La presencia de configuraciones históricas no demuestra que sean apropiadas para esta cotización.

### C. Encontrar errores antes de valorar

Reproduce las siguientes discrepancias **solo en una hoja de control externa**; no alteres los archivos de producción.

| Error didáctico | Cálculo que revela la discrepancia | Qué hacer |
| --- | --- | --- |
| Contar dos veces el tablero de Cocina | **3 + 3 + 2 = 8 hojas**, frente a las **5** de origen | Identificar y excluir la fuente duplicada; volver a cotejar el resultado. |
| Interpretar las 16 bisagras de Clóset como 16 cajas de 10 | **160 unidades** supuestas en vez de **16 unidades** verificadas | Comprobar la unidad de la fuente; «caja de 10» es solo una hipótesis del ejercicio. |
| Confundir dos referencias de canto por tener nombres similares | Un total de **40 metros** no demuestra que el ancho y el acabado coincidan | Separar por referencia técnica antes de sumar y valorar. |

**Criterio:** el total correcto del ejemplo contiene **5 hojas**, **40 metros** y **24 bisagras**, en partidas diferentes y con las especificaciones indicadas. El conteo de filas de un archivo no sustituye las cantidades efectivas; una coincidencia de nombres tampoco acredita equivalencia técnica.

### D. Verificar la valoración, sin inventar precios

Por cada partida, conserva una evidencia externa con estos datos:

| Campo de control | Evidencia mínima |
| --- | --- |
| Origen | Cliente activo, proyecto, ambiente, RP y Excel de Compras utilizados |
| Material | Descripción, referencia, especificación, cantidad y unidad |
| Precio | Proveedor, presentación, moneda, costo unitario, fecha de verificación y unidad de cotización |
| Condiciones | Márgenes aplicables, tratamiento de ITBMS, notas, exclusiones y responsable |
| Entregable | XML de Costos cuando corresponda, Excel de Costos y cotización exportada, con identificación de versión |

Para revisar manualmente una partida, compara **cantidad homogénea × costo unitario verificado para esa misma unidad**. Esta comprobación **no describe ni modifica la fórmula interna** de Costos. Si falta un costo unitario confiable, marca la partida **PENDIENTE DE VALORACIÓN** y **no la reemplaces por cero** ni presentes el total como cotización definitiva.

No se fija aquí ningún precio, margen, tasa de ITBMS o fórmula comercial: comprueba los valores y condiciones **aplicables a la operación real**. El impacto económico mostrado por el Revisor IA pertenece a otro proceso y no sustituye la cotización comercial.

### E. Exportar, conciliar y documentar el resultado

1. Con los datos ya revisados, utiliza solo las salidas disponibles en tu versión. Para crear una cotización Word o Excel, la documentación oficial indica que antes debe existir un **Excel de Costos exportado**.
2. Abre el Excel de Costos y la cotización, si existe, y coteja **proyecto, ambientes, partidas, cantidades, unidades, costos, márgenes, impuestos y notas** contra las fuentes y el control manual. Exportar un archivo no significa que haya sido aprobado.
3. Para cada prueba, registra **CONFORME** si se comprobó, **NO CONFORME** si persisten diferencias o **NO EJECUTADO** si faltó la opción, evidencia o ejecución. El trabajo no debe autorizarse para entregar una oferta si quedan partidas duplicadas, unidades incompatibles o precios sin verificar.
4. Si observas un comportamiento del programa que no logras explicar, reúne evidencias sin información sensible y usa la lección [Reporte de Errores o Feedback](reporte-de-errores-o-feedback.md). Los desacuerdos comerciales se resuelven con el responsable del presupuesto y los proveedores.

**Resultado comprobable:** otra persona puede seguir una partida desde el RP al Excel de Compras, identificarla en el ambiente correcto de Costos y localizar el archivo exportado, sin confundir comprobación manual con una función automática.

## 8. Lista de comprobación antes de entregar

- [ ] Cliente activo, proyecto y ambientes identificados sin confusión.
- [ ] Archivos importados correspondientes al trabajo y respaldados.
- [ ] Materiales, herrajes, cantidades y unidades cotejados con el Reporte de Compras.
- [ ] Precios unitarios comprobados y faltantes resueltos o expresamente señalados.
- [ ] Márgenes, ITBMS, notas y exclusiones revisados.
- [ ] Ambientes y partidas compartidas revisados para evitar duplicaciones.
- [ ] Excel de Costos y cotización final abiertos y comprobados antes de compartir.

**Consulta relacionada:** [Reporte de Compras](reporte-de-compras.md) · [Tableros](creacion-de-tableros.md) · [Herrajes](creacion-de-herrajes/README.md) · [Documentación oficial — Costos](https://cabinet-report.gitbook.io/cabinet-report-docs/funcionalidades-de-cabinet-report/costos-en-desarrollo) · [Especificación técnica histórica](https://github.com/danielmelendez-pma/DocumetacionTecnicaCabinetReport/blob/main/modulo-costos.md)

---

[← Optimizadores](optimizadores.md) · [Reporte de Errores o Feedback →](reporte-de-errores-o-feedback.md) · [Portada del Curso](README.md) · [🏠 Portal principal](https://danielmelendez-pma.github.io/cabinet-report-partners/)
