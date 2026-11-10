---
description: Convierte un Excel RP compatible a TXT y comprueba los datos antes de reabrir la producción.
---

# RP a TXT

**Curso de Cabinet Report · Conversión de archivos de producción**

Utiliza esta opción para convertir nuevamente en TXT un Excel RP generado por Cabinet Report, por ejemplo después de editarlo. La conversión requiere conservar su estructura original; sigue las capturas y verifica el TXT antes de continuar.

**Consulta también:** [Cargar TXT](cargar-txt.md) · [Parámetros de producción](parametros-de-produccion.md) · [Reporte de Producción detallado](reporte-de-produccion.md).

Para convertir los Excel RP previamente generados por Cabinet Report, al archivo TXT de producción.

Es especialmente útil si modificaste manualmente datos del Excel RP. **Guarda una copia del Excel original** y evita mover o eliminar secciones, encabezados y columnas, porque la conversión depende del formato esperado.

<figure><img src="../.gitbook/assets/image (7) (1) (1) (1) (1) (1) (1).png" alt="Vista de acceso a la conversión de Excel RP a TXT"><figcaption><p>La conversión parte de un Excel RP con su estructura conservada.</p></figcaption></figure>

---

## Ruta de comprobación

**Excel RP compatible → TXT convertido → [Parámetros de Producción](parametros-de-produccion.md) → [Revisión de Tableros y Cantos](revision-de-tableros-y-cantos.md) → [Reporte de Producción](reporte-de-produccion.md).** Convertir y abrir no equivale a validar una producción. Utiliza el ejercicio de conciliación de esta lección para comparar la copia editada y aprobada con el TXT y el RP abiertos.

## Estructura requerida del archivo Excel RP

El archivo debe conservar el formato del reporte Excel RP, con las siguientes secciones:

### Encabezado

<figure><img src="../.gitbook/assets/image (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1).png" alt="Encabezado del Excel RP utilizado en la conversión"><figcaption><p>Conserva la distribución de los campos de encabezado.</p></figcaption></figure>

### Sección de Módulos

<figure><img src="../.gitbook/assets/image (2) (1) (1) (1) (1) (1) (1) (1) (1).png" alt="Sección de módulos del Excel RP"><figcaption><p>Comprueba los módulos incluidos en el archivo de origen.</p></figcaption></figure>

### Sección de Piezas Sueltas

<figure><img src="../.gitbook/assets/image (3) (1) (1) (1) (1) (1) (1) (1) (1).png" alt="Sección de piezas sueltas del Excel RP"><figcaption><p>Revisa las piezas independientes y sus cantidades.</p></figcaption></figure>

### Sección de Observaciones

<figure><img src="../.gitbook/assets/image (4) (1) (1) (1) (1) (1) (1) (1) (1).png" alt="Sección de observaciones del Excel RP"><figcaption><p>Conserva la sección de observaciones del reporte.</p></figcaption></figure>

### Sección de Materiales

<figure><img src="../.gitbook/assets/image (5) (1) (1) (1) (1) (1) (1) (1) (1).png" alt="Sección de materiales del Excel RP"><figcaption><p>Contrasta las referencias de los materiales.</p></figcaption></figure>

### Sección de Herrajes y Accesorios

#### Zócalos de PVC

<figure><img src="../.gitbook/assets/image (6) (1) (1) (1) (1) (1) (1) (1).png" alt="Sección de zócalos de PVC del Excel RP"><figcaption><p>Verifica los registros de zócalos que correspondan.</p></figcaption></figure>

#### Golas

<figure><img src="../.gitbook/assets/image (7) (1) (1) (1) (1) (1) (1) (1).png" alt="Sección de golas del Excel RP"><figcaption><p>Verifica los registros de golas que correspondan.</p></figcaption></figure>

#### Tubos

<figure><img src="../.gitbook/assets/image (8) (1) (1) (1) (1) (1) (1).png" alt="Sección de tubos del Excel RP"><figcaption><p>Verifica los registros de tubos que correspondan.</p></figcaption></figure>

#### Accesorios

<figure><img src="../.gitbook/assets/image (9) (1) (1) (1) (1) (1) (1).png" alt="Sección de accesorios del Excel RP"><figcaption><p>Comprueba los accesorios de forma independiente.</p></figcaption></figure>

#### Ferretería de Montaje

<figure><img src="../.gitbook/assets/image (10) (1) (1) (1) (1) (1).png" alt="Sección de ferretería de montaje del Excel RP"><figcaption><p>Comprueba los registros de ferretería de montaje.</p></figcaption></figure>

#### Ferretería de Instalación

<figure><img src="../.gitbook/assets/image (11) (1) (1) (1) (1).png" alt="Sección de ferretería de instalación del Excel RP"><figcaption><p>Comprueba los registros de ferretería de instalación.</p></figcaption></figure>

{% hint style="warning" %}
**Compatibilidad:** no basta con que el archivo sea de Excel. Si el RP no conserva las secciones indicadas, la conversión puede fallar o producir un TXT incompleto. No utilices ese TXT en producción sin comprobarlo.
{% endhint %}
---
## Procedimiento de conversión

