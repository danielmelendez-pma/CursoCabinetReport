---
description: Registra ferretería de montaje, completa propiedades, filtra catálogos y selecciona herrajes por categoría.
---

# Ferretería de Montaje

La sección **Ferretería de Montaje** reúne las opciones para crear y administrar los herrajes utilizados en el montaje de los muebles.

<figure><img src="../.gitbook/assets/image (16) (1) (1) (1).png" alt=""><figcaption></figcaption></figure>

## 1. Crear un herraje de montaje

1. Escribe el **nombre** de la ferretería.
2. Selecciona la **categoría** y el **tipo**.
3. Pulsa el botón **(+)** para registrarla.

<figure><img src="../.gitbook/assets/image (18) (1).png" alt=""><figcaption></figcaption></figure>

## 2. Completar las propiedades

Después de crear el herraje, puedes agregar las propiedades necesarias para su uso, incluido el **precio** cuando corresponda utilizarlo en el módulo de Costos.

<figure><img src="../.gitbook/assets/image (19).png" alt=""><figcaption></figcaption></figure>

## 3. Filtrar el catálogo

Utiliza las opciones **PÚBLICO** y **PRIVADO** para filtrar la ferretería disponible.

<figure><img src="../.gitbook/assets/image (20).png" alt=""><figcaption></figcaption></figure>

## 4. Administrar la selección

Desde el listado puedes **agregar la ferretería seleccionada al catálogo privado** o **eliminarla**. Si estás trabajando desde el **Creador de Módulos** o el **Catálogo de Módulos**, puedes **actualizar el herraje del módulo seleccionado**.

<figure><img src="../.gitbook/assets/image (21).png" alt=""><figcaption></figcaption></figure>

## 5. Buscar por categoría

Haz clic en la **imagen de una categoría** para filtrar la lista de ferretería. Por ejemplo, al seleccionar **Rieles**, verás los rieles agregados a esa categoría.

<figure><img src="../.gitbook/assets/image (6) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1).png" alt="" width="211"><figcaption></figcaption></figure>

<figure><img src="../.gitbook/assets/image (4) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1).png" alt=""><figcaption></figcaption></figure>

{% hint style="info" %}
**Antes de aplicarlo a un módulo:** comprueba la categoría, el tipo y las propiedades del herraje seleccionado.
{% endhint %}

## 6. Ensayo de liberación de kits de ferretería de montaje en fábrica

Esta prueba documental comprueba si los herrajes **previstos por módulo** pueden prepararse para el armado sin confundirlos con accesorios ni con ferretería de instalación en obra. Es un **ensayo propuesto**, no una prueba funcional ejecutada en Windows. Las asignaciones de kits y las verificaciones físicas son **controles manuales del taller**; no se presume que Cabinet Report los realice automáticamente.

### Preparación y datos de ensayo

1. Crea o utiliza una **producción de prueba**, con cliente y ambiente reconocibles; guarda una copia de los datos iniciales para poder repetir la comprobación sin afectar un trabajo real.
2. Selecciona una referencia que figure como **Ferretería de Montaje** y anota nombre, tipo, categoría, unidad y propiedades. Distingue **PÚBLICO/PRIVADO** y al cliente propietario; filtrar no implica clonar, editar ni incorporar la referencia al RP.
3. Verifica la relación de esa referencia con cada módulo en [Creación de Módulos](../creacion-de-modulos.md) o [Catálogo de Módulos](../catalogo-de-modulos.md). No supongas que una modificación posterior del registro maestro actualiza automáticamente módulos ya guardados.
4. Define con el responsable técnico **cuánto necesita cada módulo** según el diseño y la unidad real de suministro; no deduzcas consumos a partir del nombre comercial del herraje.

**Caso exclusivamente ilustrativo:** dos módulos de prueba identificados como **M-A** y **M-B** requieren **4 unidades cada uno** de una misma referencia ficticia `FM-ENSAYO-01`. El total previsto es **8 unidades**, pero la preparación física coloca **6 en el kit M-A** y **2 en el kit M-B**. El total preparado también es 8: **la suma general coincide, aunque los kits están mal distribuidos**. Ni esos nombres ni el reparto corresponden a un algoritmo acreditado del programa.

