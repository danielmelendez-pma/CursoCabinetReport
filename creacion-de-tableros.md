# Creación de Tableros

Aprende a registrar y verificar referencias de tableros, distinguir el catálogo público del privado y preparar materiales confiables para los módulos y el Reporte de Producción. Esta lección explica el recorrido de las capturas originales; la disponibilidad de controles depende de la versión y de los permisos del usuario.

<figure><img src=".gitbook/assets/image (13) (1) (1) (1) (1) (1).png" alt=""><figcaption></figcaption></figure>

En la sección de **Stock de Tableros** puedes encontrar una variedad de tableros ya creados en el catálogo público para uso en sus proyectos, con sus medidas, marca e imagen.

<figure><img src=".gitbook/assets/IcoAglomeradosGrande.png" alt="" width="188"><figcaption></figcaption></figure>

## Antes de registrar un tablero

1. **Busca primero la referencia:** compara nombre comercial, fabricante, código de proveedor, espesor y acabado para evitar registros duplicados con nombres ligeramente diferentes.
2. **Verifica la ficha del producto:** confirma medidas de la plancha, tipo de material y dirección real de la veta. Una imagen o un nombre parecido no garantiza que sean el mismo tablero.
3. **Decide dónde debe guardarse:** usa una referencia privada cuando corresponda a tu empresa; solo el personal autorizado puede administrar las referencias públicas.
4. **Aclara el propósito:** Stock de Tableros es un catálogo de referencias; no confirma existencias físicas, reservas ni cantidades disponibles en almacén.

