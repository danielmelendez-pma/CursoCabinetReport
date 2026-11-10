---
description: Aprende a crear accesorios, configurar sus propiedades y gestionar su visibilidad en el catálogo de Cabinet Report.
---

# Accesorios

La sección **Accesorios** reúne referencias complementarias utilizadas por los muebles o sus mecanismos. El recorrido documentado permite identificar un accesorio, registrarlo, completar sus propiedades y consultar los controles disponibles para administrarlo o vincularlo con un módulo.

**Antes de comenzar:** identifica el cliente activo, la categoría correcta y el perfil con el que accedes. Las funciones de alta, edición y eliminación pueden depender de **permisos, titularidad, versión y conexión**. Un accesorio visible en un catálogo **no acredita inventario físico**, asociación con un módulo ni inclusión en un Reporte de Producción.

**Recorrido:** registrar → completar propiedades → filtrar por procedencia → administrar o asociar → comprobar la producción. Para distinguir las demás clases de herrajes, consulta [Creación de Herrajes](README.md).

<figure><img src="../.gitbook/assets/image (6) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1).png" alt="Vista general del formulario Accesorios y su listado de referencias en Cabinet Report"><figcaption>Pantalla histórica de Accesorios: identifica el área de registro y el listado antes de operar sobre una referencia.</figcaption></figure>

## 1. Registrar un accesorio

1. Comprueba que estás en la sección **Accesorios**, y no en **Ferretería de Montaje** ni **Ferretería de Instalación**.
2. Introduce un **nombre identificable** del accesorio y selecciona la **categoría** que le corresponda.
3. Si tu usuario dispone del permiso y la conexión necesarios, pulsa **(+)** para intentar agregar la referencia.
4. Revisa el listado o el mensaje de la interfaz para **confirmar el resultado**; pulsar el botón no demuestra por sí solo que el alta se haya guardado.

La categoría ayuda a clasificar y localizar referencias; no sustituye la comprobación de compatibilidad con el diseño del mueble.

<figure><img src="../.gitbook/assets/image (7) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1).png" alt="Campos de nombre y categoría y botón de agregar un accesorio"><figcaption>Alta de accesorio: registra el nombre, elige la categoría y verifica el resultado de la acción (+).</figcaption></figure>

## 2. Completar y verificar las propiedades

Después de crear o seleccionar la referencia, revisa los **campos de propiedades que muestre tu versión** y completa únicamente los pertinentes. Comprueba la descripción, la unidad o presentación utilizada y, cuando corresponda, el **precio** necesario para las consultas de [Costos](../costos.md).

No supongas que un precio escrito en el catálogo ya se trasladó a una cotización ni que dos presentaciones distintas (por ejemplo, unidad y paquete) sean equivalentes. Verifica qué datos quedaron guardados y vuelve a consultar la referencia antes de usarla en un trabajo.

<figure><img src="../.gitbook/assets/image (8) (1) (1) (1) (1) (1) (1) (1) (1) (1).png" alt="Área para consultar y completar las propiedades del accesorio"><figcaption>Propiedades del accesorio: comprueba los datos guardados, la unidad y el precio cuando corresponda.</figcaption></figure>

## 3. Filtrar las referencias públicas y privadas

Utiliza los filtros **PÚBLICO** y **PRIVADO** para consultar las referencias que correspondan al contexto y a los permisos de tu usuario.

| Procedencia | Qué debes comprobar |
| --- | --- |
| **PÚBLICO** | Referencias compartidas o generales. Su visualización **no** concede permiso para modificarlas o eliminarlas. |
| **PRIVADO** | Referencias asociadas al cliente propietario. Confirma que el **cliente activo** sea el correcto antes de editar o incorporar un elemento. |

Activar o desactivar un filtro **no cambia la propiedad, el alcance ni la visibilidad** de los registros. Si una referencia esperada no aparece, revisa los filtros, el cliente y el acceso antes de asumir que no existe.