| Kit / puesto de armado | Previsto por ficha técnica | Preparado físicamente | Diferencia manual | Resultado |
| --- | ---: | ---: | ---: | --- |
| M-A | 4 unidades | 6 unidades | +2 | Excedente; redistribuir |
| M-B | 4 unidades | 2 unidades | −2 | Faltante; no liberar |
| **Total de la producción** | **8 unidades** | **8 unidades** | **0** | **No valida los kits individuales** |

### Comprobación del recorrido hasta el banco de montaje

| Punto | Evidencia que debes comprobar | Límite de la comprobación |
| --- | --- | --- |
| **Catálogo** | Referencia de **montaje**, tipo, propiedades, unidad y visibilidad correctos. | Existir en el catálogo no prueba asociación con un módulo. |
| **Ficha de cada módulo** | Identificador, cantidad de módulos y necesidad de la referencia por cada conjunto. | El total de piezas del RP no equivale por sí solo al total de kits. |
| **Reporte de Producción** | Cliente, ambiente, módulos y herrajes efectivamente incorporados al [RP](../reporte-de-produccion/reporte-de-produccion.md). | La selección de un registro maestro no acredita su inclusión en la producción. |
| **TXT de montaje** | Si se genera el auxiliar, cotejar referencia, unidad y cantidad con la fuente aprobada; ver [Archivos generados](../reporte-de-produccion/archivos-de-reportes-generados.md). | El TXT puede no detallar el reparto físico por kit. No inventes campos ausentes. |
| **Compras y entrega interna** | Cuando corresponda, comparar las partidas del [Reporte de Compras](../reporte-de-compras.md) y los documentos de entrega disponibles. | Un Excel o una orden no confirman existencia ni entrega física. |
| **Banco de montaje** | Verificación **manual** de contenido, etiqueta de módulo, cantidad, compatibilidad y recepción de cada kit. | La inspección de operarios no es una función automática demostrada del software. |

### Ejecutar, corregir y aceptar la prueba

1. Abre la producción de ensayo y comprueba **módulos, cantidades y herrajes** tras las operaciones disponibles en tu versión. Si modificas una asociación, vuelve a verificar lo realmente guardado.
2. Si se producen archivos de ferretería, conserva el **TXT original** y contrástalo con el RP. Si no se genera alguno, registra «no generado» y revisa la configuración; no completes el archivo manualmente para fingir una salida del programa.
3. Prepara una **hoja manual por kit** a partir de la ficha aprobada: cliente, ambiente, módulo, referencia exacta, unidad y cantidad prevista. No atribuyas esta hoja a una exportación automática de Cabinet Report.
4. Reproduce el reparto didáctico **6/2**, comprueba por separado los dos kits y registra el desvío. Rectifica a **4/4**, vuelve a contar y solicita la aceptación del responsable de montaje antes de liberar cada kit.
5. Conserva la evidencia mínima: versión del programa, módulo y RP de origen, nombres y fechas de archivos consultados, valores previstos, cantidades físicamente preparadas, incidencias, corrección, responsable y fecha de aprobación.

{% hint style="warning" %}
**Criterio de aceptación y detención:** no liberes un kit para ensamblaje si presenta **referencia equivocada, unidad no conciliada, faltantes, excedentes sin resolver o asignación a otro módulo**, aunque el total global coincida. El responsable debe verificar **cada kit individualmente** y confirmar la corrección; esto no implica que el programa bloquee automáticamente el armado.
{% endhint %}

---

[← Accesorios](accesorios.md) · [Creación de Herrajes](README.md) · [Ferretería de Instalación →](ferreteria-de-instalacion.md) · [🏠 Portal principal](https://danielmelendez-pma.github.io/cabinet-report-partners/)
