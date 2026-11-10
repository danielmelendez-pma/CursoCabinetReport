---
description: >-
  Aprende a localizar, definir y comprobar piezas con fórmulas, variables,
  materiales y cantos, diferenciando ejemplos históricos de datos efectivos.
layout:
  width: wide
---

# Creación de Piezas

Aprende a **identificar, definir y comprobar piezas** para integrarlas en módulos y en el Reporte de Producción de Cabinet Report. Las capturas y los resultados numéricos son referencias históricas de la interfaz documentada: no sustituyen las medidas ni los parámetros reales de tu proyecto.

## Recorrido de aprendizaje

1. **Reconoce las áreas** del Creador de Piezas y localiza definiciones existentes.
2. **Distingue fórmulas y valores efectivos** antes de trabajar con espesor, ancho, largo y cantos.
3. **Prepara o revisa una pieza** sin alterar por error una definición compartida.
4. **Interpreta el ejemplo histórico**, identificando datos sin acreditar y discrepancias pendientes.
5. **Comprueba dos módulos de ensayo** con evidencias independientes antes de fabricar.

Para comprender las variables, consulta [Fórmulas y Variables](formulas-y-variables.md); para la función general, revisa el [Creador de piezas de la Documentación Oficial](https://cabinet-report.gitbook.io/cabinet-report-docs/funcionalidades-de-cabinet-report/creador-de-piezas).

<figure><img src=".gitbook/assets/image (4) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1).png" alt="Vista general histórica del Creador de Piezas de Cabinet Report"><figcaption><p>Acceso visual a la interfaz histórica del Creador de Piezas; verifica los controles disponibles en tu versión.</p></figcaption></figure>

Una pieza puede ser un costado, una base, una tablilla o un frente. **El mismo nombre no demuestra que tenga la misma fórmula en todos los módulos**: identifica la definición y el contexto técnico antes de seleccionarla.

{% hint style="info" %}
**Antes de empezar:** ten disponibles una copia de ensayo del proyecto, la versión del programa, las dimensiones del módulo, las definiciones de tableros y los parámetros del cliente. Si solo necesitas consultar una pieza existente, evita editar el catálogo.
{% endhint %}

## Creador de Piezas

La definición describe **cómo se calcula una pieza**, mientras que la medida obtenida depende del módulo y de los valores aplicados. La edición, el guardado y la reutilización deben comprobarse de acuerdo con los controles y permisos presentes en tu versión.

{% hint style="warning" %}
**Guardar no equivale a aprobar para fabricación.** Una fórmula guardada o una medida visible no garantiza que la pieza sea fabricable. Comprueba el cálculo, el material, la orientación, los cantos y la producción correspondiente.
{% endhint %}

---

## Áreas del Creador de Piezas

La interfaz histórica se organiza en **tres áreas**: lista de piezas guardadas, edición de fórmulas y consulta de variables. Identifica cada área en tu versión antes de ejecutar cambios.

<figure><img src=".gitbook/assets/image (22).png" alt="Vista histórica de las tres áreas del Creador de Piezas"><figcaption><p>Reconoce lista de piezas, área de fórmulas y variables antes de editar una definición.</p></figcaption></figure>

## Lista de Piezas Guardadas

1. **Busca una definición existente** por su denominación y comprueba si corresponde al tipo de módulo que vas a preparar.
2. **Consulta las expresiones reales** de espesor, ancho y largo: dos nombres iguales no acreditan fórmulas iguales.
3. **Reconoce el estado del control de edición** documentado antes de modificar un registro. Si no conoces el alcance de una actualización sobre otros módulos, conserva la definición original y realiza la prueba en una copia autorizada.

La lista permite reconocer piezas guardadas, pero **no acredita por sí misma** sus resultados en una producción concreta.

## Área de Fórmulas

En la interfaz documentada se identifica la pieza por su nombre y se preparan **tres expresiones diferenciadas**, una por dimensión. La notación de lectura es:

**ESPESOR X ANCHO X LARGO**

La **X** separa las dimensiones en la explicación; no indica que debas introducirlas juntas en un único campo. Conserva el orden exacto de ancho y largo y comprueba qué orientación corresponde a cada pieza.

<figure><img src=".gitbook/assets/image (23).png" alt="Captura histórica de los campos de definición de fórmulas de piezas"><figcaption><p>Referencia visual para revisar las expresiones dimensionales por separado.</p></figcaption></figure>

<figure><img src=".gitbook/assets/image (24).png" alt="Segunda captura histórica del área de fórmulas del Creador de Piezas"><figcaption><p>Detalle complementario del editor; contrasta los campos con tu versión instalada.</p></figcaption></figure>

## Sección de Variables

Esta área permite consultar variables que intervienen en las expresiones. Revisa en [Fórmulas y Variables](formulas-y-variables.md) las dimensiones `PROF`, `ANCHO` y `ALTO`, los espesores `ESPC`, `ESPV` y `RESP`, las luces, las ranuras y los cantos.

**Diferencia entre definición y valor:** una variable identificada no significa que se haya comprobado el número efectivo de ese cliente o módulo. Un valor **0** puede ser válido; no lo sustituyas por otro por mera apariencia.

{% hint style="warning" %}
La expresión histórica de la `BASE` utiliza `CART`. La clasificación de materiales `CART` que aparece en [Creación de Tableros](creacion-de-tableros.md) **no acredita** que el término de la fórmula tenga ese mismo significado ni establece su valor. Registra esa definición como pendiente si no puedes verificarla en tu versión.
{% endhint %}

## Secuencia para definir o revisar una pieza

1. **Localiza la pieza** en el listado y decide si se trata de una consulta, una definición nueva o una modificación autorizada.
2. **Identifica el módulo de referencia** y registra `PROF`, `ANCHO`, `ALTO` y las unidades de trabajo.
3. **Anota la procedencia de cada variable efectiva**: espesores, luces, ranuras, pines y otros descuentos que aparezcan en **esa** fórmula. No conviertas valores de ejemplo en parámetros globales.
4. **Revisa o introduce por separado** espesor, ancho y largo; comprueba signos, paréntesis y orden dimensional.
5. **Contrasta la referencia del tablero** y su espesor con el material real previsto; no confundas el catálogo con existencias físicas.
6. **Verifica cantos por lado** (superior, inferior, izquierdo y derecho), junto con veta y orientación si intervienen en el diseño.
7. **Calcula independientemente** el resultado de la fórmula para el módulo conocido y compara con lo que muestra el programa.
8. **Guarda o actualiza solo si corresponde** y si tienes autorización. Antes de modificar una pieza existente, conserva su definición inicial y confirma el efecto de la edición en las estructuras que la utilizan.
9. **Revisa la pieza en el módulo y en una producción de ensayo**, utilizando [Creación de Módulos](creacion-de-modulos.md), [Catálogo de Módulos](catalogo-de-modulos.md) y [Reporte de Producción](reporte-de-produccion/README.md).

**Resultado esperado de este procedimiento:** una definición identificada, con fórmulas y valores verificables, y un registro de las medidas obtenidas; no una aprobación automática de corte.

{% hint style="info" %}
Si una variable carece de definición o no puedes verificar su valor efectivo, **no deduzcas su valor únicamente a partir del resultado mostrado en un ejemplo**. Señala el dato pendiente de validación.
{% endhint %}


***

## Antes de interpretar las fórmulas

Los registros siguientes son **ejemplos históricos**, no una tabla de cortes autorizada. Cada pieza presenta **espesor, ancho y largo**, además del canto asignado a cada borde. El símbolo **X** separa las dimensiones del resultado mostrado; no significa que debas escribir las tres expresiones en un único campo. Conserva la fórmula original al contrastar el resultado, aunque detectes una inconsistencia.

La distinción entre `CVISTO` y `CCAJON` identifica tipos de canto; **no son descuentos dimensionales**. Verifica además a qué borde corresponde cada asignación.

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

**Convención de lectura:** en cada bloque, `FÓRMULA` y `RESULTADO` se presentan en orden **espesor × ancho × largo**, seguidos de los cantos indicados por lado. Se preservan literalmente las expresiones y resultados históricos; la comprobación de su coherencia exige los valores efectivos del caso.

<figure><img src=".gitbook/assets/image (26).png" alt="Captura histórica asociada al ejemplo de fórmulas de un mueble base"><figcaption><p>Referencia visual del caso de 580 × 900 × 780; no convierte sus medidas en valores predeterminados.</p></figcaption></figure>

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

### Registro de discrepancias que requieren evidencia

| Cuestión | Evidencia histórica | Criterio de comprobación |
| --- | --- | --- |
| `CART` en la `BASE` | Aparece en la expresión `PROF-ESPC-CART`, sin definición de variable acreditada en [Fórmulas y Variables](formulas-y-variables.md). | No equiparar con `RESP` ni con el tipo de tablero `CART`; contrastar la procedencia y el valor efectivo en la versión instalada. |
| Respaldo de **4 mm / 3 mm** | La descripción indica cartón de **4 mm**, mientras `RESPALDO CART` presenta **3 mm**. | Confirmar material, ficha de tablero, variable `RESP` y fórmula aplicable; no corregir la documentación por inferencia. |
| Puertas de **448 mm / 447 mm** | Aquí figura **448 mm** por hoja; el ejercicio de [Fórmulas y Variables](formulas-y-variables.md) obtiene **447 mm** con luces didácticas explícitas. | Comparar solo si se acreditan las luces y el contexto del módulo; resultados de ejemplos diferentes no demuestran un error automático. |

Estas cuestiones permanecen **pendientes de confirmación técnica en una versión y un proyecto identificados**. El registro editorial no modifica fórmulas ni parámetros del programa.

---

## Ensayo reproducible: una misma pieza en dos módulos de medidas diferentes

Este es un **ensayo de comprobación documental** para detectar cálculos incoherentes al reutilizar una definición de pieza. No acredita por sí solo el funcionamiento de todas las versiones ni sustituye la inspección del despiece en una producción real.

### Prepara un caso controlado

1. Trabaja en una **copia de ensayo** del proyecto y conserva intactos los archivos originales. Anota cliente, ambiente, versión de Cabinet Report y referencia de la prueba.
2. Escoge dos módulos de prueba **A y B**, del mismo tipo constructivo, que puedan utilizar la **misma definición de pieza**. Deben tener medidas distintas en al menos una dimensión (`PROF`, `ANCHO` o `ALTO`) que aparezca realmente en la fórmula elegida.
3. Identifica la pieza por su nombre y, si la interfaz lo permite, por su código o referencia. Copia **las expresiones exactas** de espesor, ancho y largo que se muestran para A y B; **un nombre igual no demuestra que sean la misma fórmula**.
4. Registra por separado las dimensiones de A y B, los tableros y espesores, el material, la veta, los cuatro cantos y **cada variable efectiva** empleada por esas expresiones. Un valor `0` puede ser legítimo: no lo reemplaces por un valor público o supuesto.
5. Si no puedes acreditar que la pieza y sus fórmulas son comparables, o falta el valor de una variable, marca la comprobación afectada como **NO EJECUTADO**. No inventes el dato para completar el ejercicio.

### Calcula y contrasta sin editar la definición compartida

1. Calcula **por separado** el resultado esperado de la pieza en A y en B, sustituyendo únicamente los valores efectivos comprobados en **la fórmula de esa misma pieza**. Anota la operación y sus unidades; no copies como referencia universal los resultados históricos de esta página.
2. Consulta la pieza calculada en cada módulo mediante el recorrido descrito en [Creación de Módulos](creacion-de-modulos.md) y [Catálogo de Módulos](catalogo-de-modulos.md). Registra las medidas y cantidades que realmente aparecen.
3. Compara **espesor, ancho y largo** con los cálculos independientes de cada módulo; compara también material, veta y lados de canto con la configuración prevista para **ese** módulo. No supongas que estos atributos deban ser idénticos entre A y B.
4. Comprueba que ninguna otra pieza o cantidad haya cambiado inadvertidamente en el proyecto de ensayo y que los datos originales permanecen intactos. Si una fórmula mostrada en A difiere de la de B, registra la diferencia y **no la atribuyas automáticamente a un error de recálculo**.
5. Si ambos módulos se incorporan a una producción de ensayo, revisa sus piezas por separado en el [Reporte de Producción](reporte-de-produccion/README.md). La coincidencia en el creador no demuestra por sí sola que el archivo final conserve los mismos datos.

### Matriz de evidencias

| Control | Evidencia para considerar CONFORME |
| --- | --- |
| Definición utilizada | Identificación y expresiones de la pieza registradas para A y B; diferencias justificadas antes de comparar. |
| Procedencia de valores | Dimensiones y variables efectivas de cada módulo identificadas, sin completar incógnitas por suposición. |
| Resultado dimensional | Espesor, ancho y largo coinciden con la evaluación independiente de la fórmula aplicable a cada módulo. |
| Propiedades y cantidades | Material, veta, cantos, cantidad y piezas no seleccionadas se corresponden con el diseño y el registro inicial. |
| Salida de producción, si se ejecuta | Las piezas de A y B se reconocen por separado y conservan sus atributos técnicos en el reporte de ensayo. |

Registra para cada control **CONFORME** cuando exista evidencia suficiente, **NO CONFORME** cuando se confirme una discrepancia, o **NO EJECUTADO** cuando no se haya probado o falten datos. Conserva una tabla o capturas con los valores **A / B / esperado / obtenido**, la versión probada y la decisión tomada. No declares conforme el ensayo completo si algún control aplicable queda sin comprobar.

{% hint style="warning" %}
**Antes de reutilizar la pieza en fabricación:** si hay una diferencia no justificada, detén su incorporación al trabajo definitivo y revisa la fórmula concreta, el módulo y las variables del cliente. No modifiques una definición compartida para resolver un caso de prueba, ni presupongas propagación, reversión automática o persistencia de cambios en el catálogo. Recupera solo una copia original previamente verificada.
{% endhint %}

## Referencias para contrastar

- [Fórmulas y Variables](formulas-y-variables.md): significado documentado de parámetros y ejemplo didáctico de puertas.
- [Creación de Módulos](creacion-de-modulos.md) y [Catálogo de Módulos](catalogo-de-modulos.md): uso de la definición en un módulo real.
- [Creación de Tableros](creacion-de-tableros.md): material, espesor y distinción entre clasificación de tablero y expresión de cálculo.
- [Creador de piezas — Documentación Oficial](https://cabinet-report.gitbook.io/cabinet-report-docs/funcionalidades-de-cabinet-report/creador-de-piezas) y [Reporte de Producción — Documentación Oficial](https://cabinet-report.gitbook.io/cabinet-report-docs/funcionalidades-de-cabinet-report/reporte-de-produccion): alcance funcional y revisión de salida.

---

[← Fórmulas y variables](formulas-y-variables.md) · [Creación de módulos →](creacion-de-modulos.md) · [🏠 Portal principal](https://danielmelendez-pma.github.io/cabinet-report-partners/)
