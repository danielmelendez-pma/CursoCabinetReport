# Creación de Piezas

Conoce las áreas del Creador de Piezas y estudia los ejemplos de fórmulas de espesor, ancho, largo y cantos. Conserva las variables y los valores de cada ejemplo como referencia de la versión documentada.

<figure><img src=".gitbook/assets/image (4) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1).png" alt=""><figcaption></figcaption></figure>

Después de conocer las [variables de cálculo](formulas-y-variables.md), continúa con el **Creador de Piezas**. Aquí puedes preparar nuevas piezas o consultar las que ya están guardadas en Cabinet Report.

## Creador de Piezas

> 💡 **Importante**\
> Un Creador de Piezas bien configurado garantiza que Cabinet Report genere información confiable, minimizando errores humanos y mejorando la eficiencia en el proceso productivo.

***

## Áreas del Creador de Piezas

La sección del Creador de Piezas se divide en tres partes:

<figure><img src=".gitbook/assets/image (22).png" alt=""><figcaption></figcaption></figure>

## Lista de Piezas Guardadas

Aparecen las piezas existentes creadas y las nuevas que se creen con sus propias fórmulas

También tiene un campo para desactivar si desea editar una pieza creada.

## Área de Fórmulas

Para colocar el nombre de la pieza y sus fórmulas para las medidas de:

ESPESOR X ANCHO X LARGO

<figure><img src=".gitbook/assets/image (23).png" alt=""><figcaption></figcaption></figure>

<figure><img src=".gitbook/assets/image (24).png" alt=""><figcaption></figcaption></figure>

## Sección de Variables

Lista de variables que le ayuda a crear las formulas de cada una de sus piezas.

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

---

[← Fórmulas y variables](formulas-y-variables.md) · [Creación de módulos →](creacion-de-modulos.md) · [🏠 Portal principal](https://danielmelendez-pma.github.io/cabinet-report-partners/)
