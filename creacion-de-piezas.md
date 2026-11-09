# Creación de Piezas

Conoce las áreas del Creador de Piezas y estudia los ejemplos de fórmulas de espesor, ancho, largo y cantos. Conserva las variables y los valores de cada ejemplo como referencia de la versión documentada.

<figure><img src=".gitbook/assets/image (4) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1).png" alt=""><figcaption></figcaption></figure>

Después de conocer las [variables de cálculo](formulas-y-variables.md), continúa con el **Creador de Piezas**. Aquí puedes preparar nuevas piezas o consultar las que ya están guardadas en Cabinet Report.

## Creador de Piezas

> 💡 **Importante**\
> Una definición de pieza revisada ayuda a mantener un despiece consistente. **Guardar una fórmula o ver una medida calculada no garantiza que la pieza sea fabricable**: comprueba su resultado para el módulo, los materiales y los parámetros del cliente.

***

## Áreas del Creador de Piezas

La sección del Creador de Piezas se divide en tres partes:

<figure><img src=".gitbook/assets/image (22).png" alt=""><figcaption></figcaption></figure>

## Lista de Piezas Guardadas

Muestra las piezas existentes y las nuevas definiciones guardadas con sus fórmulas. Antes de crear una nueva, busca si ya existe una equivalente y comprueba que sus expresiones correspondan al módulo que estás preparando.

La interfaz documentada también incluye un control relacionado con la edición de piezas existentes; identifica su estado antes de modificar una definición que otros módulos puedan utilizar.

## Área de Fórmulas

Aquí se indica el nombre de la pieza y se preparan las expresiones de sus tres dimensiones, cada una en su campo:

**ESPESOR X ANCHO X LARGO**

<figure><img src=".gitbook/assets/image (23).png" alt=""><figcaption></figcaption></figure>

<figure><img src=".gitbook/assets/image (24).png" alt=""><figcaption></figcaption></figure>

## Sección de Variables

Lista de variables que ayuda a construir las fórmulas de las piezas. Antes de utilizarlas, revisa la definición y el valor aplicado en el contexto del módulo; consulta [Fórmulas y Variables](formulas-y-variables.md).

## Secuencia para definir o revisar una pieza

1. **Localiza la pieza** en el listado o identifica la nueva definición que necesitas.
2. **Revisa el módulo de referencia** y sus dimensiones `PROF`, `ANCHO` y `ALTO`.
3. **Comprueba los valores de variables** de espesores, luces, ranuras y demás descuentos que intervienen.
4. **Introduce por separado** la expresión de espesor, ancho y largo.
5. **Asigna los cantos por lado** y confirma material y orientación cuando se definan en tu flujo.
6. **Contrasta el resultado** con medidas conocidas antes de guardar o reutilizar la pieza.

{% hint style="info" %}
Si una variable carece de definición o no puedes verificar su valor efectivo, **no deduzcas su valor únicamente a partir del resultado mostrado en un ejemplo**. Señala el dato pendiente de validación.
{% endhint %}

***

## Antes de interpretar las fórmulas

En los ejemplos siguientes, cada pieza presenta **espesor, ancho y largo**, además del canto asignado a cada borde. El símbolo **X** separa las dimensiones del resultado mostrado; no significa que debas escribir las tres expresiones en un único campo.

| Revisión | Qué comprobar |
| --- | --- |
| **Espesor** | Variable y tablero utilizados para la pieza. |
| **Ancho y largo** | Expresiones y descuentos respecto del módulo actual. |
| **Cantos** | Aplicación correcta en los cuatro lados. |
| **Resultado** | Coincidencia de las medidas calculadas con el diseño. |

{% hint style="warning" %}
**Ejemplo heredado: comprueba sus valores antes de reutilizarlos.** La descripción original menciona un respaldo de cartón de **4 mm**, pero el resultado de «RESPALDO CART» indica **3 mm**. Además, la fórmula de «BASE» utiliza `CART`, cuyo significado no se desarrolla en la lista de [Fórmulas y Variables](formulas-y-variables.md). Se conservan las expresiones y los resultados originales para su consulta, sin presentarlos como parámetros universales. Verifica el espesor real, la definición de cada término y las medidas de salida en tu versión del programa.
{% endhint %}

## Ejemplo de fórmulas por pieza

Para un mueble base de 580 x 900 x 780, con 2 puertas con 1 tablilla y respaldo de cartón 4mm, donde el cajon interno es color blanco 15mm y las partes vistas es color madera 18mm, tomando en cuenta que el costado izquierdo es visto:

**Cómo leer este ejemplo histórico:** las dimensiones iniciales describen el mueble; los resultados siguientes corresponden a cada pieza. Las luces, ranuras y otros descuentos no están acompañados de todos sus valores efectivos. **No reutilices los resultados como medidas estándar de fabricación**.

<figure><img src=".gitbook/assets/image (26).png" alt=""><figcaption></figcaption></figure>

***

### COSTADO IZQUIERDO
FÓRMULA: ESPV **X** PROF **X** ALTO 