### 1. Selecciona el Excel RP

Seleccionar el archivo de Excel RP:

<figure><img src="../.gitbook/assets/image (16) (1) (1).png" alt="Selector del archivo Excel RP en la herramienta de conversión"><figcaption><p>Elige una copia del archivo Excel RP compatible.</p></figcaption></figure>

### 2. Comprueba el contenido

Cabinet Report analiza el archivo y puede mostrar su contenido. Comprueba que las secciones, cantidades y materiales reconocidos correspondan al Excel antes de generar el TXT:

<figure><img src="../.gitbook/assets/image (1) (1) (1) (1) (1) (1) (1) (1) (1) (1).png" alt="Vista de comprobación del contenido previo a la conversión"><figcaption><p>Contrasta las secciones, cantidades y materiales con el Excel aprobado.</p></figcaption></figure>

### 3. Genera el archivo TXT

Haz clic en **Generar TXT de Producción** cuando la vista previa corresponda con el Excel original.

<figure><img src="../.gitbook/assets/image (2) (1) (1) (1) (1) (1) (1) (1).png" alt="Control para generar un TXT de producción desde el Excel RP"><figcaption><p>Genera el TXT únicamente cuando los datos de origen estén comprobados.</p></figcaption></figure>

### 4. Selecciona dónde guardarlo

Selecciona dónde guardar el TXT de Producción. Para conservar una referencia, evita sobrescribir una versión anterior sin una copia de respaldo:

<figure><img src="../.gitbook/assets/image (3) (1) (1) (1) (1) (1) (1) (1).png" alt="Selección de destino para el TXT de producción convertido"><figcaption><p>Guarda el TXT de prueba sin sobrescribir el respaldo.</p></figcaption></figure>

### 5. Verifica y abre el resultado

Cabinet Report le informa que se ha generado y ya lo puede abrir, le muestra los datos del archivo y le pregunta si lo desea abrir, entonces le pide seleccione si es un RP nuevo o es para modificar un RP Anterior:

<figure><img src="../.gitbook/assets/image (4) (1) (1) (1) (1) (1) (1) (1).png" alt="Confirmación de generación del TXT y opción de apertura"><figcaption><p>La confirmación de creación no valida los datos convertidos.</p></figcaption></figure>

Haz clic en **Abrir** para acceder al **Reporte de Producción**. Antes de generar u optimizar, **compara el TXT convertido y el reporte abierto con el Excel de origen**: cliente, ambiente, módulos, piezas, cantidades, medidas, materiales y cantos. Si faltan datos, regresa al Excel original y revisa su estructura.

Continúa con [Revisión de Tableros y Cantos](revision-de-tableros-y-cantos.md) y la [guía detallada de la ventana](reporte-de-produccion.md).

<figure><img src="../.gitbook/assets/image (6) (1) (1) (1) (1) (1) (1).png" alt="Reporte de Producción abierto a partir de un TXT convertido"><figcaption><p>Concilia las piezas, unidades, medidas, materiales y cantos después de abrir.</p></figcaption></figure>


## Ejercicio verificable: Excel RP editado → TXT → RP recuperado

Este ensayo comprueba **la continuidad de los datos de piezas** cuando se modifica un Excel RP y se utiliza **RP a TXT** para abrirlo nuevamente en Cabinet Report. Es una **prueba manual de conciliación**, no una garantía de conversión reversible para cualquier archivo de Excel ni una descripción de un algoritmo nuevo.

### 1. Prepara las fuentes y define qué versión es válida

1. Parte de un **Excel RP generado por Cabinet Report** cuya estructura coincida con las secciones de las capturas anteriores. Conserva el **Excel original sin editar**.
2. Trabaja sobre una **copia del Excel** y registra los cambios autorizados: pieza, módulo o pieza suelta, cantidad, dimensión, material, veta o canto por lado. Evita alterar encabezados, hojas, posiciones de columnas, secciones o celdas de estructura que el conversor pueda necesitar.
3. Identifica **cliente, ambiente, número RP si existe, nombre del archivo y versión o fecha** tanto en el original como en la copia modificada. Indica cuál de los dos es la fuente aprobada para la comparación; una edición sin revisar no debe convertirse automáticamente en referencia de fabricación.
4. Convierte la **copia modificada** siguiendo los pasos 1 a 4 de esta lección. Guarda el **TXT resultante en un destino de prueba distinto**, sin sustituir el archivo de producción anterior.

{% hint style="warning" %}
**Evita modificar una producción real durante el ensayo.** Para comprobar la apertura del TXT, elige la opción de **RP nuevo** que ofrezca la versión instalada; utiliza **Modificar RP Anterior** únicamente cuando tengas identificado y respaldado el RP que realmente deseas actualizar.
{% endhint %}

### 2. Prepara una hoja de conciliación por pieza