<figure><img src="../.gitbook/assets/image (9) (1) (1) (1) (1) (1) (1) (1) (1).png" alt="Selecciones Público y Privado del listado de accesorios"><figcaption>Filtros de procedencia: permiten consultar referencias públicas o privadas sin modificar su titularidad.</figcaption></figure>

## 4. Administrar una referencia y asociarla a un módulo

La interfaz histórica documenta acciones de administración y selección; **su disponibilidad efectiva no es universal**. Antes de pulsar un control, identifica desde dónde abriste la ventana y qué referencia está seleccionada.

| Acción documentada | Alcance y precaución |
| --- | --- |
| **Agregar al catálogo privado** | Utilízala solo en un contexto autorizado. Comprueba a qué cliente pertenece el resultado; no confundas esta acción con un cambio de filtro o con la incorporación al TXT. |
| **Eliminar** | Revisa la titularidad y los permisos de edición o eliminación. No borres referencias públicas o compartidas para hacer pruebas. |
| **Actualizar el herraje del módulo seleccionado** | Si llegaste desde el [Creador de Módulos](../creacion-de-modulos.md) o el [Catálogo de Módulos](../catalogo-de-modulos.md), y la acción está habilitada, verifica **módulo, referencia y cantidad** antes y después de actualizar. |

