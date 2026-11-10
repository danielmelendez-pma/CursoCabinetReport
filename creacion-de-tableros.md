---
description: >-
  Guía para registrar, identificar y comprobar referencias de tableros,
  sus dimensiones, veta, visibilidad y datos comerciales antes de producción.
layout:
  width: wide
---

# Creación de Tableros

Aprende a **identificar, registrar y comprobar referencias de tableros** antes de utilizarlas en módulos y producciones. Se conservan las capturas históricas de la interfaz: algunos controles dependen de la versión de Cabinet Report y de los permisos del usuario.

## Recorrido de aprendizaje

1. **Identifica la referencia** y comprueba si ya existe en el catálogo.
2. **Registra sus características** y determina la visibilidad pública o privada permitida.
3. **Consulta, filtra y gestiona** la ficha sin confundir el catálogo con existencias físicas.
4. **Comprueba un caso de ensayo** antes de asignar el tablero a piezas o autorizar cortes.

La referencia funcional para permisos y operaciones es [Stock de Tableros — Documentación Oficial](https://cabinet-report.gitbook.io/cabinet-report-docs/funcionalidades-de-cabinet-report/stock-de-tableros).

<figure><img src=".gitbook/assets/image (13) (1) (1) (1) (1) (1).png" alt="Vista general de la sección Stock de Tableros de Cabinet Report"><figcaption><p>Reconoce el catálogo de referencias antes de crear o seleccionar materiales.</p></figcaption></figure>

En **Stock de Tableros** se consultan referencias existentes, incluidas las del catálogo público que permite visualizar tu perfil. Cada ficha puede aportar medidas, marca, proveedor e imagen; **estar registrada no significa que la plancha esté disponible en el almacén**.

<figure><img src=".gitbook/assets/IcoAglomeradosGrande.png" alt="Icono del catálogo de aglomerados y tableros" width="188"><figcaption><p>Acceso visual asociado al área de tableros o aglomerados.</p></figcaption></figure>

## 1. Antes de registrar un tablero

1. **Busca primero la referencia:** compara nombre comercial, fabricante, código de proveedor, espesor y acabado para evitar registros duplicados con nombres ligeramente diferentes.
2. **Verifica la ficha del producto:** confirma medidas de la plancha, tipo de material y dirección real de la veta. Una imagen o un nombre parecido no garantiza que sean el mismo tablero.
3. **Decide dónde debe guardarse:** usa una referencia privada cuando corresponda a tu empresa; solo el personal autorizado puede administrar las referencias públicas.
4. **Aclara el propósito:** Stock de Tableros es un catálogo de referencias; no confirma existencias físicas, reservas ni cantidades disponibles en almacén.

Para el alcance de permisos, búsqueda y clonación, consulta la [Documentación oficial — Stock de Tableros](https://cabinet-report.gitbook.io/cabinet-report-docs/funcionalidades-de-cabinet-report/stock-de-tableros).

## 2. Registrar un tablero

Para incorporar una referencia propia, abre la sección de registro cuando esté disponible para tu perfil. **Busca antes un tablero equivalente** y evita duplicar la misma marca, código, espesor y acabado.

<figure><img src=".gitbook/assets/image (14) (1) (1) (1) (1).png" alt="Pantalla de registro de un tablero con campos técnicos de tipo y dimensiones"><figcaption><p>Comprueba nombre, tipo, veta, espesor, ancho y largo antes de continuar.</p></figcaption></figure>

### Campos de la ficha

Sigue la secuencia de identificación de la captura: tipo y nombre, propiedades de la plancha, información comercial y, finalmente, comprobación antes de guardar. No inventes una referencia si el producto aún no está identificado.

**TIPO:** selecciona el tipo de tablero mostrado en el catálogo, por ejemplo AGL (aglomerado), MDF o CART (cartón). Esta clasificación **no establece el significado de la variable `CART` en una fórmula de piezas**; esa definición sigue pendiente de comprobación técnica.

**NOMBRE AGLOMERADO:** escribe el nombre comercial del tablero sin añadir el prefijo AGL cuando este ya esté representado en el campo de tipo.

**VETA:** en el control documentado se utiliza `0` para tableros sin veta direccional y `1` para tableros con veta. Confirma el dato con la ficha técnica.

**ESP:** registra el espesor real del producto en las unidades aplicables y comprueba que coincida con el material previsto para las piezas.

**ANCHO:** registra la dimensión comercial correspondiente según la ficha del fabricante. Aunque suele ser el lado menor, no inviertas medidas automáticamente.

**LARGO:** registra el largo comercial según la ficha del tablero. Habitualmente es la dimensión mayor, pero no supongas que la veta siempre sigue ese eje: confirma la orientación indicada por el fabricante.

{% hint style="warning" %}
**Control antes de guardar:** comprueba las unidades y el orden **ANCHO/LARGO**, el espesor real y el valor de **VETA**. Si la dirección de veta del producto difiere de la orientación habitual, no la corrijas por suposición: verifica la ficha técnica y el corte previsto.
{% endhint %}

***

## 3. Visibilidad y datos comerciales

Después de identificar el material y sus medidas, registra **la visibilidad permitida** y los datos comerciales. No confundas la información que se muestra con las acciones que tu usuario tiene autorizadas.

<figure><img src=".gitbook/assets/image (15) (1) (1) (1).png" alt="Área para visibilidad pública o privada y datos de proveedor y fabricante"><figcaption><p>Revisa permisos de visibilidad, proveedor, código y fabricante.</p></figcaption></figure>

**PÚBLICO:** identifica referencias compartidas del catálogo general. **No todos los usuarios pueden crearlas, editarlas o eliminarlas**: la documentación oficial reserva su administración a los permisos de nivel A.

**PRIVADO:** corresponde a las referencias del cliente propietario. Los permisos de nivel B se limitan a sus referencias privadas; comprueba la visibilidad permitida por tu perfil antes de guardar.

**Proveedor:** registra la empresa que suministra el tablero.

**Código:** registra el identificador utilizado por el proveedor en sus catálogos o facturas.

**Fabricante:** indica la marca o empresa fabricante del producto.

**Precio:** dato opcional del registro que puede utilizarse en Costos cuando corresponda; un valor guardado no confirma una cotización vigente del proveedor.

{% hint style="info" %}
**Visibilidad no equivale a permiso de edición.** El nivel A administra referencias públicas; el nivel B está limitado a las privadas del cliente según las condiciones documentadas. Ver una ficha pública no concede autorización para modificarla. Para adaptar una referencia compartida, utiliza **Agregar a mi catálogo** únicamente si tu perfil lo permite y comprueba los datos de la copia privada.
{% endhint %}

***

## 4. Identificar el tablero mediante una imagen

La imagen puede ayudarte a reconocer el color o acabado, pero **no sustituye** fabricante, código ni ficha técnica. El editor documentado dispone de estas acciones cuando estén habilitadas:

<figure><img src=".gitbook/assets/image (7) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1).png" alt="Sección de imagen del tablero y búsqueda de su ficha técnica"><figcaption><p>La fotografía ayuda a identificar el acabado; la ficha técnica debe contrastarse por producto.</p></figcaption></figure>

**Agregar imagen:** selecciona una fotografía o referencia visual correspondiente al producto identificado.

**Ampliar:** permite observar la imagen con mayor detalle en otra ventana.

**Eliminar imagen:** retira la imagen asociada; comprueba que estás actuando sobre la ficha correcta.

**Realizar búsqueda de Ficha Técnica:** abre una búsqueda en Internet para localizar información del producto. **Una búsqueda no garantiza una ficha oficial ni que corresponda exactamente al tablero elegido**; confirma fabricante, código, acabado y espesor antes de tomar sus datos como referencia.

***

## 5. Buscar y filtrar tableros

En la consulta puedes visualizar las referencias públicas y privadas que estén permitidas para tu perfil.

<figure><img src=".gitbook/assets/image (4) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1).png" alt="Listado de tableros públicos y privados disponibles para consulta"><figcaption><p>Consulta las referencias permitidas y distingue catálogo público de privado.</p></figcaption></figure>

Escribe un nombre o parte de él en **Filtrar Aglomerados** para localizar coincidencias. Si aparecen varias referencias parecidas, compara fabricante, código, espesor, acabado y medidas antes de elegir.

<figure><img src=".gitbook/assets/image (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1).png" alt="Campo Filtrar Aglomerados y controles de visibilidad de la lista"><figcaption><p>El filtro acota la lista visible, pero no cambia la titularidad ni los permisos.</p></figcaption></figure>

Si quieres trabajar solo con referencias privadas, desmarca la opción **Público** cuando esté disponible. Los filtros cambian lo que se muestra en la lista, **no los permisos de edición ni la titularidad** de cada registro.

***

## 6. Guardar, eliminar y clonar referencias

Las operaciones siguientes requieren revisar la **referencia seleccionada y los permisos del perfil**. No todas las acciones están habilitadas para todos los usuarios.

### Agregar una referencia

<figure><img src=".gitbook/assets/IcoAgregar.png" alt="Icono de la acción Agregar una referencia de tablero"><figcaption><p>Guarda la ficha solo después de comprobar sus campos técnicos y comerciales.</p></figcaption></figure>

Con los campos revisados y los permisos adecuados, pulsa este botón para guardar la referencia. Después **búscala de nuevo** y confirma que se conservaron tipo, nombre, proveedor, código, dimensiones, espesor, veta y visibilidad.

<figure><img src=".gitbook/assets/IcoBorrar.png" alt="Icono de la acción Eliminar una referencia de tablero"><figcaption><p>Confirma la identidad de la referencia y su autorización antes de eliminarla.</p></figcaption></figure>

### Eliminar una referencia

Selecciona el tablero correcto y verifica que tengas autorización para eliminarlo. La eliminación puede afectar referencias que otros trabajos utilizan; no borres registros por similitud de nombres ni asumas que puedes eliminar referencias públicas.

{% hint style="warning" %}
**Antes de eliminar:** verifica nombre, fabricante, código y visibilidad. Si no puedes determinar si la referencia se utiliza en un trabajo existente, no la elimines como parte de un ejercicio.
{% endhint %}

<figure><img src=".gitbook/assets/image (3) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1).png" alt="Control para incorporar una referencia pública al catálogo privado"><figcaption><p>Verifica que la clonación genere la referencia privada esperada, sin modificar la pública.</p></figcaption></figure>

### Agregar una referencia pública a mi catálogo

Utiliza esta opción para **clonar una referencia pública al catálogo privado**, si está habilitada para tu perfil. Después localiza la nueva referencia privada y verifica sus datos; duplicar no significa editar la ficha pública ni confirmar stock físico.

## 7. Comprobación antes de producción

1. **Identidad:** verifica fabricante, nombre, código y acabado contra el material pedido o disponible físicamente.
2. **Geometría:** confirma dimensiones de plancha y espesor, incluyendo las unidades; no intercambies ancho y largo por costumbre.
3. **Veta:** comprueba si es direccional y su orientación frente a las piezas y el plan de corte.
4. **Catálogo:** confirma si seleccionaste la referencia pública o la copia privada correcta y que tienes permiso para gestionarla.
5. **Despiece:** en el [Catálogo de Módulos](catalogo-de-modulos.md) comprueba que la selección actualiza los materiales previstos; revisa las piezas resultantes en el [Reporte de Producción](reporte-de-produccion/README.md).
6. **Disponibilidad real:** valida existencias con el almacén o proveedor; este catálogo no es una confirmación de inventario.

{% hint style="warning" %}
**No autorices cortes solo porque el tablero aparece en el catálogo.** Un espesor, formato, veta o acabado incorrecto puede trasladarse al despiece y a la optimización. Contrasta la referencia con la ficha del producto y el diseño antes de fabricar.
{% endhint %}

## 8. Ejercicio de comprobación: una referencia de ensayo

Realiza este ensayo **solo sobre una referencia privada que puedas gestionar con autorización** o mediante una ficha existente que puedas consultar sin modificar. No elimines materiales de trabajo ni alteres el catálogo público para completar la práctica.

1. **Identifica un tablero de referencia:** anota fabricante, proveedor, código, tipo, acabado, espesor, ancho, largo y veta desde la ficha técnica verificable.
2. **Busca antes de registrar:** utiliza el filtro y anota si ya existe una ficha equivalente. Si existe, evita crear un duplicado solo para superar el ejercicio.
3. **Verifica la visibilidad y la operación permitida:** comprueba si es pública o privada; si está habilitada la clonación de una pública, contrasta los datos de la copia con la ficha de origen.
4. **Contrasta la salida:** consulta el [Catálogo de Módulos](catalogo-de-modulos.md) y la [Revisión de Tableros y Cantos](reporte-de-produccion/revision-de-tableros-y-cantos.md) cuando trabajes con una producción de ensayo. Comprueba que el material asignado y sus atributos sean los esperados; una vista del catálogo no acredita el resultado de producción.
5. **Documenta el resultado:** conserva las evidencias necesarias sin registrar como correcto lo que no hayas comprobado.

| Control | Evidencia a registrar | Resultado |
| --- | --- | --- |
| Identificación | Fabricante, código y acabado coinciden con la ficha del producto. | Conforme / No conforme / No ejecutado |
| Dimensiones y veta | Espesor, ancho, largo, unidades y orientación comprobados. | Conforme / No conforme / No ejecutado |
| Catálogo y permisos | Visibilidad correcta y acción autorizada; copia privada revisada si corresponde. | Conforme / No conforme / No ejecutado |
| Uso en producción, si se ensaya | Material de piezas y datos técnicos contrastados con el diseño. | Conforme / No conforme / No ejecutado |
| Existencia física | Confirmación independiente del almacén o proveedor. | Conforme / No conforme / No ejecutado |

Marca **No ejecutado** cuando falten permisos, evidencias o una producción de ensayo. Una ficha correcta no permite deducir la existencia física del material ni autoriza por sí sola la fabricación.

## Para continuar

Revisa [Creación de Módulos](creacion-de-modulos.md) para entender cómo se integra el material en una definición, [Fórmulas y Variables](formulas-y-variables.md) para contrastar espesores y descuentos, y [Costos](costos.md) si necesitas trabajar con referencias de precios, sin tratarlas como cotizaciones actuales.

---

[← Pantalla principal](pantalla-principal.md) · [Fórmulas y variables →](formulas-y-variables.md) · [🏠 Portal principal](https://danielmelendez-pma.github.io/cabinet-report-partners/)