Para el alcance de permisos, búsqueda y clonación, consulta la [Documentación oficial — Stock de Tableros](https://cabinet-report.gitbook.io/cabinet-report-docs/funcionalidades-de-cabinet-report/stock-de-tableros).

## Crear un tablero

También puedes crear tus propios tableros para uso privado desde la siguiente sección:

<figure><img src=".gitbook/assets/image (14) (1) (1) (1) (1).png" alt=""><figcaption></figcaption></figure>

**TIPO:** selecciona el tipo de tablero mostrado en el catálogo, por ejemplo AGL (aglomerado), MDF o CART (cartón). Esta clasificación **no establece el significado de la variable `CART` en una fórmula de piezas**; esa definición sigue pendiente de comprobación técnica.

**NOMBRE AGLOMERADO:** Es donde vas a colocar el nombre del tablero, sin colocar abreviatura o prefijo AGL.

**VETA:** Este lleva el valor "0" para tableros sin Vetas y "1" para tableros con Vetas.

**ESP:** Aquí debes colocar el espesor del tablero.

**ANCHO:** Lugar donde colocas el ancho del tablero. Por lo general el ancho es la medida más angosta acorde a la mayoría de los fabricantes.

**LARGO:** registra el largo comercial según la ficha del tablero. Habitualmente es la dimensión mayor, pero no supongas que la veta siempre sigue ese eje: confirma la orientación indicada por el fabricante.

{% hint style="warning" %}
**Control antes de guardar:** comprueba las unidades y el orden **ANCHO/LARGO**, el espesor real y el valor de **VETA**. Si la dirección de veta del producto difiere de la orientación habitual, no la corrijas por suposición: verifica la ficha técnica y el corte previsto.
{% endhint %}

***

## Visibilidad y datos comerciales

Luego de ingresar las medidas y el nombre del tablero, completa los datos de proveedor y fabricante.

<figure><img src=".gitbook/assets/image (15) (1) (1) (1).png" alt=""><figcaption></figcaption></figure>

**PÚBLICO:** identifica referencias compartidas del catálogo general. **No todos los usuarios pueden crearlas, editarlas o eliminarlas**: la documentación oficial reserva su administración a los permisos de nivel A.

**PRIVADO:** corresponde a las referencias del cliente propietario. Los permisos de nivel B se limitan a sus referencias privadas; comprueba la visibilidad permitida por tu perfil antes de guardar.

**Proveedor:** Para colocar el nombre del Proveedor local que suministra el tablero en su País.

**Código:** Código que le asigna el Proveedor para identificar al tablero en sus facturas.

Fabricante: Aquí colocar la marca o fabricante del tablero que está creando.

**Precio:** dato opcional del registro que puede utilizarse en Costos cuando corresponda; un valor guardado no confirma una cotización vigente del proveedor.

{% hint style="info" %}
**No confundas visibilidad con propiedad.** Ver un tablero público no significa poder modificarlo. Si necesitas personalizar una referencia pública, utiliza **Agregar a mi catálogo** cuando tu versión y tus permisos lo permitan, y revisa la copia privada antes de utilizarla.
{% endhint %}

***

## Imagen del tablero

También tienes la opción de agregar una imagen para identificar el color del tablero:

<figure><img src=".gitbook/assets/image (7) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1).png" alt=""><figcaption></figcaption></figure>

**Agregar Imagen:** Al hacer clic aquí puede seleccionar la imagen del tablero para agregarla.

**Ampliar:** Opcion para ver la imagen en un tamaño más grande en otra ventana ampliada.

**Eliminar:** Para eliminar la imagen agregada.

**Realizar búsqueda de Ficha Técnica:** abre una búsqueda en Internet para localizar información del producto. **Una búsqueda no garantiza una ficha oficial ni que corresponda exactamente al tablero elegido**; confirma fabricante, código, acabado y espesor antes de tomar sus datos como referencia.

***

## Buscar y filtrar tableros

Desde esta parte puedes visualizar la lista de tableros públicos y privados de tu empresa.

<figure><img src=".gitbook/assets/image (4) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1).png" alt=""><figcaption></figcaption></figure>

Puede realizar búsquedas escribiendo en el campo de **Filtrar Aglomerados**, para mostrar la lista de solos los tableros que coinciden con la frase buscada.

<figure><img src=".gitbook/assets/image (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1).png" alt=""><figcaption></figcaption></figure>

Si quieres trabajar solo con referencias privadas, desmarca la opción **Público** cuando esté disponible. Los filtros cambian lo que se muestra en la lista, **no los permisos de edición ni la titularidad** de cada registro.

***

## Agregar, eliminar y duplicar

Los siguientes elementos permiten gestionar los tableros:

<figure><img src=".gitbook/assets/IcoAgregar.png" alt=""><figcaption></figcaption></figure>

Con los campos revisados y los permisos adecuados, pulsa este botón para guardar la referencia. Después **búscala de nuevo** y confirma que se conservaron tipo, nombre, proveedor, código, dimensiones, espesor, veta y visibilidad.

<figure><img src=".gitbook/assets/IcoBorrar.png" alt=""><figcaption></figcaption></figure>

Selecciona el tablero correcto y verifica que tengas autorización para eliminarlo. La eliminación puede afectar referencias que otros trabajos utilizan; no borres registros por similitud de nombres ni asumas que puedes eliminar referencias públicas.

<figure><img src=".gitbook/assets/image (3) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1).png" alt=""><figcaption></figcaption></figure>

Utiliza esta opción para **clonar una referencia pública al catálogo privado**, si está habilitada para tu perfil. Después localiza la nueva referencia privada y verifica sus datos; duplicar no significa editar la ficha pública ni confirmar stock físico.

## Comprobación antes de usar el tablero en producción

1. **Identidad:** verifica fabricante, nombre, código y acabado contra el material pedido o disponible físicamente.
2. **Geometría:** confirma dimensiones de plancha y espesor, incluyendo las unidades; no intercambies ancho y largo por costumbre.
3. **Veta:** comprueba si es direccional y su orientación frente a las piezas y el plan de corte.
4. **Catálogo:** confirma si seleccionaste la referencia pública o la copia privada correcta y que tienes permiso para gestionarla.
5. **Despiece:** en el [Catálogo de Módulos](catalogo-de-modulos.md) comprueba que la selección actualiza los materiales previstos; revisa las piezas resultantes en el [Reporte de Producción](reporte-de-produccion/README.md).
6. **Disponibilidad real:** valida existencias con el almacén o proveedor; este catálogo no es una confirmación de inventario.

{% hint style="warning" %}
**No autorices cortes solo porque el tablero aparece en el catálogo.** Un espesor, formato, veta o acabado incorrecto puede trasladarse al despiece y a la optimización. Contrasta la referencia con la ficha del producto y el diseño antes de fabricar.
{% endhint %}

---

[← Pantalla principal](pantalla-principal.md) · [Fórmulas y variables →](formulas-y-variables.md) · [🏠 Portal principal](https://danielmelendez-pma.github.io/cabinet-report-partners/)
