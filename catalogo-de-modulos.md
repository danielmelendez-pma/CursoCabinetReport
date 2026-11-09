# Catálogo de Módulos

<figure><img src=".gitbook/assets/image (14) (1) (1) (1).png" alt=""><figcaption></figcaption></figure>

## Selecciona y configura un módulo

**Preparación:** confirma el cliente y ambiente de destino, identifica el catálogo que usarás y ten a mano las dimensiones y los materiales del diseño. Para crear una definición nueva, utiliza antes [Creación de Módulos](creacion-de-modulos.md); esta lección se centra en **seleccionar y adaptar** una definición del catálogo.

A continuación se describen las partes de la ventana de <mark style="color:$primary;">**Catálogo de Módulos**</mark> y te explico como funciona cada una paso a paso:

Crear la carpeta donde se guardará el archivo de muebles ingresando los valores de Cliente y Ambiente. Si ya está creada, debes abrirla y seleccionar el archivo.

<figure><img src=".gitbook/assets/image (3) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1).png" alt=""><figcaption></figcaption></figure>

<figure><img src=".gitbook/assets/image (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1).png" alt=""><figcaption></figcaption></figure>

Seleccionar si vas a trabajar con Catálogos Públicos o Privado

Seleccionar el Catálogo, Categoría y SubCategoría.

Se filtrará la lista de muebles previamente creados que corresponde a la selección.

<figure><img src=".gitbook/assets/image (4) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1).png" alt=""><figcaption></figcaption></figure>

<figure><img src=".gitbook/assets/image (3) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1).png" alt=""><figcaption></figcaption></figure>

También aparecerán las imágenes de los muebles seleccionados...

Una vez filtrado, puedes seleccionar un mueble tanto de la lista izquierda como de la barra de imagenes superior.

<figure><img src=".gitbook/assets/image (5) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1).png" alt=""><figcaption></figcaption></figure>

Agregar o cambiar las medidas que se va a aplicar a este mueble.

Agregar los tableros de Cajón, Visto y Respaldo que previamente ha creado en la Sección de Creación de Tableros.

Mientras va seleccionado los tableros, automáticamente se van agregando los espesores y el indicador de Vetas.

Metras va seleccionando los tableros, automáticamente se generará el nombre del canto que se aplicará tanto para lo interno como para lo visto:

<figure><img src=".gitbook/assets/image (6) (1) (1) (1) (1) (1) (1) (1) (1) (1).png" alt=""><figcaption></figcaption></figure>

Si gusta, puede cambiar este valor, importante que siempre indique el espesor del canto ejemplo: 0.45MM, 1MM, 1.8MM, 2MM, etc.

<figure><img src=".gitbook/assets/image (7) (1) (1) (1) (1) (1) (1) (1) (1).png" alt=""><figcaption></figcaption></figure>

Revisar y modificar si es necesario los parámetros seleccionados, incluyendo el riel aunque no se vaya a utilizar uno.

Hacer click al botón de Aplicar Parámetros

<figure><img src=".gitbook/assets/image (8) (1) (1) (1) (1) (1) (1) (1).png" alt=""><figcaption></figcaption></figure>

Si todos los campos estan correctos y los valores están seleccionados...Automáticamente la lista de piezas se calculará según las medidas de muebles ingresadas.

<figure><img src=".gitbook/assets/image (9) (1) (1) (1) (1) (1) (1) (1).png" alt=""><figcaption></figcaption></figure>

Revisar o agregar los herrajes creados al mueble seleccionado:

<figure><img src=".gitbook/assets/image (10) (1) (1) (1) (1) (1) (1).png" alt=""><figcaption></figcaption></figure>

Revisar y si alguna pieza no coincide con la medida esperada, puede hacer click en el Botón de Mostrar Fórmulas para revisarla y modificarla.

<figure><img src=".gitbook/assets/image (11) (1) (1) (1) (1) (1).png" alt=""><figcaption></figcaption></figure>

Según el procedimiento mostrado, si modificas una fórmula durante la selección, el cambio se aplica a **este mueble** y no a la definición guardada en la base de datos. Comprueba las piezas recalculadas antes de continuar; no confundas esta edición con una actualización permanente del catálogo.

### Comprueba el módulo antes de incorporarlo

Revisa estos resultados en la lista de piezas calculadas:

