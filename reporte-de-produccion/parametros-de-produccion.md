# Parámetros de Producción

Antes de importar un archivo TXT o CSV, revisa las opciones de vetas, automatizaciones, packing list y el tipo de reporte que vas a preparar. Esta página describe las opciones de las capturas originales; la aplicación exacta de cada automatismo debe comprobarse con los materiales y la versión instalados.

Cada vez que va a abrir un archivo CSV o TXT, debe seleccionar las opciones de **Parámetros de Producción**, según las condiciones de los materiales y lo que va a fabricar:

<figure><img src="../.gitbook/assets/image (1) (1) (1) (1) (1) (1) (1) (1).png" alt=""><figcaption></figcaption></figure>

***

<figure><img src="../.gitbook/assets/image (3) (1) (1) (1) (1) (1).png" alt=""><figcaption></figcaption></figure>

## Vetas de Aglomerados

Seleccione los tipos de Vetas que manejará en su producción.

Importante y obligatorio para que Cabinet Report pueda ejecutar ciertos algoritmos durante el proceso.

***

## Automatizaciones

Active o desactive las automatizaciones de este listado según su necesidad.

Las que se mantengan activas, Cabinet Report las toma en cuenta para ejecutar ciertos algoritmos durante el proceso.

<figure><img src="../.gitbook/assets/image (5) (1) (1) (1) (1) (1).png" alt=""><figcaption></figcaption></figure>

Te explico que significa cada automatización:

**Ordenamiento de Piezas:** Cabinet Report te ordena las piezas para mantener siempre un formato y orden en la lista de piezas de cada módulo y todos tengan la misma secuencia ordenada.

**Redondeado de Medida:** si algún calculo de una medida está con puntos decimales, ejemplo: 100.5mm, Cabinet Report lo redondea a 101mm.

**Agrandar Piezas Ajustables:** si el usuario ingresa una pieza que se deba ajustar en obra por ejemplo RELLENO AJUSTABLE, Cabinet report le agranda la medida, si la pieza es de 60mm, la agranda a 90mm, para que en obra el instalador la corte a la medida que necesita.

**Activar Traducción Técnica:** Si quiere que sus piezas cambien de nombre a los nombres que su empresa maneja, puede agregar estos nombres y activando esta opción, Cabinet Report le cambia el nombre de manera automática durante la carga del archivo.

**Activar Repasado de Cantos Mayor a 2 (>2):** Cabinet Report le reduce a cada pieza la medida que el usaurio le indique, para que el operador de la canteadora no tenga que reducir con la fresadora el espesor completo.

Ejemplo conservado de la guía original: si el canto es de 2 mm, se describe una reducción de 1 mm por lado para el repasado.

{% hint style="warning" %}
**Regla por comprobar:** el nombre de la opción dice **«Mayor a 2 (>2)»**, pero el ejemplo anterior usa exactamente **2 mm**. La documentación no permite determinar por sí sola si ese ejemplo se aplica a la condición del control. Antes de activar esta automatización, verifica el umbral y las medidas resultantes en la versión instalada. No se modifica aquí ninguna regla de cálculo.
{% endhint %}

**Aplicar Medidas Mínimas de Fascias:** si el usuario ingresa una pieza o fascia de 30mm, Cabinet Report de manera automática la agranda a 60mm para que así pase sin problemas por las máquinas de Corte y Canteo.

**Carga automática de Herrajes y Perfilerías:** al abrir el archivo TXT y la carpeta también contiene los archivos de herrajes, en lugar de que el usuario los cargue manualmente, Cabinet Report lo carga de manera automática.

Invertir medida de Piezas sin Vetas: si el usuario activa que la producción contiene material sin vetas, Cabinet Report arregla medidas de algunas piezas:

Ejemplos de orientación recogidos en el curso (no deben aplicarse como regla universal a todas las piezas):

PUERTA de 18X780X300 Cabinet Report la agrega a 18X300X780 sabiendo que primero debe colocar el ancho y luego la altura