Como ejemplo didáctico, imagina **un módulo** con dos costados, una base y una tapa, más **una pieza suelta**. La composición es solo una referencia para contar; **no establece medidas ni fórmulas constructivas**.

| Origen de la pieza | Tipo de pieza | Unidades efectivas esperadas |
| --- | --- | ---: |
| Módulo de práctica | Costado | 2 |
| Módulo de práctica | Base | 1 |
| Módulo de práctica | Tapa | 1 |
| Pieza suelta | Pieza independiente | 1 |
| **Total teórico** | **4 tipos de registro** | **5 unidades** |

**No confundas filas, tipos de pieza y unidades.** El ejemplo contiene cinco unidades físicas esperadas, aunque el número de filas representadas por la interfaz o por el archivo pueda ser distinto. En una producción real, registra cada identificación de pieza y sus unidades, sin sumar como equivalentes conjuntos diferentes.

Para las piezas que se hayan modificado en la copia del Excel, utiliza además una tabla de control como esta (rellénala con datos reales del proyecto):

| Dato a verificar | Excel original | Excel editado y aprobado | TXT convertido | RP abierto desde el TXT |
| --- | --- | --- | --- | --- |
| Cliente, ambiente e identificación del trabajo | Registrar | Confirmar | Comprobar | Comprobar |
| Módulo o pertenencia a piezas sueltas | Registrar | Confirmar | Comprobar | Comprobar |
| Pieza y **cantidad efectiva** | Registrar | Confirmar cambio | Comprobar | Comprobar |
| Espesor, ancho, largo y orientación | Registrar | Confirmar cambio | Comprobar | Comprobar |
| Material, veta y **cada lado de canto** | Registrar | Confirmar cambio | Comprobar | Comprobar |

La columna **Excel editado y aprobado** es la referencia para evaluar la conversión; el original permite rastrear qué se cambió. Si un dato no aparece o no puede verificarse en una de las representaciones, marca **«No comprobado»** en lugar de asumir que se transfirió correctamente.

### 3. Abre el TXT y contrasta el resultado

1. Conserva el TXT obtenido y vuelve a abrirlo mediante el recorrido [Cargar TXT](cargar-txt.md), utilizando una **prueba separada** de la producción original.
2. Revisa los [Parámetros de Producción](parametros-de-produccion.md) seleccionados al abrir. Si hay automatizaciones que afectan medidas, veta, orientación o materiales, **registra su configuración** antes de comparar; no atribuyas automáticamente cada diferencia al conversor.
3. En el RP abierto, compara las **unidades efectivas por pieza**, incluida su pertenencia a un módulo o a piezas sueltas. Comprueba también dimensiones, espesor, material, veta y los cuatro lados del canteo, donde correspondan.
4. Identifica cada discrepancia con la **pieza de origen** y el dato afectado. Distingue si procede de la edición del Excel, de la conversión, de una automatización al abrir o de una diferencia todavía no explicada. No corrijas los totales de destino sin rastrear su fuente.
5. Comprueba los **archivos complementarios por separado**. El TXT de piezas y el RP recuperado **no demuestran por sí solos** que se hayan recuperado accesorios, ferretería, parámetros técnicos, metadatos XML o decisiones de Auditoría RP. Consulta [Archivos de Reportes Generados](archivos-de-reportes-generados.md).

{% hint style="info" %}
**Variantes históricas del TXT:** esta prueba no fija ni sustituye encabezados, separadores o posiciones de campos. Utiliza un archivo generado por el conversor de la versión compatible y aplica las comprobaciones del procedimiento [Cargar TXT](cargar-txt.md); no reconstruyas columnas por deducción.
{% endhint %}

### 4. Decide si puedes continuar

| Resultado de la prueba | Acción |
| --- | --- |
| Identificación, piezas, cantidades, dimensiones, materiales y cantos coinciden con la fuente aprobada | Registra los archivos y las comprobaciones; continúa con la revisión técnica habitual del RP |
| Hay una diferencia explicable por una configuración o edición intencional | Documenta su origen y vuelve a validar la pieza afectada antes de aprobar |
| Faltan piezas, sobran unidades, cambia un material o no se acredita un canto o una medida | **Detén la generación, optimización y entrega**; conserva todas las versiones y revisa el origen y la conversión |
| Los datos complementarios o la persistencia del proyecto no se han comprobado | **No los declares recuperados**; verifica sus registros de forma independiente |

**Evidencia mínima del ensayo:** conserva la ruta de cada archivo, la versión del Excel original y la copia editada, el TXT convertido, la identificación del RP de prueba, los parámetros aplicados, el recuento efectivo por pieza, los cambios esperados y las diferencias resueltas. Solo tras esa conciliación debe evaluarse la preparación de fabricación; **abrir el archivo sin error no equivale a aprobarlo**.

---

[← Cargar TXT](cargar-txt.md) · [Reporte en blanco →](reporte-en-blanco.md) · [Índice del Reporte de Producción](README.md) · [🏠 Portal principal](https://danielmelendez-pma.github.io/cabinet-report-partners/)