RESULTADO: 18 X 580 X 780 MADERA

CANTO SUPERIOR = CVISTO

CANTO INFERIOR = CVISTO

CANTO IZQUIERDO = CVISTO

CANTO DERECHO = CVISTO

***

### COSTADO DERECHO
FÓRMULA: ESPC **X** PROF **X** ALTO 

RESULTADO: 15 X 580 X 780 BLANCO

CANTO SUPERIOR = CVISTO

CANTO INFERIOR = CCAJON

CANTO IZQUIERDO = CCAJON

CANTO DERECHO = CCAJON

***

### BASE
FÓRMULA: ESPC **X** PROF-ESPC-CART **X** ANCHO-ESPV-ESPC 

RESULTADO: 15 X 562 X 867 BLANCO

CANTO SUPERIOR = CVISTO

CANTO INFERIOR = CCAJON

CANTO IZQUIERDO = CCAJON

CANTO DERECHO = CCAJON

***

### CADENA POST
FÓRMULA: ESPC **X** 100 **X** ANCHO-ESPV-ESPC 

RESULTADO: 15 X 100 X 867 BLANCO

CANTO SUPERIOR = CCAJON

CANTO INFERIOR = CCAJON

CANTO IZQUIERDO = CCAJON

CANTO DERECHO = CCAJON

***

### CADENA FRONT
FÓRMULA: ESPC **X** 100 **X** ANCHO-ESPV-ESPC 

RESULTADO: 15 X 100 X 867 BLANCO

CANTO SUPERIOR = CVISTO

CANTO INFERIOR = CCAJON

CANTO IZQUIERDO = CCAJON

CANTO DERECHO = CCAJON

***

### TABLILLA MOVIBLE
FÓRMULA: ESPC **X** PROF-ESPC-RESP-ESPC **X** ANCHO-ESPC-ESPV-PIN-PIN 

RESULTADO: 15 X 547 X 865 BLANCO

CANTO SUPERIOR = CCAJON

CANTO INFERIOR = CCAJON

CANTO IZQUIERDO = CCAJON

CANTO DERECHO = CVISTO

***

### RESPALDO CART
FÓRMULA: RESP **X** ANCHO-ESPC-ESPV+RAN+RAN **X** ALTO-LSR 

RESULTADO: 3 X 881 X 778 CARTON

CANTO SUPERIOR = N/A

CANTO INFERIOR = N/A

CANTO IZQUIERDO = N/A

CANTO DERECHO = N/A

***

### PUERTA IZQ
FÓRMULA: ESPV **X** (ANCHO-LIZ-LDE-LCE)/2 **X** ALTO-LSU-LIN 

RESULTADO: 18 X 448 X 776

CANTO SUPERIOR = CVISTO

CANTO INFERIOR = CVISTO

CANTO IZQUIERDO = CVISTO

CANTO DERECHO = CVISTO

***

### PUERTA DER
**FÓRMULA:** ESPV **X** (ANCHO-LIZ-LDE-LCE)/2 **X** ALTO-LSU-LIN 

**RESULTADO:** 18 X 448 X 776

CANTO SUPERIOR = CVISTO

CANTO INFERIOR = CVISTO

CANTO IZQUIERDO = CVISTO

CANTO DERECHO = CVISTO

***

## Comprueba los ejemplos antes de reutilizarlos

1. **Valida el módulo y sus unidades:** que 580 × 900 × 780 y los resultados mostrados correspondan a tus referencias de diseño.
2. **Identifica las variables.** La fórmula de la `BASE` utiliza `CART`, pero aquí no consta su definición ni su valor efectivo. No la equipares automáticamente con `RESP`.
3. **Confirma el espesor real del respaldo:** la introducción menciona **4 mm** y el resultado histórico de **RESPALDO CART** muestra **3 mm**. La discrepancia sigue **pendiente de comprobación técnica**.
4. **Contrasta las puertas:** esta lección muestra **448 mm** por hoja; el ejemplo didáctico de [Fórmulas y Variables](formulas-y-variables.md) muestra **447 mm**, calculados con luces expresamente asumidas. Sin los valores efectivos de este caso, **no se puede corregir un resultado por comparación directa**.
5. **Revisa los cantos y la orientación:** cada borde tiene una función; confirma material, veta, ancho y largo antes de fabricar.
6. **Prueba con tu configuración:** comprueba los valores efectivos del cliente y del módulo, y revisa las piezas resultantes en el RP.

Para consultar las funciones y precauciones relacionadas, revisa el [Creador de piezas en la Documentación oficial](https://cabinet-report.gitbook.io/cabinet-report-docs/funcionalidades-de-cabinet-report/creador-de-piezas) y la [guía del Reporte de Producción](https://cabinet-report.gitbook.io/cabinet-report-docs/funcionalidades-de-cabinet-report/reporte-de-produccion).

---

[← Fórmulas y variables](formulas-y-variables.md) · [Creación de módulos →](creacion-de-modulos.md) · [🏠 Portal principal](https://danielmelendez-pma.github.io/cabinet-report-partners/)
