# RP a TXT

**Curso de Cabinet Report · Conversión de archivos de producción**

Utiliza esta opción para convertir nuevamente en TXT un Excel RP generado por Cabinet Report, por ejemplo después de editarlo. La conversión requiere conservar su estructura original; sigue las capturas y verifica el TXT antes de continuar.

**Consulta también:** [Cargar TXT](cargar-txt.md) · [Parámetros de producción](parametros-de-produccion.md) · [Reporte de Producción detallado](reporte-de-produccion.md).

Para convertir los Excel RP previamente generados por Cabinet Report, al archivo TXT de producción.

Es especialmente útil si modificaste manualmente datos del Excel RP. **Guarda una copia del Excel original** y evita mover o eliminar secciones, encabezados y columnas, porque la conversión depende del formato esperado.

<figure><img src="../.gitbook/assets/image (7) (1) (1) (1) (1) (1) (1).png" alt=""><figcaption></figcaption></figure>

---
## Estructura requerida del archivo Excel RP

El archivo debe conservar el formato del reporte Excel RP, con las siguientes secciones:

### Encabezado

<figure><img src="../.gitbook/assets/image (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1).png" alt=""><figcaption></figcaption></figure>

### Sección de Módulos

<figure><img src="../.gitbook/assets/image (2) (1) (1) (1) (1) (1) (1) (1) (1).png" alt=""><figcaption></figcaption></figure>

### Sección de Piezas Sueltas

<figure><img src="../.gitbook/assets/image (3) (1) (1) (1) (1) (1) (1) (1) (1).png" alt=""><figcaption></figcaption></figure>

### Sección de Observaciones

<figure><img src="../.gitbook/assets/image (4) (1) (1) (1) (1) (1) (1) (1) (1).png" alt=""><figcaption></figcaption></figure>

### Sección de Materiales

<figure><img src="../.gitbook/assets/image (5) (1) (1) (1) (1) (1) (1) (1) (1).png" alt=""><figcaption></figcaption></figure>

### Sección de Herrajes y Accesorios

#### Zócalos de PVC

<figure><img src="../.gitbook/assets/image (6) (1) (1) (1) (1) (1) (1) (1).png" alt=""><figcaption></figcaption></figure>

#### Golas

<figure><img src="../.gitbook/assets/image (7) (1) (1) (1) (1) (1) (1) (1).png" alt=""><figcaption></figcaption></figure>

#### Tubos

<figure><img src="../.gitbook/assets/image (8) (1) (1) (1) (1) (1) (1).png" alt=""><figcaption></figcaption></figure>

#### Accesorios

<figure><img src="../.gitbook/assets/image (9) (1) (1) (1) (1) (1) (1).png" alt=""><figcaption></figcaption></figure>

#### Ferretería de Montaje

<figure><img src="../.gitbook/assets/image (10) (1) (1) (1) (1) (1).png" alt=""><figcaption></figcaption></figure>

#### Ferretería de Instalación

<figure><img src="../.gitbook/assets/image (11) (1) (1) (1) (1).png" alt=""><figcaption></figcaption></figure>

{% hint style="warning" %}
**Compatibilidad:** no basta con que el archivo sea de Excel. Si el RP no conserva las secciones indicadas, la conversión puede fallar o producir un TXT incompleto. No utilices ese TXT en producción sin comprobarlo.
{% endhint %}
---
## Procedimiento de conversión

### 1. Selecciona el Excel RP

Seleccionar el archivo de Excel RP:

<figure><img src="../.gitbook/assets/image (16) (1) (1).png" alt=""><figcaption></figcaption></figure>

### 2. Comprueba el contenido

Cabinet Report analiza el archivo y puede mostrar su contenido. Comprueba que las secciones, cantidades y materiales reconocidos correspondan al Excel antes de generar el TXT:

<figure><img src="../.gitbook/assets/image (1) (1) (1) (1) (1) (1) (1) (1) (1) (1).png" alt=""><figcaption></figcaption></figure>

### 3. Genera el archivo TXT

Haz clic en **Generar TXT de Producción** cuando la vista previa corresponda con el Excel original.

<figure><img src="../.gitbook/assets/image (2) (1) (1) (1) (1) (1) (1) (1).png" alt=""><figcaption></figcaption></figure>

### 4. Selecciona dónde guardarlo

Selecciona dónde guardar el TXT de Producción. Para conservar una referencia, evita sobrescribir una versión anterior sin una copia de respaldo:

<figure><img src="../.gitbook/assets/image (3) (1) (1) (1) (1) (1) (1) (1).png" alt=""><figcaption></figcaption></figure>

### 5. Verifica y abre el resultado

Cabinet Report le informa que se ha generado y ya lo puede abrir, le muestra los datos del archivo y le pregunta si lo desea abrir, entonces le pide seleccione si es un RP nuevo o es para modificar un RP Anterior:

<figure><img src="../.gitbook/assets/image (4) (1) (1) (1) (1) (1) (1) (1).png" alt=""><figcaption></figcaption></figure>

Haz clic en **Abrir** para acceder al **Reporte de Producción**. Antes de generar u optimizar, **compara el TXT convertido y el reporte abierto con el Excel de origen**: cliente, ambiente, módulos, piezas, cantidades, medidas, materiales y cantos. Si faltan datos, regresa al Excel original y revisa su estructura.

Continúa con [Revisión de Tableros y Cantos](revision-de-tableros-y-cantos.md) y la [guía detallada de la ventana](reporte-de-produccion.md).

<figure><img src="../.gitbook/assets/image (6) (1) (1) (1) (1) (1) (1).png" alt=""><figcaption></figcaption></figure>

---

[← Cargar TXT](cargar-txt.md) · [Reporte en blanco →](reporte-en-blanco.md) · [Índice del Reporte de Producción](README.md) · [🏠 Portal principal](https://danielmelendez-pma.github.io/cabinet-report-partners/)