La [Documentación Oficial de Herrajes](https://github.com/danielmelendez-pma/CabinetReport-Docs/blob/main/funcionalidades-de-cabinet-report/herrajes-en-desarrollo.md) distingue operaciones maestras, referencias privadas y trabajo con una producción activa. El alta de referencias maestras está limitada en modo **sin conexión**; la consulta y otras operaciones dependen del contexto y los datos disponibles. **Abrir el catálogo desde otra ventana no otorga permisos adicionales.**

<figure><img src="../.gitbook/assets/image (10) (1) (1) (1) (1) (1) (1) (1).png" alt="Controles de administración y selección de accesorios según el contexto"><figcaption>Acciones sobre la referencia seleccionada: su disponibilidad depende del contexto, la versión y los permisos.</figcaption></figure>

{% hint style="info" %}
**Antes de actualizar un módulo:** comprueba cliente, módulo, accesorio, categoría, unidad y cantidad. Si el control de asociación no existe o está deshabilitado en tu versión, regístralo como **no ejecutado**; no infieras que la referencia quedó vinculada.
{% endhint %}

## 5. Distinguir catálogo, módulo y producción

| Dónde lo consultas | Qué demuestra | Qué no demuestra |
| --- | --- | --- |
| **Catálogo de accesorios** | Existe una referencia consultable con sus propiedades y procedencia. | Que esté físicamente disponible, comprada o asignada a algún mueble. |
| **Creador o Catálogo de Módulos** | Puedes comprobar la relación con un módulo, si la función está disponible y se guardó. | Que un cambio posterior del catálogo actualice automáticamente módulos anteriores. |
| **Reporte de Producción y TXT auxiliar** | Puedes comprobar lo realmente incorporado a la producción activa y al archivo generado, cuando exista. | Que la mera alta de catálogo haya generado esas líneas o archivos. |
| **Compras y Costos** | Puedes cotejar cantidades, unidad y precio presentes en esas salidas. | Que haya existencias o que los importes estén actualizados sin revisión. |

**Importante:** **Agregar al catálogo** y **Agregar al TXT** son operaciones distintas. La sincronización de auxiliares requiere el contexto real de producción; verifica siempre el [Reporte de Producción](../reporte-de-produccion/README.md) y los [Archivos de Reportes Generados](../reporte-de-produccion/archivos-de-reportes-generados.md) que correspondan.

## Ejercicio de verificación: del catálogo a la fabricación

El registro de un accesorio en el catálogo **no demuestra** que ya esté incorporado a un módulo, al TXT de una producción ni a un Reporte de Compras. Para comprobar el recorrido sin afectar trabajos reales, utiliza un **cliente, módulo y producción de prueba** y conserva sus datos de origen.

### Caso didáctico reproducible

Supón un accesorio de prueba llamado `ACC-ENSAYO-01` (nombre ilustrativo, no una referencia real verificada) y una necesidad de **2 unidades por módulo** para **2 módulos iguales**. El total teórico sería **4 unidades**. No se afirma que Cabinet Report calcule o exporte automáticamente ese total: el objetivo es contrastarlo con las salidas reales de tu versión.

| Punto de control | Comprobación antes de darlo por válido |
| --- | --- |
| **Referencia** | Nombre, categoría, propiedades y unidad correctos; distinguirla de la ferretería de montaje o instalación. |
| **Visibilidad** | Identificar si el elemento consultado es público o privado y el cliente propietario. Los filtros **PÚBLICO/PRIVADO** no cambian por sí solos la propiedad del registro. |
| **Módulo** | Confirmar que el módulo de ensayo tiene la referencia adecuada y **2 unidades previstas**; comprobar la asociación después de guardar o actualizar, según las acciones disponibles. |
| **Producción** | Verificar el cliente y ambiente, las **2 unidades de módulo** y la cantidad final del accesorio. No asumir propagación automática desde una definición modificada. |
| **Archivo auxiliar** | Si la producción genera un TXT de accesorios, abrirlo y cotejar **referencia, unidad y cantidad** con el RP; no confundir **Agregar al catálogo** con incorporar al **TXT del RP**. |
| **Compras y costos** | Comparar el accesorio con el **Reporte de Compras** y, si se valora en **Costos**, comprobar descripción, unidad y precio unitario. Una salida ausente o una cantidad distinta requiere revisión. |

### Secuencia de prueba y recuperación

1. **Antes de editar**, conserva los datos del módulo y de la producción de prueba. Evita eliminar una referencia existente para hacer el ensayo, especialmente si pertenece a un catálogo compartido.
2. Revisa el accesorio en esta pantalla y su clasificación. Si necesitas una referencia privada, utiliza únicamente las acciones permitidas para el cliente activo; **filtrar** y **agregar al catálogo privado** no son la misma operación.
3. Desde el [Creador de Módulos](../creacion-de-modulos.md) o el [Catálogo de Módulos](../catalogo-de-modulos.md), verifica la referencia y las unidades asociadas al módulo de prueba. Vuelve a abrirlo para comprobar que se conservó la relación esperada.
4. Prepara el [Reporte de Producción](../reporte-de-produccion/README.md) de prueba y revisa la información efectivamente cargada. Si una edición del catálogo no se refleja, **no supongas que actualiza módulos o producciones anteriores**: contrasta la relación guardada y el método de incorporación que admite tu versión.
5. Comprueba los archivos auxiliares realmente generados y el [Reporte de Compras](../reporte-de-compras.md). Para valorar el artículo, consulta [Costos](../costos.md). Contrasta cantidades y **unidades de presentación** antes de comprar o distribuir documentos.
6. Si el resultado no coincide con las **4 unidades teóricas** del ejemplo, conserva la evidencia (referencia, módulo, RP y archivos), corrige la configuración en el entorno de ensayo y **repite la comprobación** antes de usar ese accesorio en una fabricación real.

### Registro del resultado del ejercicio

Anota **versión, cliente, ambiente, módulo, referencia, unidad y archivo de origen**. Para cada punto de control de la tabla, indica **Conforme**, **No conforme** o **No ejecutado**, y guarda la evidencia que permita repetir la comprobación. Si tu instalación no genera un auxiliar o no ofrece una acción de asociación, no lo marques como conforme por suposición.

{% hint style="warning" %}
**Criterio de liberación:** no basta con ver el accesorio en un listado. Deben coincidir su clasificación, asociación al módulo, cantidad y unidad en las salidas que correspondan. Este ejercicio es una **prueba propuesta**, no una prueba funcional ejecutada ni una garantía de propagación automática. Una discrepancia sin resolver impide dar el ensayo por conforme.
{% endhint %}

---

[← Creación de Herrajes](README.md) · [Ferretería de Montaje →](ferreteria-de-montaje.md) · [Catálogo de Módulos](../catalogo-de-modulos.md) · [🏠 Portal principal](https://danielmelendez-pma.github.io/cabinet-report-partners/)