FRENTE GAVETA de 18X300X600 Cabinet Report la agrega a 18X300X600 sabiendo que primero debe colocar el ancho y luego la altura

***

## Funcionalidad para Generar Packing List

<figure><img src="../.gitbook/assets/image (6) (1) (1) (1) (1).png" alt=""><figcaption></figcaption></figure>

Puede activar esta opción y Cabinet Report le agrega un archivo Packing List a su producción, listo para ser utilizado por su transportista y receptor de la producción en obra.

Tambien si ya tiene la producción generada y quiere agregarle el Packing List después, puede hacerlo haciendo clic en este boton

<figure><img src="../.gitbook/assets/image (7) (1) (1) (1) (1).png" alt=""><figcaption></figcaption></figure>

***

## Importar:

Antes de importar el TXT o CSV, debe seleccionar si es un RP Nuevo o va a Modificar un RP Existente:

<figure><img src="../.gitbook/assets/image (8) (1) (1) (1) (1).png" alt=""><figcaption></figcaption></figure>

RP Nuevo: Es una producción nueva que está generando.

RP Anterior: Es que va a aplicar un cambio a un RP que había sido generado previamente, para eso debe colocar el  número del RP y con esto Cabinet Report entiende que está haciendo cambios a una producción anterior.

Esta elección afecta la identificación del trabajo en el historial de producción. Si vas a modificar un RP anterior, comprueba su número y la correspondencia con el cliente y ambiente antes de abrir el archivo.

***

### Lista de comprobación antes de importar

1. Confirma el **cliente, ambiente y archivo de origen**.
2. Revisa **vetas y automatizaciones** según los materiales reales; las opciones activadas pueden modificar piezas o nombres durante la carga.
3. Selecciona **RP Nuevo** o **RP Anterior** y verifica el número del RP si estás recuperando una producción.
4. Tras importar, continúa con la [Revisión de Tableros y Cantos](revision-de-tableros-y-cantos.md) y contrasta las medidas antes de generar archivos.

Una vez cumplido lo anterior, puedes abrir el archivo correspondiente.

<figure><img src="../.gitbook/assets/image (54).png" alt=""><figcaption></figcaption></figure>


## Ensayo reproducible: verificar el efecto de las automatizaciones

Antes de usar un archivo importado para corte o canteo, comprueba **qué cambió realmente** al activar cada automatización. Esta prueba se centra en las **transformaciones por parámetros**; no sustituye las pruebas de compatibilidad de [Cargar TXT](cargar-txt.md) o [Cargar CSV](cargar-csv.md), ni valida por sí sola las fórmulas de las piezas.

### 1. Preparar una referencia y proteger la producción

1. Conserva intacto un **TXT generado por una versión compatible** o un **CSV exportado por el programa de origen** que ya hayas comprobado como importable. Trabaja con copias y un proyecto de ensayo, nunca sobre el RP aprobado para fabricar.
2. Anota versión instalada, formato y procedencia del archivo, cliente y ambiente de ensayo, modo de importación, configuración de vetas y **estado de todas las automatizaciones**. Para la prueba, elige **RP Nuevo**; no utilices «RP Anterior» para sobrescribir una producción real.
3. Selecciona una pieza o un grupo reducido cuyo dato de origen sea comprobable. Registra **módulo, pieza, cantidad, espesor, ancho, largo, material, veta y cantos por cada lado**, así como el plano o despiece autorizado. Si el archivo no contiene un caso que active la opción elegida, consigna **NO EVALUABLE**: no fabriques datos ni alteres columnas para forzar la prueba.
4. Identifica qué esperas observar *según la descripción histórica* de la opción, pero no conviertas esa descripción en garantía de comportamiento actual. Por ejemplo, esta página menciona el redondeo de **100.5 a 101 mm** y el agrandamiento de una pieza ajustable de **60 a 90 mm**; ambos resultados deben **comprobarse en la versión instalada** y contrastarse con el diseño aprobado.

### 2. Comparar dos importaciones controladas