- **Medidas y cantidades:** contrástalas con el diseño y con la función de cada pieza, incluidas las luces de puertas y frentes cuando correspondan.
- **Materiales y espesores:** verifica la asignación de tableros de cajón, visto y respaldo.
- **Vetas y cantos:** confirma la orientación y los lados que requieren canteo, sin asumir que un nombre de material basta para validarlos.
- **Fórmulas y herrajes:** revisa cualquier fórmula ajustada para este mueble y los herrajes asociados.

### Caso de control: puertas, luces y variables del cliente

Si un módulo tiene **450 mm de ancho exterior**, no concluyas que una puerta deba medir 450 mm. Las luces, el sistema de apertura y la fórmula aplicable pueden producir una medida diferente. No se fija aquí un valor esperado (447, 448 mm u otro) sin comprobar **la fórmula de esa pieza y los parámetros efectivos del cliente**.

Antes de aceptar un cálculo:

1. Comprueba la **ficha del módulo** y que la fórmula consultada corresponda exactamente a la pieza seleccionada; no transfieras una fórmula de otra pieza solo por compartir nombre.
2. Revisa las **luces, separaciones, espesores y demás variables** que intervengan. Un valor de parámetro **0** puede ser válido y no debe reemplazarse automáticamente por otro.
3. Contrasta el **ancho y largo resultantes**, la orientación de veta y los lados de canto con el diseño y el tipo de apertura.
4. Si cambias una fórmula para este mueble, **vuelve a calcular y revisar las piezas**. No supongas que esa corrección modificó la definición permanente del catálogo.

