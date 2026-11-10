# Reporte de Producción

**Curso de Cabinet Report · Guía detallada de la ventana**

Esta lección recorre las áreas de trabajo del Reporte de Producción, sus opciones de edición, revisión y generación. Las capturas originales se muestran en secuencia vertical para facilitar la consulta desde diferentes pantallas.

**Otras lecciones del proceso:** [Opciones para abrir un reporte](README.md) · [Parámetros de producción](parametros-de-produccion.md) · [Revisión de tableros y cantos](revision-de-tableros-y-cantos.md) · [Archivos generados](archivos-de-reportes-generados.md).

## Encuentra la tarea que necesitas

Esta página es una **guía de consulta de la ventana**, no una lista de acciones que debas ejecutar siempre en el mismo orden. Puedes ir directamente al control que necesitas y volver al [índice de entradas al RP](README.md) si aún no has abierto una producción.

| Necesitas… | Consulta… |
| --- | --- |
| Identificar un trabajo y localizar sus piezas | [Datos del cliente](#datos-del-cliente) y [Listado de piezas](#listado-de-piezas) |
| Corregir, agrupar, duplicar o cambiar medidas | [Herramientas de edición](#herramientas-para-editar-el-reporte-de-producción) |
| Cambiar cantidades o trasladar piezas | [Multiplicar o dividir](#multiplicar-o-dividir-producción) y [Mover piezas entre vistas](#mover-piezas-de-módulos-a-piezas-sueltas) |
| Revisar complementos del trabajo | [Perfilería](#gestión-de-perfilería) y [Herrajes](#gestión-de-herrajes) |
| Preparar la salida RP y atender avisos | [Generar producción](#generar-producción) y [Revisiones automáticas](#revisiones-automáticas-y-filtros-de-errores) |
| Completar la revisión de materiales y el corte | [Revisar aglomerados](#revisar-aglomerados), [Revisar cantos](#revisar-cantos) y [Optimizar producción](#optimizar-producción) |

## Secuencia de trabajo de esta ventana

1. **Identificar el trabajo:** confirma cliente, ambiente, referencia y datos del diseño.
2. **Revisar el despiece:** comprueba módulos, piezas sueltas, cantidades, medidas, tableros, vetas y cantos; realiza las correcciones necesarias.
3. **Preparar la generación:** revisa los parámetros y ejecuta las comprobaciones disponibles antes de crear los archivos RP.
4. **Completar las revisiones posteriores:** verifica tableros y cantos en sus secciones correspondientes.
5. **Optimizar y comprobar las salidas:** selecciona los parámetros y formatos de optimización, y contrasta los archivos resultantes con la producción revisada.

{% hint style="info" %}
**Distingue los controles:** el [control preliminar de tableros y cantos](#control-de-optimización-de-tableros-y-cantos) ofrece una consulta de materiales antes de generar; **Generar Producción** crea el RP en el recorrido documentado, mientras que **Optimizar Producción** prepara después los archivos para corte y otras salidas según las opciones elegidas. Cada resultado debe comprobarse por separado.
{% endhint %}

Las capturas reflejan el recorrido histórico de la interfaz. Si los nombres o la posición de los controles difieren de tu versión instalada, verifica la función equivalente antes de continuar; no interpretes todas las capturas como una única pantalla actual.

{% hint style="warning" %}
**Antes de generar o fabricar:** verifica manualmente medidas, cantidades, materiales, cantos y piezas. Las alertas automáticas ayudan a detectar inconsistencias, pero no sustituyen la comprobación técnica.
{% endhint %}

<figure><img src="../.gitbook/assets/image (10) (1) (1).png" alt="Vista general histórica de la ventana Reporte de Producción"><figcaption>Ubica las áreas de trabajo antes de modificar el despiece.</figcaption></figure>

Y llegó el momento de conocer el Corazón de Cabinet Report, el **Reporte de Producción**, el lugar donde el usuario pasará más tiempo revisando y organizando su producción, dándole forma y validando antes de generar los reportes.

---
## Recorrido por las partes de la ventana
## Logo
<figure><img src="../.gitbook/assets/image (1) (1) (1) (1) (1) (1) (1).png" alt="Área del logotipo de empresa en el Reporte de Producción"></figure>

Aquí aparecerá el logo de su empres si lo desea, para que se sienta más familiarizado y sus reportes se impriman con su imagen.

Al hacer clic encima te sale la opción de cambiar la imagen y poder seleccionar tu logo. 

<figure><img src="../.gitbook/assets/image (2) (1) (1) (1) (1).png" alt="Opción para seleccionar o cambiar el logotipo de empresa"></figure>

---
## Datos del cliente
<figure><img src="../.gitbook/assets/image (3) (1) (1) (1) (1).png" alt="Campos de identificación del cliente, ambiente, referencia y dibujante"><figcaption>Confirma la identidad del trabajo al comenzar la revisión.</figcaption></figure>

En esta sección debe colocar los datos de:

* **Cliente:** Nombre del cliente final, al que se le está fabricando los muebles.
* **Ambiente:** Nombre de la producción, si es Cocina, Baño, Closet u otro ambiente.
* **Referencia:** Alguna información adicional, dirección, modelo, proyecto, etc.
* **Dibujante:** Nombre del Dibujante que participó en los diseños, información importante para que los operarios, instaladores, inspectores sepan a quién hacerle alguna consulta del diseño.

<figure><img src="../.gitbook/assets/image (4) (1) (1) (1) (1).png" alt="Controles para modificar los datos de identificación de la producción"></figure>

Puede cambiar estos datos del cliente desde aquí

Por los nuevos datos que desee colocar 

<figure><img src="../.gitbook/assets/image (5) (1) (1) (1) (1).png" alt="Vista de los datos del cliente después de modificarlos"></figure>

---
## Listado de piezas
Lugar donde se muestra toda la lista de piezas:

<figure><img src="../.gitbook/assets/image (6) (1) (1) (1).png" alt="Listado de piezas agrupadas por módulos y piezas sueltas"><figcaption>Comprueba por separado módulos, piezas sueltas y cantidades.</figcaption></figure>

En la interfaz documentada se puede alternar la vista entre **módulos** y **piezas sueltas**. Comprueba en cuál de las dos estás antes de editar.

<figure><img src="../.gitbook/assets/image (7) (1) (1) (1).png" alt="Vista de selección entre módulos y piezas sueltas"></figure>

Puede agregar nuevas piezas al módulo seleccionado o a la lista de Piezas Sueltas desde la sección inferior:

<figure><img src="../.gitbook/assets/image (8) (1) (1) (1).png" alt="Campos de ingreso de piezas en el Reporte de Producción"></figure>

Sólo coloque los valores y las agrega con el botón **(+)**.

---
## Conteo de piezas y número RP
<figure><img src="../.gitbook/assets/image (9) (1) (1) (1).png" alt="Indicadores de conteo de piezas y control del reporte RP"><figcaption>Controla los totales y el número de referencia del RP.</figcaption></figure>

Cabinet Report de manera automática te hace un conteo de piezas:

* **Total Items:** es la cantidad de filas que contienen la lista de Módulos y de Piezas Sueltas
* **Total Piezas:** es la cantidad de sumas de piezas en total de la producción
* **Múltiplo de Producción:** es el indicador que estas trabajando con cantidades de Ejemplo: para 1 casas, 2 casas, etc.

Estos indicadores ayudan a controlar las cantidades. Después de multiplicar, dividir o mover piezas, compara el total previsto con el resultado mostrado.

Además, Cabinet Report le asigna un número de control a tu Reporte RP, importante para poder llevar un control y métricas más adelante.

---
## Herramientas para editar el Reporte de Producción
<figure><img src="../.gitbook/assets/image (10) (1) (1) (1).png" alt="Control de agrupación de piezas de características coincidentes"><figcaption>Agrupa únicamente piezas que realmente sean equivalentes.</figcaption></figure>

La herramienta permite agrupar filas con piezas de características coincidentes. **Verifica también material, orientación y la pertenencia al módulo** antes de consolidarlas; nombres y medidas iguales no prueban por sí solos que dos piezas sean intercambiables.

Ejemplo si tienes:

1 COSTADO 15X580X780

1 COSTADO 15X580X780

agruparla en:

2 COSTADO 15X580X780

<figure><img src="../.gitbook/assets/image (11) (1) (1).png" alt="Ejemplo visual de piezas agrupadas y sus cantidades"></figure>

Si quieres que Cabinet Report Invierta las medidas con un solo clic en cada pieza que necesites.

<figure><img src="../.gitbook/assets/image (12) (1) (1).png" alt="Control para intercambiar las dimensiones de una pieza"><figcaption>Comprueba veta y cantos antes de invertir ancho y largo.</figcaption></figure>

En la interfaz documentada, el icono de las dos flechas intercambia ancho y largo. **Antes de aplicar el cambio**, revisa la orientación, la veta y los cantos; intercambiar medidas no demuestra por sí solo que la pieza admita giro.

---
<figure><img src="../.gitbook/assets/image (57).png" alt="Referencia visual de la edición de orientación o dimensiones de piezas"></figure>

Si quieres eliminar todos los cantos de la producción con un solo clic.

<figure><img src="../.gitbook/assets/image (58).png" alt="Opción de eliminación de cantos en la producción"></figure>

Si necesitas buscar una pieza, canto, tablero o medida, solo escribe aquí y haciendo clic en la lupa puedes saltar de resultado en resultado.

---
Con la opción de **Filtrar Aglomerado**, puedes reducir la lista de tableros si necesitas buscar un tablero para cambiar el existente:

<figure><img src="../.gitbook/assets/image (60).png" alt="Filtro de aglomerados para localizar un tablero del reporte"></figure>

<figure><img src="../.gitbook/assets/image (61).png" alt="Listado de tableros al utilizar el filtro de aglomerados"></figure>

Al reemplazar un tablero, revisa si la opción de aplicación masiva está activada. **Comprueba todas las filas afectadas** para evitar asignar un material equivocado a piezas con medidas similares.

<figure><img src="../.gitbook/assets/image (62).png" alt="Controles de reemplazo de tablero y aplicación de cambios"><figcaption>Revisa el alcance de cualquier reemplazo de tablero.</figcaption></figure>

Al reemplazar un canto, revisa si se aplicará a una pieza o a múltiples coincidencias. **Confirma los lados, colores y espesores afectados** antes de guardar los cambios.

Pero si no quieres que Cabinet Report haga los procesos automáticos, simplemente desmarca la opción en la parte superior derecha de la ventana de Reporte de Producción y tú tendrás el control de todos los cambios sin automatización:

<figure><img src="../.gitbook/assets/image (63).png" alt="Configuración de automatizaciones durante la edición del reporte"></figure>

---
Al hacer clic al nombre de un módulo, Cabinet Report te pregunta si quieres intentar cambiar el nombre o duplicar el modulo:

<figure><img src="../.gitbook/assets/image (64).png" alt="Opciones disponibles al seleccionar el nombre de un módulo"><figcaption>Verifica el módulo seleccionado antes de cambiarlo o duplicarlo.</figcaption></figure>

<figure><img src="../.gitbook/assets/image (65).png" alt="Diálogo de las acciones de cambiar nombre o duplicar un módulo"></figure>

**Cambiar el nombre:** Te permite hacer un cambio en el nombre del módulo, y Cabinet Report hace el cambio para cada una de las piezas que corresponde a este mueble.

**Duplicar Módulo:** Te permite crear otro módulo igual, a partir de un módulo existente, duplicándolo directo en el Reporte de Producción.

<figure><img src="../.gitbook/assets/image (66).png" alt="Resultado visual de la acción de duplicar un módulo"></figure>

---
## Gestión de piezas enchapadas
Si tu producción cuenta con piezas enchapadas, Cabinet Report te ayuda a Gestionarlas,

Para eso debes agregar la palabra ENCHAPA, seguido de (-) y el número de piezas que se debe enchapar (ENCHAPA-#).

**Ejemplo:**

1 TABLILLA ENCHAPA-2 15X300X900, quiere decir que necesitas enchapar 2 tablillas de 15mm para lograr una tablilla de 30mm

<figure><img src="../.gitbook/assets/image (71).png" alt="Ejemplo histórico de gestión de una pieza marcada para enchape"><figcaption>Comprueba las piezas marcadas para enchape y su cantidad.</figcaption></figure>

Te revisa antes de Generar la producción si quieres incrementar las medidas de las piezas enchapadas en caso de que lo necesites y no lo consideraste. Al indicarle que (Si), lo hace automático por ti.

Y te devuelve el resultado:

<figure><img src="../.gitbook/assets/image (72).png" alt="Resultado o aviso del tratamiento de piezas enchapadas"></figure>

---
## Multiplicar o dividir producción
Si necesita multiplicar la producción que actualmente tiene por 1 casa y va a fabricar 5 casas, no necesita sacar la calculadora y cambiar manualmente pieza por pieza, Cabinet Report hace el trabajo por ti, haciendo clic en:

<figure><img src="../.gitbook/assets/image (79).png" alt="Herramienta para multiplicar o dividir cantidades de producción"><figcaption>Concilia las unidades antes y después de multiplicar o dividir.</figcaption></figure>

Colocando solo la cantidad y hacer un clic en Multiplicar o también Dividir

<figure><img src="../.gitbook/assets/image (80).png" alt="Control para introducir el factor de multiplicación o división"></figure>

---
## Fichas de tableros
Si no esta seguro de cómo son las vetas de uno de los tableros de la producción, o quiere ver si tiene o no vetas o su tamaño, con el botón de **Ver Ficha del Aglomerado** puede visualizarlo

<figure><img src="../.gitbook/assets/image (81).png" alt="Acceso a la ficha de un tablero utilizado en la producción"></figure>

La imagen se muestra siempre que la haya agregado al crear el tablero.

<figure><img src="../.gitbook/assets/image (83).png" alt="Vista de la imagen o información asociada a una ficha de tablero"></figure>

---
## Mover piezas de módulos a piezas sueltas

Si quiere que varias piezas de un módulo se fabriquen como piezas sueltas independientes, solo debe seleccionar el grupo de piezas.

<figure><img src="../.gitbook/assets/image (84).png" alt="Selección de piezas de un módulo antes de moverlas"><figcaption>Registra el origen antes de mover piezas del módulo.</figcaption></figure>

Después de seleccionadas haga clic en **Mover Piezas**.

Las piezas seleccionadas se muestran en la siguiente ventana:

<figure><img src="../.gitbook/assets/image (86).png" alt="Ventana de revisión de las piezas seleccionadas para mover"></figure>

Luego de revisadas las piezas, haga clic en Mover

Y si todo sale bien, Cabinet Report le avisa que las piezas ya se encuentran en la lista de piezas sueltas.

<figure><img src="../.gitbook/assets/image (87).png" alt="Confirmación de un traslado de piezas a piezas sueltas"></figure>

Piezas movidas a piezas sueltas:

<figure><img src="../.gitbook/assets/image (88).png" alt="Listado de piezas sueltas después del traslado desde un módulo"></figure>

---
## Mover piezas sueltas a un módulo

Si hay un grupo de piezas en la lista de piezas sueltas pero en realidad pertenecen a un módulo o forman un módulo, puede moverlas seleccionandolas y haciendo clic en **Mover Piezas**.

<figure><img src="../.gitbook/assets/image (89).png" alt="Selección de piezas sueltas para incorporarlas a un módulo"><figcaption>Comprueba el módulo de destino al devolver piezas sueltas.</figcaption></figure>

Se muestra la lista de piezas, después de hacer clic en Mover te muestra la lista de muebles para seleccionar a cuál módulo la quieres mover o colocar el nombre del módulo nuevo que quieres crear con esas piezas:

<figure><img src="../.gitbook/assets/image (90).png" alt="Selección del módulo de destino al mover piezas sueltas"></figure>

Y si todo sale bien, Cabinet Report te avisa que el proceso se completó

<figure><img src="../.gitbook/assets/image (92).png" alt="Mensaje de resultado de traslado de piezas a un módulo"></figure>

<figure><img src="../.gitbook/assets/image (91).png" alt="Vista del módulo y las piezas después de la transferencia"></figure>

---

## Ensayo reproducible: mover piezas sin perder ni duplicar cantidades

Este ensayo de **control documental** comprueba la transferencia entre **módulos** y **piezas sueltas** descrita arriba. No es una prueba automatizada del programa ni una autorización para fabricar.

### Prepara un caso de prueba

1. Trabaja con una **copia identificada de la producción** y conserva el origen sin cambios. Anota cliente, ambiente, referencia, número RP (si existe) y fecha de la comprobación.
2. Elige un módulo de prueba con **al menos cuatro filas de piezas** y una fila cuya cantidad sea **1**. De este modo podrás revisar tres filas restantes sin confundir el ensayo con la reorganización de un módulo pequeño.
3. Registra antes del movimiento las filas del módulo y de piezas sueltas. Para la pieza seleccionada, anota nombre, cantidad, espesor, ancho, largo, tablero/material, veta y canto de cada lado; incorpora código o identificador si aparece en tu vista.
4. Anota el **total físico de unidades de pieza**: suma de cantidades del módulo de prueba y de la lista de piezas sueltas. No utilices el número de filas ni el total de módulos como sustituto de esa suma.

### Ejecuta la transferencia y el retorno

1. En el módulo de prueba, selecciona **solo la fila registrada** y utiliza **Mover Piezas**, siguiendo las pantallas del apartado anterior. Verifica la selección antes de confirmar.
2. Abre **Piezas Sueltas** y localiza la pieza transferida. Compárala campo por campo con el registro inicial; comprueba además que no permanezca otra unidad no justificada en el módulo de origen.
3. Vuelve a contar las unidades de pieza del módulo y de piezas sueltas. La cantidad trasladada debe **restarse del origen y aparecer en destino**, sin cambiar el total conjunto. Comprueba también las filas no seleccionadas.
4. Desde **Piezas Sueltas**, selecciona esa pieza y utiliza **Mover Piezas** para devolverla al módulo original, conforme al apartado siguiente. Verifica el módulo de destino antes de confirmar.
5. Compara el estado final con el inicial: pertenencia al módulo, cantidades, dimensiones, espesor, material, veta y cuatro cantos. Si el sistema presenta identificadores, registra cualquier diferencia para su revisión; **no presupongas** que una transferencia conserva el identificador interno.

### Evidencias y criterios de resultado

| Comprobación | Resultado esperado |
| --- | --- |
| Salida del módulo | La unidad seleccionada deja de contabilizarse en el origen. |
| Entrada a piezas sueltas | La misma unidad queda visible en destino con sus propiedades técnicas. |
| Cantidad total | La suma de cantidades entre ambas vistas no aumenta ni disminuye por el traslado. |
| Piezas no seleccionadas | Sus cantidades y propiedades se mantienen. |
| Retorno al módulo | La pieza queda asignada al módulo previsto y el estado técnico vuelve a coincidir con el inicial. |

Registra el resultado como **CONFORME** si las cinco comprobaciones se verifican; **NO CONFORME** si aparece una pérdida, duplicación, alteración técnica o destino incorrecto; **NO EJECUTADO** si no se realizó el ejercicio o no se dispone de evidencias suficientes.

{% hint style="warning" %}
**Si hay una discrepancia:** detén la generación y el envío a corte, conserva capturas y totales de ambos estados y recupera únicamente una **copia previamente comprobada**. No supongas que el mensaje de éxito equivale a integridad, que existe un deshacer automático o que mover piezas conserva por sí solo todos los metadatos y herrajes asociados.
{% endhint %}

Para continuar el control antes de fabricación, consulta [Revisión de Tableros y Cantos](revision-de-tableros-y-cantos.md) y [Archivos de Reportes Generados](archivos-de-reportes-generados.md).

---

## Gestión de perfilería
Desde Reporte de Producción puedes agregar la perfilería ZÓCALOS, TUBOS, GOLA, para que todo vaya dentro del reporte

### Zócalos

<figure><img src="../.gitbook/assets/image (18).png" alt="Sección de zócalos dentro de la gestión de perfilería"><figcaption>Incorpora solo los zócalos correspondientes al trabajo.</figcaption></figure>

### Tubos

<figure><img src="../.gitbook/assets/image (1) (1) (1) (1) (1) (1).png" alt="Sección de tubos dentro de la gestión de perfilería"></figure>

### Golas

<figure><img src="../.gitbook/assets/image (3) (1) (1) (1).png" alt="Sección de golas dentro de la gestión de perfilería"></figure>

En cada uno puedes agregar **seleccionando** el perfil de la lista y haciendo clic en **Ingresar (+)**, colocas la medida y **Aceptar**.

---
## Gestión de herrajes
Gestiona los Accesorios, Ferretería de Montaje, Ferretería de Instalación para la producción que estás trabajando

### Accesorios

<figure><img src="../.gitbook/assets/image (4) (1) (1) (1).png" alt="Sección de accesorios en la gestión de herrajes"><figcaption>Concilia accesorios y cantidades con el diseño aprobado.</figcaption></figure>

### Ferretería de Montaje

<figure><img src="../.gitbook/assets/image (5) (1) (1) (1).png" alt="Sección de ferretería de montaje de la producción"></figure>

### Ferretería de Instalación

<figure><img src="../.gitbook/assets/image (6) (1) (1).png" alt="Sección de ferretería de instalación de la producción"></figure>

---
## Control de optimización de tableros y cantos

Antes de generar los reportes RP, puedes saber cuánto se está consumiendo en laminas de aglomerado y metrajes de canto haciendo clic en este botón

<figure><img src="../.gitbook/assets/image (7) (1) (1).png" alt="Acceso al control preliminar de tableros y cantos"><figcaption>Este control preliminar no reemplaza la revisión del despiece.</figcaption></figure>

Y de manera automática mostrarte las cantidades

Te muestra la lista de tableros actuales, te pregunta que algoritmo y parametros de optimizacion utilizarás:

<figure><img src="../.gitbook/assets/image (8) (1) (1).png" alt="Selección de parámetros o algoritmo en el control de materiales"></figure>

### Optimización

<figure><img src="../.gitbook/assets/image (9) (1) (1).png" alt="Resultado visual del control preliminar de optimización"></figure>

---
## Generar producción
Una vez revisado y estando listo para generar el Reporte de Producción RP, hacer clic al botón **Generar Producción**.

<figure><img src="../.gitbook/assets/image (73).png" alt="Botón Generar Producción del Reporte de Producción"><figcaption>Genera el RP solo después de revisar los datos de producción.</figcaption></figure>

En el recorrido documentado, cuando la generación pasa las comprobaciones correspondientes, se muestra la selección del destino del archivo RP. Verifica la ubicación elegida y comprueba luego que el archivo se haya generado con el contenido previsto.

<figure><img src="../.gitbook/assets/image (77).png" alt="Selección del destino para guardar el archivo RP generado"><figcaption>Comprueba el archivo creado en la ubicación seleccionada.</figcaption></figure>

Si alguna comprobación encuentra una inconsistencia, la aplicación puede presentar alertas. **La ausencia de alertas no significa que todas las medidas, materiales o fórmulas sean correctos**; mantén la revisión manual.

---
## Revisiones automáticas y filtros de errores
Revisión automática si una pieza excede de la medida del tablero en ancho y en largo.

<figure><img src="../.gitbook/assets/image (67).png" alt="Advertencia histórica al detectar una pieza que excede el tablero"><figcaption>Las advertencias automáticas no sustituyen la inspección manual.</figcaption></figure>

---
<figure><img src="../.gitbook/assets/image (68).png" alt="Captura complementaria de la comprobación de medidas del tablero"></figure>

Revisión automática si el espesor de una pieza no coincide con el espesor del tablero.

Detecta error si quieres enchapar unas piezas pero no escribiste bien la frase ENCHAPA.

<figure><img src="../.gitbook/assets/image (69).png" alt="Alerta histórica relacionada con la escritura de ENCHAPA"></figure>

<figure><img src="../.gitbook/assets/image (70).png" alt="Alerta relacionada con la cantidad de piezas para enchapar"></figure>

Si vas a enchapar 2 piezas y solo colocas a fabricar 1, te detecta y te informa que deben ser 2 piezas para poder enchaparla.

Una captura histórica muestra un aviso relacionado con cantos de **2 mm** y la reducción automática de piezas. **No se debe deducir de esta captura el umbral exacto del algoritmo**: la lección de [Parámetros de Producción](parametros-de-produccion.md) conserva una discrepancia pendiente entre la opción «Mayor a 2 (>2)» y ese ejemplo. Confirma el comportamiento con una prueba de tu versión antes de aplicarlo.

<figure><img src="../.gitbook/assets/image (78).png" alt="Aviso histórico de comprobación de cantos de 2 milímetros"><figcaption>No deduzcas de esta imagen el umbral exacto de reducción por canto.</figcaption></figure>

---
## Observaciones
Espacio donde puede colocar observaciones dirigidas al aquipo de producción o inspección:

<figure><img src="../.gitbook/assets/image (11) (1).png" alt="Campo de observaciones de la producción"><figcaption>Las observaciones deben ser claras para fabricación e inspección.</figcaption></figure>

---
## Recargar producción
Si necesitas hacer un cambio y ya has generado el RP, no te va a permitir hacer cambios, para eso debes hacer clic en el botón **Recargar Producción**.

<figure><img src="../.gitbook/assets/image (75).png" alt="Control para recargar una producción generada"><figcaption>Comprueba la producción correcta antes de recargarla.</figcaption></figure>

<figure><img src="../.gitbook/assets/image (76).png" alt="Vista complementaria del proceso de recarga de producción"></figure>

---
## Revisar aglomerados
En el recorrido de generación documentado, después se utiliza **Revisar Aglomerados** para comprobar la clasificación de los tableros. Antes de avanzar, comprueba que los materiales de la producción sean los esperados.

<figure><img src="../.gitbook/assets/image (10) (1).png" alt="Sección Revisar Aglomerados del Reporte de Producción"><figcaption>Revisa los tableros detectados y sus referencias.</figcaption></figure>

Hacer clic aquí para desplegar los tableros.

Una vez activado, se desplegará la lista de tableros que componen la producción actual y debe seleccionar de las opciones a que parte del mueble corresponde cada tablero:

<figure><img src="../.gitbook/assets/image (12) (1).png" alt="Listado de tableros durante la revisión de aglomerados"></figure>

---
## Revisar cantos
<figure><img src="../.gitbook/assets/image (14) (1).png" alt="Sección Revisar Cantos del Reporte de Producción"><figcaption>Confirma los cantos y su correspondencia con el despiece.</figcaption></figure>

Hacer clic aquí para desplegar los cantos.

Después de comprobar los tableros, utiliza **Revisar Cantos** para verificar los materiales de canto y su clasificación. Revisa las asignaciones antes de optimizar.

Una vez activado, se desplegará la lista de cantos que componen la producción actual y debe seleccionar de las opciones a que parte del mueble corresponde cada canto:

<figure><img src="../.gitbook/assets/image (15) (1).png" alt="Listado de cantos durante la revisión de materiales"></figure>

---
## Optimizar producción
Es momento de completar los reportes y iniciar el proceso de Optimización de la Producción

<figure><img src="../.gitbook/assets/image (16) (1).png" alt="Acceso a la función Optimizar Producción"><figcaption>La optimización es una etapa distinta de la generación del RP.</figcaption></figure>

Hacer clic aquí para iniciar

<figure><img src="../.gitbook/assets/image (17).png" alt="Control para iniciar la optimización de la producción"></figure>

Si llegado a este punto, y activa **Optimizar Producción** y algún proceso no se completó, Cabinet Report le enviará este mensaje

La optimización requiere completar los procesos previos previstos por la interfaz. La aplicación puede ejecutar controles de consistencia y mostrar un mensaje al finalizar; **no presupongas que detecta todos los duplicados o faltantes**. Contrasta los archivos generados con el despiece antes de enviarlos a fabricación:

<figure><img src="../.gitbook/assets/image (5) (1).png" alt="Mensaje de comprobaciones pendientes antes de optimizar"></figure>

### Parámetros de optimización

En la ventana de optimización puedes elegir el algoritmo disponible. La documentación histórica menciona **Guillotina** como opción recomendada; su conveniencia depende del tablero, la máquina y las restricciones del corte.

También colocar el espesor de la sierra para que se tome en cuenta para el cálculo de material.

Si se ofrece el giro de piezas para materiales sin veta, verifica que la orientación y las restricciones de cada pieza permitan girarla. Un tablero sin veta no elimina las demás condiciones de fabricación.

Por último coloca el grosor de resane que desea que se tome en cuenta al calcular los tableros.

<figure><img src="../.gitbook/assets/image (1) (1) (1) (1) (1).png" alt="Parámetros de optimización de tableros y condiciones de corte"><figcaption>Verifica algoritmo, espesor de sierra, giro y resane según tu trabajo.</figcaption></figure>

Si todo está listo, haga clic en **Optimizar**.

### Seleccione el Optimizador de Su Seccionadora

<figure><img src="../.gitbook/assets/image (2) (1) (1).png" alt="Selección del optimizador de la seccionadora y archivos de salida"><figcaption>Elige el formato de salida compatible con la seccionadora.</figcaption></figure>

En este punto, se seleccionan todos los archivos que se van a generar para su producción.

Cabinet Report automáticamente selecciona los que ha detectado que tienen contenido.

Seleccione el **Software de Optimización** de su seccionadora para que se generen los archivos de corte de manera automática.

Cuanto tenga el Optimizador seleccionado, haga clic en **Generar**.

Al finalizar, verifica el mensaje de resultado **y abre los archivos generados**. Comprueba totales, dimensiones, tableros, cantos y formatos de salida según el optimizador seleccionado.

Consulta la lección [Archivos de Reportes Generados](archivos-de-reportes-generados.md) para identificar cada salida.

<figure><img src="../.gitbook/assets/image (3) (1) (1).png" alt="Pantalla o mensaje de resultado al generar los archivos optimizados"><figcaption>Abre los archivos resultantes y verifica su contenido antes de fabricar.</figcaption></figure>

---

[← Revisión de tableros y cantos](revision-de-tableros-y-cantos.md) · [Archivos de reportes generados →](archivos-de-reportes-generados.md) · [Índice del Reporte de Producción](README.md) · [🏠 Portal principal](https://danielmelendez-pma.github.io/cabinet-report-partners/)
