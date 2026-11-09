# Creación de Piezas

Conoce las áreas del Creador de Piezas y estudia los ejemplos de fórmulas de espesor, ancho, largo y cantos. Conserva las variables y los valores de cada ejemplo como referencia de la versión documentada.

<figure><img src=".gitbook/assets/image (4) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1).png" alt=""><figcaption></figcaption></figure>

Una vez aprendido las variables para crear formulas de calculo de piezas, puede adentrarse a la sección de

## Creador de Piezas

Donde puede crear sus piezas o utilizar las piezas ya creadas dentro de Cabinet Report

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

CANTO IZQUIERDO = CCAJONCCAJON

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