Para el alcance de estos controles, consulta la [Documentación oficial del Catálogo de Módulos](https://cabinet-report.gitbook.io/cabinet-report-docs/funcionalidades-de-cabinet-report/catalogo-de-modulos) y la [guía del Reporte de Producción](https://cabinet-report.gitbook.io/cabinet-report-docs/funcionalidades-de-cabinet-report/reporte-de-produccion).

{% hint style="warning" %}
**Un módulo del catálogo no es automáticamente un despiece validado.** Si aparece el aviso de módulo no verificado, comprueba las medidas y piezas antes de decidir si continúas. La revisión debe repetirse en el [Reporte de Producción](reporte-de-produccion/README.md).
{% endhint %}

Una vez todo listo, puede agregar el mueble a su archivo de Producción:

<figure><img src=".gitbook/assets/image (12) (1) (1) (1) (1) (1).png" alt=""><figcaption></figcaption></figure>

<figure><img src=".gitbook/assets/image (13) (1) (1) (1) (1).png" alt=""><figcaption></figcaption></figure>

Al agregar el mueble, sale este mensaje, si el mueble aún no ha sido verificado por un técnico dentro de su empresa, le va a informar esta advertencia para que sepa que debe revisar el resultado, hacer clic en <mark style="color:$primary;">**Sí**</mark> para continuar.

Lo siguiente es colocarle un nombre al mueble que está agregando, este nombre debe ser correspondiente a las especificaciones del mueble o el diseño:

<figure><img src=".gitbook/assets/image (6) (1) (1) (1) (1) (1) (1) (1) (1).png" alt=""><figcaption></figcaption></figure>

<figure><img src=".gitbook/assets/image (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1).png" alt=""><figcaption></figcaption></figure>

Mensaje de éxito si todo salió bien y el mueble se ha agregado a su archivo de producción.

En este punto, comprueba en la carpeta del proyecto que se incorporaron los archivos esperados del mueble y, si corresponde, los de herrajes. Luego abre el [Reporte de Producción](reporte-de-produccion/README.md) para contrastar el listado final con el diseño:

<figure><img src=".gitbook/assets/image (2) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1).png" alt=""><figcaption></figcaption></figure>

## <mark style="color:$primary;">**Este proceso lo repites por cada mueble que necesitas agregar desde el Catálogo de Módulos.**</mark>

## Otras herramientas del Catálogo de Módulos

<figure><img src=".gitbook/assets/image (45).png" alt=""><figcaption></figcaption></figure>

Si ha seleccionado un mueble y desea agregar mas de una unidad del mismo, puede multiplicar sus cantidades desde aquí. También lo puede hacer manualmente.

**Control de cantidades:** diferencia el número de **módulos** solicitados del número de **piezas** por módulo. Después de multiplicar, comprueba las cantidades finales de cada pieza y de los herrajes asociados antes de agregar la producción; no deduzcas el número de muebles únicamente del total de filas.

<figure><img src=".gitbook/assets/image (46).png" alt=""><figcaption></figcaption></figure>

Para imprimir el muele seleccionado, se genera un documento de excel tipo ficha del mueble con su imagen y lista de piezas y herrajes.

<figure><img src=".gitbook/assets/image (47).png" alt=""><figcaption></figcaption></figure>

### Ensayo reproducible: ficha Excel frente al Reporte de Producción

La opción anterior permite generar una **ficha Excel del mueble con su imagen y las listas de piezas y herrajes**. Antes de entregar esa ficha al taller, comprueba que corresponde a la misma configuración incorporada a producción. **No supongas que una ficha ya guardada se actualiza al cambiar el módulo o volver a generar el RP.**

{% hint style="warning" %}
**Realiza el ensayo con una copia identificada del proyecto.** Conserva el archivo de producción y las fichas originales sin sobrescribirlos; no alteres una definición pública o compartida para ejecutar la prueba.
{% endhint %}

1. **Identifica el punto de partida.** Registra versión instalada, cliente, ambiente, referencia del trabajo, módulo seleccionado, sus dimensiones y materiales, y la cantidad de módulos que vas a incorporar.
2. **Obtén la ficha A.** Con una unidad del módulo, genera la ficha Excel desde la opción documentada. Guárdala como evidencia diferenciada y comprueba que el archivo puede abrirse; registra la fecha de generación.
3. **Contrasta la producción A.** Incorpora ese módulo al archivo de prueba y consulta las piezas y herrajes en el [Reporte de Producción](reporte-de-produccion/README.md) y, si corresponde, en los [archivos generados](reporte-de-produccion/archivos-de-reportes-generados.md). Anota las cantidades y propiedades efectivamente visibles, sin presumir que todos los campos figuren en la ficha.
4. **Prepara una segunda versión controlada.** En otra copia del trabajo, utiliza la opción documentada para multiplicar la cantidad del mismo módulo y genera una nueva ficha Excel **B**, si la opción lo permite. Identifica la nueva producción por separado para evitar sumar accidentalmente ambas versiones.
5. **Concilia A y B.** Comprueba que los cambios de cantidades se reflejen en el contenido correspondiente del RP y de cada ficha; vuelve a comparar identidad, piezas y herrajes. Si un dato no aparece en la ficha, indícalo como **no visible** y verifica su valor en el documento que sí lo contiene.
6. **Decide qué se entrega.** Si una ficha no coincide con la producción aprobada o no puedes acreditar su versión, sepárala de los documentos válidos y no la utilices como orden de fabricación.

| Elemento que se compara | Evidencia de control |
| --- | --- |
| **Identidad** | Cliente, ambiente, nombre o código del módulo y versión A/B identificada en el registro del ensayo. |
| **Geometría y material** | Medidas, espesor y material de cada pieza que sean visibles en ambos documentos; los campos ausentes se anotan, no se suponen. |
| **Cantidades** | Unidades de módulo, piezas por tipo y total correspondiente a la versión A o B, sin mezclar las dos producciones. |
| **Herrajes** | Referencia y cantidades de los herrajes visibles en la ficha frente al detalle disponible de la producción. |
| **Archivo entregado** | Nombre, fecha y versión de la ficha utilizada, contrastados con el RP autorizado para fabricar. |

**Criterio del ensayo:** **CONFORME** si la identidad, los datos comparables y las cantidades concuerdan y quedan identificados los campos no visibles; **NO CONFORME** si hay una diferencia sin resolver o no puedes determinar qué ficha corresponde al RP; **NO EJECUTADO** si faltan los archivos o no se efectuó la comparación. El ensayo es un procedimiento de verificación documental, **no una prueba funcional Windows realizada en esta página**.


Si le ha creado un código al mueble, puede buscar directamente por su código.

<figure><img src=".gitbook/assets/image (48).png" alt=""><figcaption></figcaption></figure>

Desde aquí también puede ampliar la Descripción o crearla si aún no la tenía.

[← Portada del Curso](README.md) · [Creación de Módulos](creacion-de-modulos.md) · [Reporte de Producción](reporte-de-produccion/README.md) · [🏠 Portal principal](https://danielmelendez-pma.github.io/cabinet-report-partners/)
