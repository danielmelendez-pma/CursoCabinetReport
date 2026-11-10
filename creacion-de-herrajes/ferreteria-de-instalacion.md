---
description: Crea ferretería de instalación, configura sus propiedades y filtra herrajes por categoría o visibilidad.
---

# Ferretería de Instalación

La sección **Ferretería de Instalación** permite registrar y consultar referencias destinadas a **fijar o instalar los muebles en obra**. Esta lección conserva la secuencia de siete capturas históricas y explica cómo contrastar una referencia desde el catálogo hasta su uso en un módulo, el Reporte de Producción (RP), los archivos auxiliares y su entrega física.

**Antes de comenzar:** comprueba la **sección**, el **cliente activo**, los permisos, la conexión y la versión instalada. Las acciones ilustradas pueden estar limitadas por **perfil, propiedad del registro y contexto de apertura**. Crear una referencia no acredita inventario, compra, asignación a un módulo ni inclusión en el RP.

**Recorrido:** registrar → comprobar propiedades y unidad → filtrar → administrar o asociar → localizar por categoría → conciliar RP, TXT y Compras → verificar recepción en obra. Para la clasificación general, consulta [Creación de Herrajes](README.md) y la [Documentación Oficial de Herrajes](https://github.com/danielmelendez-pma/CabinetReport-Docs/blob/main/funcionalidades-de-cabinet-report/herrajes-en-desarrollo.md).

<figure><img src="../.gitbook/assets/image (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1).png" alt="Vista general del formulario Ferretería de Instalación y su catálogo en Cabinet Report"><figcaption>Vista histórica de instalación: identifica la sección y el listado de referencias antes de registrar o seleccionar un herraje.</figcaption></figure>

## 1. Crear un herraje de instalación

1. Abre **Ferretería de Instalación**; confirma que no estás en **Ferretería de Montaje** ni **Accesorios**.
2. Escribe un **nombre identificable** que distinga la referencia y su presentación cuando sea necesario.
3. Selecciona la **categoría** y el **tipo** correctos para su función técnica. La sección indica el destino de uso; la categoría organiza la búsqueda; el tipo y las propiedades distinguen variantes.
4. Comprueba cliente, permisos y conexión. Si el botón **(+)** está habilitado, púlsalo para intentar agregar la referencia.
5. Verifica el resultado en el **listado o mensaje de la interfaz**. Pulsar (+) no demuestra por sí solo que la operación se haya guardado.

El alta de registros maestros está limitada en modo **sin conexión**, según la documentación oficial. Para un ensayo utiliza una referencia privada autorizada, no una referencia pública compartida.

<figure><img src="../.gitbook/assets/image (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1).png" alt="Campos de nombre categoría y tipo con botón de agregar herraje de instalación"><figcaption>Alta de instalación: identifica nombre, categoría y tipo, utiliza (+) si está autorizado y confirma que el registro aparece.</figcaption></figure>

## 2. Completar y comprobar las propiedades

Selecciona la referencia guardada y revisa los **campos realmente disponibles en tu versión**. Completa las propiedades técnicas pertinentes y comprueba de nuevo el registro antes de utilizarlo.

| Dato a comprobar | Criterio práctico |
| --- | --- |
| **Nombre y categoría** | Deben identificar la pieza y su función de instalación, sin confundirla con una de montaje. |
| **Tipo y propiedades** | Deben corresponder con la fijación y con la especificación técnica del mueble u obra. |
| **Unidad o presentación** | Distingue piezas individuales, cajas o paquetes, si esa información está disponible; no supongas equivalencia entre presentaciones. |
| **Cantidad prevista** | Se define por módulo o trabajo y debe verificarse después en la producción; no equivale al contenido de un paquete. |
| **Precio** | Cuando se utilice en [Costos](../costos.md), verifica moneda, vigencia, unidad de compra y fuente del importe antes de valorar. |

Un precio registrado no garantiza que sea el precio actual del proveedor ni que se haya aplicado al presupuesto. Si la compra es por caja y el uso por unidad, confirma la cantidad por caja antes de convertirla; **Cabinet Report no se declara aquí responsable de esa conversión**.

<figure><img src="../.gitbook/assets/image (2) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1).png" alt="Área de edición de propiedades y precio de la ferretería de instalación seleccionada"><figcaption>Propiedades: revisa los datos efectivamente guardados y verifica unidad, presentación y precio cuando correspondan.</figcaption></figure>

## 3. Consultar referencias públicas y privadas

Utiliza **PÚBLICO** y **PRIVADO** para filtrar el catálogo según las referencias visibles para el usuario y el cliente activo.

| Filtro | Qué permite consultar | Control antes de actuar |
| --- | --- | --- |
| **PÚBLICO** | Referencias generales o compartidas visibles para el acceso actual. | Verlas no otorga permiso para editarlas o eliminarlas. |
| **PRIVADO** | Referencias vinculadas al cliente propietario. | Comprueba el cliente correcto y el permiso para modificar o incorporar elementos. |

**Filtrar no cambia la titularidad, no crea una copia privada y no agrega líneas al TXT.** Si una referencia no aparece, revisa sección, categoría, filtros, cliente, permisos y conexión antes de crear otra. Una lista vacía en modo sin conexión no demuestra que el registro no exista en el catálogo remoto.

<figure><img src="../.gitbook/assets/image (20).png" alt="Filtros Público y Privado del catálogo de Ferretería de Instalación"><figcaption>Filtros de visibilidad: consulta referencias públicas o privadas sin alterar su propiedad ni su asociación a módulos.</figcaption></figure>

## 4. Administrar o aplicar la referencia seleccionada

La ventana histórica muestra controles cuyo alcance cambia según **desde dónde se abrió**, la versión, la conexión y las autorizaciones:

| Acción | Comprobación y límite |
| --- | --- |
| **Agregar al catálogo privado** | Si el control está disponible y autorizado, verifica qué referencia y **cliente propietario** recibe el registro. No equivale a activar PRIVADO ni a agregar al TXT. |
| **Eliminar** | Confirma titularidad y permiso antes de borrar. Nunca uses un registro público o compartido para una prueba de eliminación. |
| **Actualizar el herraje del módulo seleccionado** | Si abriste la ventana desde [Creación de Módulos](../creacion-de-modulos.md) o [Catálogo de Módulos](../catalogo-de-modulos.md), confirma módulo, referencia, categoría y cantidad; comprueba el resultado al volver a abrir el módulo. |
| **Incorporar al TXT de producción** | Es una operación **distinta** de administrar el catálogo y solo debe darse por efectiva si el contexto del [RP](../reporte-de-produccion/reporte-de-produccion.md) está activo y la línea aparece en el auxiliar correspondiente. |

Abrir esta pantalla desde un módulo o desde producción **no concede permisos administrativos adicionales**. Editar una referencia maestra tampoco demuestra que módulos o RP anteriores se hayan actualizado automáticamente.

<figure><img src="../.gitbook/assets/image (21).png" alt="Controles de administración y aplicación del herraje de instalación seleccionado"><figcaption>Administración de la referencia: comprueba permisos, titularidad y contexto antes de agregar, eliminar o actualizar un módulo.</figcaption></figure>

## 5. Localizar herrajes por categoría: Tornillos

Pulsa la **imagen de una categoría** para filtrar sus referencias. En el ejemplo histórico, al seleccionar **Tornillos** se muestran los elementos registrados bajo esa categoría.

1. Selecciona **Tornillos** y confirma que sigues dentro de **Ferretería de Instalación**.
2. Identifica la **referencia y el tipo** de tornillo; contrasta sus propiedades con la fijación requerida.
3. Comprueba **unidad, presentación y cantidad** antes de escogerlo para un módulo o una producción.
4. Si asocias la referencia a un módulo, verifica después que esa asociación se guardó; **filtrar por Tornillos no asigna automáticamente el herraje**.

<figure><img src="../.gitbook/assets/image (5) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1).png" alt="Imagen de la categoría Tornillos utilizada como filtro de la ferretería de instalación" width="171"><figcaption>Categoría Tornillos: pulsa su imagen para consultar referencias registradas bajo esa clasificación.</figcaption></figure>

<figure><img src="../.gitbook/assets/image (3) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1).png" alt="Listado de herrajes de instalación filtrado por la categoría Tornillos"><figcaption>Resultado del filtro Tornillos: comprueba nombre, tipo y propiedades de la referencia antes de asociarla o planificar su uso.</figcaption></figure>

{% hint style="info" %}
**Control técnico:** el nombre comercial no basta para determinar compatibilidad con sustrato, longitud de fijación o condiciones de obra. Confirma la especificación del diseño y la recomendación del fabricante; las capturas no acreditan un cálculo automático de tornillos necesarios.
{% endhint %}

## 6. Diferenciar instalación, montaje y accesorios

| Sección | Uso principal | Lección relacionada |
| --- | --- | --- |
| **Ferretería de Instalación** | Elementos para fijar o instalar el mueble **en obra**. | Esta lección. |
| **Ferretería de Montaje** | Elementos utilizados para **armar muebles en fábrica**. | [Ferretería de Montaje](ferreteria-de-montaje.md). |
| **Accesorios** | Complementos de funcionamiento, uso o mecanismos del mueble. | [Accesorios](accesorios.md). |

Una misma denominación comercial no justifica mezclar categorías: clasifica la referencia según el **uso técnico real** y comprueba dónde se consumirá. Los **Rieles** ilustrados en montaje y los **Tornillos** de esta lección son ejemplos de filtros, no reglas universales de fabricación.

## 7. Del catálogo al módulo, RP y entrega documental

| Etapa | Qué puedes comprobar | Qué **no** demuestra |
| --- | --- | --- |
| **Catálogo de instalación** | Referencia, sección, categoría, tipo, propiedades, procedencia y unidad. | Stock físico, compra o asociación al proyecto. |
| **Creación / Catálogo de Módulos** | Asociación y cantidad previstas, si la función está habilitada y se guardó. | Cambio automático de módulos previamente almacenados. |
| **Reporte de Producción** | Cliente, ambiente, módulos y ferretería realmente incorporada a la producción. | Que el alta de catálogo inserte una partida por sí misma. |
| **TXT de Ferretería de Instalación** | Referencias y cantidades del archivo auxiliar **cuando se genere**. | Que todas las producciones lo generen o que haya disponibilidad física. |
| **Reporte de Compras** | Partidas de instalación seleccionadas entre las fuentes del proyecto y su Excel resultante. | Compra, llegada a almacén o reserva efectiva. |
| **Orden de Entrega de Herrajes** | Documento de preparación o entrega, **si existe**, y partidas destinadas al trabajo. | Firma, recepción o instalación física registrada automáticamente. |

Consulta los [Archivos de Reportes Generados](../reporte-de-produccion/archivos-de-reportes-generados.md) para identificar el **TXT de Ferretería de Instalación** y las **Órdenes de Entregas de Herrajes**. El [Reporte de Compras](../reporte-de-compras.md) contempla la selección de archivos de materiales, instalación, montaje y accesorios; confirma que todos provengan del mismo proyecto. La [Orden de Producción](../orden-de-produccion.md) es **otro documento**, que agrupa reportes RP para organizar fabricación: **no equivale** a una orden de entrega ni a un comprobante de recepción en obra.

**Distingue siempre:** **Agregar al catálogo** almacena una referencia para uso posterior; **agregar al TXT** trabaja con una producción activa; **preparar una entrega** y **recibirla físicamente** son controles operativos diferentes. No presupongas propagación automática entre esas etapas.

## 8. Ensayo de trazabilidad: de la ferretería de instalación a la obra

Este ejercicio propone una **comprobación reproducible**, sin afectar una producción real. Sigue una referencia desde el catálogo hasta su preparación por almacén y la recepción por instalación. **No es una prueba funcional ejecutada** ni presupone que Cabinet Report descuente existencias, genere pedidos o registre entregas físicas automáticamente.

### Preparar el caso de prueba

1. Utiliza un **cliente, ambiente y módulo de ensayo** identificables; conserva copia de los datos y archivos iniciales. No borres ni modifiques un registro público o compartido para realizar la prueba.
2. Elige una referencia permitida de **Ferretería de Instalación** o, si tu acceso lo permite, crea una referencia privada de ensayo. Comprueba **nombre, categoría, tipo, unidad, propiedades, visibilidad y cliente propietario**. Un filtro **PÚBLICO/PRIVADO** no equivale a cambiar la titularidad.
3. Anota la necesidad prevista en unidades reales para ese ambiente, definida por el responsable técnico. **Ejemplo exclusivamente didáctico:** se requieren **8 unidades** de una referencia ficticia `FI-ENSAYO-01`. El código y el total no son nombres, parámetros ni cálculos propios de Cabinet Report.
4. Documenta la versión del programa, el módulo o trabajo de origen y los archivos que esperas obtener. Verifica la disponibilidad de cada operación en tu instalación.

### Comprobar el recorrido

| Punto de control | Evidencia que debes contrastar | Qué no demuestra por sí solo |
| --- | --- | --- |
| **Catálogo** | Referencia, categoría **Instalación**, unidad, visibilidad y propietario correcto. | Que la referencia ya esté asignada a un módulo o producción. |
| **Módulo** | Asociación y cantidad previstas en el [Creador de Módulos](../creacion-de-modulos.md) o [Catálogo](../catalogo-de-modulos.md), si el caso utiliza esa relación. | Que editar el catálogo actualice módulos existentes. |
| **Reporte de Producción** | Cliente, ambiente, módulo y cantidades de ferretería efectivamente incorporadas al [RP](../reporte-de-produccion/reporte-de-produccion.md). | Que la referencia se haya agregado al TXT solo por figurar en el catálogo. |
| **TXT auxiliar** | Cuando se genere el **TXT de Ferretería de Instalación**, abrirlo y cotejar descripción, unidad y cantidad con la producción aprobada. | Que todos los complementarios se generen en todos los trabajos. |
| **Compras** | Si corresponde, abrir el [Reporte de Compras](../reporte-de-compras.md) y comparar la partida y sus unidades con la fuente seleccionada. | Que exista stock, se haya comprado o recibido la ferretería. |
| **Almacén e instalación** | Si se genera una **Orden de Entrega de Herrajes**, cotejarla con la preparación física y registrar responsable, fecha, cantidad entregada y recepción. | Que el software haya verificado o registrado la entrega física. |

Consulta las capturas de los [Archivos de Reportes Generados](../reporte-de-produccion/archivos-de-reportes-generados.md) para distinguir el TXT de instalación, las órdenes de entrega y otros archivos. **Agregar al catálogo** y **agregar al TXT de una producción** son acciones distintas; verifica qué acción estás realizando según el contexto disponible.

### Ensayo de discrepancia y criterio de entrega

En el ejemplo didáctico, el responsable del trabajo ha previsto **8 unidades**, pero almacén solo prepara **6**. La diferencia de **2 unidades** es un control **manual** entre lo requerido y lo físicamente disponible; no se afirma que Cabinet Report la calcule, advierta o bloquee.

1. Comprueba primero si la diferencia nace en la asociación al módulo, el RP, el TXT auxiliar, el Reporte de Compras o la preparación de almacén. Anota el **archivo y la línea o partida concreta** donde aparece.
2. Si el TXT o el Excel muestran otra unidad de presentación (por ejemplo, un paquete frente a una unidad), **no compares los números directamente**: confirma contenido por paquete y equivalencias con el proveedor, sin inventar conversiones.
3. **No declares completa ni entregues como completa** la dotación del ejemplo mientras falten las dos unidades. Registra la incidencia, resuelve el faltante con el responsable y vuelve a conciliar la cantidad preparada.
4. Tras la entrega física, pide al receptor que confirme manualmente **referencia, cantidad realmente recibida, ambiente, fecha y observaciones**. Una firma o comprobante de obra forma parte del procedimiento de la empresa, no de una función automática acreditada de Cabinet Report.

{% hint style="warning" %}
**Criterio de aceptación:** la clasificación debe ser **Ferretería de Instalación**, y la referencia, unidad y cantidad deben concordar entre las fuentes realmente utilizadas. Si hay un archivo ausente que era necesario, una discrepancia sin explicación, un cliente o ambiente equivocado, o una dotación física incompleta, **detén la liberación a instalación** hasta resolverla. Conserva los originales y registra el resultado del ensayo; no edites directamente los TXT/XML para ocultar diferencias.
{% endhint %}

### Recepción, faltantes y liberación en obra

El control físico siguiente es un **procedimiento manual sugerido para la empresa**; las capturas del curso no demuestran que Cabinet Report administre existencias, reservas, entregas parciales, firmas, recepción o bloqueos automáticos.

1. **Preparación en almacén:** contrasta la orden de entrega, si se emitió, con el TXT auxiliar y las unidades reales. Cuenta las piezas, separa las referencias dañadas o incompatibles y deja asentados los faltantes.
2. **Incidencia y reposición:** registra la cantidad faltante, su causa, responsable y la acción acordada. Si compras debe reponer material, coteja la solicitud con el Reporte de Compras, pero no registres una recepción aún no realizada.
3. **Salida autorizada:** quien corresponda en la empresa confirma por escrito la cantidad **efectivamente liberada** y el trabajo de destino. Si se permite una entrega parcial, documéntala expresamente como parcial; no la presentes como dotación completa.
4. **Recepción en obra:** el instalador verifica referencia, unidad, cantidad, estado y destino; registra manualmente diferencias, fecha, responsable y evidencia de recepción.
5. **Cierre:** libera el kit como **completo** únicamente cuando las cantidades previstas y las recibidas estén conciliadas o cuando se haya aprobado y documentado una modificación de alcance.

Si los datos documentales difieren de lo recibido, conserva la incidencia abierta en el control de la empresa y revisa la fuente correcta. **No edites retroactivamente el TXT de producción para simular una entrega que no ocurrió.**

### Registro mínimo de evidencia

| Dato | Qué registrar |
| --- | --- |
| **Origen** | Cliente de prueba, ambiente, módulo (si aplica), versión y referencia de ferretería. |
| **Comparación** | Cantidad prevista, unidad, cantidad en RP/TXT y cantidad en Compras, cuando existan. |
| **Salida física** | Cantidad preparada, entregada y recibida; responsable y fecha registrados por la empresa. |
| **Resultado** | Coincide / difiere / no aplica, causa identificada y archivo o comprobante que respalda la conclusión. |

El recorrido **no supone propagación automática**, ni valida el comportamiento de una versión sin ejecutar la prueba en Windows. Si se modifica un módulo o el catálogo, vuelve a revisar las asociaciones y el RP existente antes de emitir nuevos archivos.

---

[← Ferretería de Montaje](ferreteria-de-montaje.md) · [Creación de Herrajes](README.md) · [Catálogo de Módulos](../catalogo-de-modulos.md) · [🏠 Portal principal](https://danielmelendez-pma.github.io/cabinet-report-partners/)
