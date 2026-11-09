# Parámetros de Producción

Antes de importar un archivo TXT o CSV, revisa las opciones de vetas, automatizaciones, packing list y el tipo de reporte que vas a preparar.

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

Ejemplo: si el canto es de 2mm, Cabinet Report le reduce 1mm de cada lado a cada pieza y así la fresadora solo debe resanar 1mm y no 2mm

**Aplicar Medidas Mínimas de Fascias:** si el usuario ingresa una pieza o fascia de 30mm, Cabinet Report de manera automática la agranda a 60mm para que así pase sin problemas por las máquinas de Corte y Canteo.

**Carga automática de Herrajes y Perfilerías:** al abrir el archivo TXT y la carpeta también contiene los archivos de herrajes, en lugar de que el usuario los cargue manualmente, Cabinet Report lo carga de manera automática.

Invertir medida de Piezas sin Vetas: si el usuario activa que la producción contiene material sin vetas, Cabinet Report arregla medidas de algunas piezas:

Ejemplos:

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

Esto es importante ya que si no se usa de manera correcta, no puede llevar un control adecuado sobre las producciones.

***

Una vez cumlido con lo anterior, estal listo para el siguiente paso y puede abrir su archivo

<figure><img src="../.gitbook/assets/image (54).png" alt=""><figcaption></figcaption></figure>

---

[← Reporte en blanco](reporte-en-blanco.md) · [Revisión de tableros y cantos →](revision-de-tableros-y-cantos.md) · [🏠 Portal principal](https://danielmelendez-pma.github.io/cabinet-report-partners/)
