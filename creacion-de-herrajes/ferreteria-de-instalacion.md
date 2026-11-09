---
description: Crea ferretería de instalación, configura sus propiedades y filtra herrajes por categoría o visibilidad.
---

# Ferretería de Instalación

La sección **Ferretería de Instalación** permite registrar y administrar los herrajes necesarios para las tareas de instalación de muebles.

<figure><img src="../.gitbook/assets/image (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1).png" alt=""><figcaption></figcaption></figure>

## 1. Crear un herraje de instalación

1. Escribe el **nombre** de la ferretería.
2. Selecciona la **categoría** y el **tipo**.
3. Pulsa el botón **(+)** para agregarla.

<figure><img src="../.gitbook/assets/image (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1).png" alt=""><figcaption></figcaption></figure>

## 2. Completar las propiedades

Después de crear el herraje, agrega las propiedades que necesites, incluido el **precio** cuando corresponda utilizarlo en el módulo de Costos.

<figure><img src="../.gitbook/assets/image (2) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1).png" alt=""><figcaption></figcaption></figure>

## 3. Filtrar el listado

Utiliza las opciones **PÚBLICO** y **PRIVADO** para filtrar la ferretería disponible.

<figure><img src="../.gitbook/assets/image (20).png" alt=""><figcaption></figcaption></figure>

## 4. Administrar y aplicar un herraje

Desde esta sección puedes **agregar la ferretería seleccionada a tu catálogo privado** o **eliminarla**. Si accediste desde el **Creador de Módulos** o el **Catálogo de Módulos**, también puedes **actualizar el herraje del módulo seleccionado**.

<figure><img src="../.gitbook/assets/image (21).png" alt=""><figcaption></figcaption></figure>

## 5. Localizar herrajes por categoría

Selecciona la **imagen de una categoría** para filtrar la lista. Por ejemplo, al elegir **Tornillos** se muestran los tornillos registrados en esa categoría.

<figure><img src="../.gitbook/assets/image (5) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1).png" alt="" width="171"><figcaption></figcaption></figure>

<figure><img src="../.gitbook/assets/image (3) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1).png" alt=""><figcaption></figcaption></figure>

{% hint style="info" %}
**Verificación recomendada:** revisa las propiedades y la categoría del herraje antes de incorporarlo a un módulo o planificar su uso.
{% endhint %}

## 6. Ensayo de trazabilidad: de la ferretería de instalación a la obra

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