1. **Ensayo A:** importa una copia del archivo con la automatización seleccionada **desactivada**. Registra la pieza y sus datos tal como aparecen en el RP después de importar.
2. **Ensayo B:** parte de **otra copia idéntica del mismo archivo de origen**, en un trabajo de ensayo independiente, con **solo esa automatización activada** y el resto de las opciones iguales. Registra el resultado sin editar manualmente las piezas entre ambas lecturas.
3. Compara **origen → A → B**, no únicamente los totales generales. Si cambia el número de piezas, el material, la orientación, la medida o el canto aplicado a un lado, identifica la pieza exacta y decide si la diferencia está autorizada.
4. Repite el ensayo **por separado** para cada automatización relevante. En particular, examina el redondeo, el agrandamiento de ajustables, la traducción técnica y la inversión de dimensiones en piezas sin veta *solo cuando existan casos verificables*. La carga automática de herrajes o perfilerías requiere además conciliar los **archivos complementarios**, no solo las piezas del RP.

| Campo de control | Fuente aprobada | Ensayo A: opción desactivada | Ensayo B: opción activada |
| --- | --- | --- | --- |
| Pieza, módulo y cantidad | Registrar identificación y unidades | Registrar lo observado | Registrar lo observado |
| Espesor, ancho y largo (mm) | Registrar dimensiones | Registrar las tres medidas | Registrar las tres medidas |
| Material y veta | Registrar referencia y orientación | Registrar lo observado | Registrar lo observado |
| Canto superior / inferior / derecho / izquierdo | Registrar cada borde | Registrar cada borde | Registrar cada borde |
| Parámetro y justificación del cambio | Opción y criterio de diseño | Desactivada | Activada; explicar cada diferencia |
| Evidencia | Nombre y copia del origen | RP/captura identificable | RP/captura identificable |

**Caso de contraste del redondeo:** si el archivo de ensayo contiene una medida original de **100.5 mm**, la descripción histórica indica **101 mm** al aplicar «Redondeado de Medida». Anota el resultado real de **A** y **B**; si difiere de esa referencia, no lo corrijas por suposición: documenta la diferencia y verifica la configuración o la versión antes de continuar.

{% hint style="warning" %}
**Umbral de repasado de cantos sin resolver:** esta prueba **no interpreta** «Mayor a 2 (>2)» como equivalente a un canto de 2 mm. El ejemplo de 2 mm y el nombre del control siguen discrepando. Si ese caso afecta la producción, determina el resultado en la aplicación y solicita validación técnica antes de aprobar una reducción de medidas.
{% endhint %}

### 3. Decisión y evidencia de liberación

- **APTO para continuar la revisión del RP:** la importación conserva identidad, cantidades, materiales, vetas y cantos esperados; cada cambio de medida o nombre está localizado, justificado contra el diseño y aprobado por el responsable. Todavía deben verificarse el [RP completo](reporte-de-produccion.md) y los [archivos generados](archivos-de-reportes-generados.md).
- **NO APTO:** hay cambios de dimensión, orientación, cantidad, material o borde sin explicación o sin aprobación. No generes ni entregues archivos para fabricación desde ese ensayo; corrige origen o parámetros y repite la comparación.
- **NO EVALUABLE:** falta un caso representativo, no se pudo mantener la misma configuración entre A y B o no se dispone de evidencia suficiente. No declares comprobada esa automatización.

Conserva las **dos configuraciones**, copias de entrada, resultados, diferencias detectadas, decisión, responsable y fecha. **Un ensayo correcto demuestra únicamente lo observado con ese archivo, opciones y versión**; no acredita otros importadores, reglas generales de corte ni la ejecución automática de estos controles por Cabinet Report.


---

[← Reporte en blanco](reporte-en-blanco.md) · [Opciones del Reporte de Producción](README.md) · [Revisión de tableros y cantos →](revision-de-tableros-y-cantos.md) · [🏠 Portal principal](https://danielmelendez-pma.github.io/cabinet-report-partners/)
