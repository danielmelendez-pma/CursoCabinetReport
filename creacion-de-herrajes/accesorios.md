---
description: Aprende a crear accesorios, configurar sus propiedades y gestionar su visibilidad en el catálogo de Cabinet Report.
---

# Accesorios

La sección **Accesorios** permite registrar un accesorio en la base de datos, completar sus propiedades y seleccionarlo para utilizarlo en módulos cuando corresponda.

<figure><img src="../.gitbook/assets/image (6) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1).png" alt=""><figcaption></figcaption></figure>

## 1. Crear un accesorio

1. Introduce el **nombre** del accesorio.
2. Selecciona su **categoría**.
3. Pulsa el botón **(+)** para agregarlo a la base de datos.

<figure><img src="../.gitbook/assets/image (7) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1).png" alt=""><figcaption></figcaption></figure>

## 2. Completar sus propiedades

Después de crearlo, puedes agregar otras propiedades según el accesorio. Completa únicamente los datos que correspondan, incluido el **precio** cuando necesites utilizarlo en el módulo de Costos.

<figure><img src="../.gitbook/assets/image (8) (1) (1) (1) (1) (1) (1) (1) (1) (1).png" alt=""><figcaption></figcaption></figure>

## 3. Filtrar los accesorios disponibles

Utiliza las selecciones **PÚBLICO** y **PRIVADO** para filtrar los accesorios que aparecen en el listado.

<figure><img src="../.gitbook/assets/image (9) (1) (1) (1) (1) (1) (1) (1) (1).png" alt=""><figcaption></figcaption></figure>

## 4. Administrar y utilizar el accesorio

Desde esta sección puedes **agregar el accesorio seleccionado a tu catálogo privado** o **eliminarlo**. Si accediste desde el **Creador de Módulos** o el **Catálogo de Módulos**, también puedes **actualizar el herraje del módulo seleccionado**.

<figure><img src="../.gitbook/assets/image (10) (1) (1) (1) (1) (1) (1) (1).png" alt=""><figcaption></figcaption></figure>

{% hint style="info" %}
**Antes de actualizar un módulo:** verifica que el accesorio elegido, su categoría y sus propiedades correspondan al trabajo.
{% endhint %}

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

{% hint style="warning" %}
**Criterio de liberación:** no basta con ver el accesorio en un listado. Debe coincidir su clasificación, asociación al módulo, cantidad y unidad en las salidas que correspondan. Este ejercicio es una **prueba propuesta**, no una prueba funcional ejecutada ni una garantía de propagación automática.
{% endhint %}

---

[← Creación de Herrajes](README.md) · [Ferretería de Montaje →](ferreteria-de-montaje.md) · [Catálogo de Módulos](../catalogo-de-modulos.md) · [🏠 Portal principal](https://danielmelendez-pma.github.io/cabinet-report-partners/)
