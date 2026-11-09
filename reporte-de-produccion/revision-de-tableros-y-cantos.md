---
description: Verifica los tableros, cantos, tipos y archivos complementarios antes de continuar con la producción.
---

# Revisión de Tableros y Cantos

Después de abrir un archivo **TXT o CSV**, Cabinet Report presenta la ventana **Revisión de Tableros y Cantos**. Aquí debes comprobar que los materiales del archivo corresponden a los que realmente utilizarás.

<figure><img src="../.gitbook/assets/image (13) (1) (1).png" alt=""><figcaption></figcaption></figure>

## 1. Comprobar los materiales encontrados

La ventana permite revisar los tableros y cantos detectados y verificar su correspondencia con los registros públicos o privados de la base de datos. Esta identificación se utiliza también en las comprobaciones posteriores de la Orden de Producción.

<figure><img src="../.gitbook/assets/image (55).png" alt=""><figcaption></figcaption></figure>

Antes de continuar, comprueba lo siguiente:

- **Tableros:** cada uno debe tener el tipo adecuado, por ejemplo **AGL**, **MDF** o **CART**, según corresponda.
- **Cantos:** cada canto debe estar identificado con el tipo **CANTO**.
- **Color del tablero:** si necesitas cambiarlo, selecciónalo en la lista desplegable de la derecha.
- **Nombre del canto:** puedes modificarlo en el campo de la derecha, respetando el formato e indicando el espesor.

{% hint style="warning" %}
**Verificación técnica:** no confirmes automáticamente un material solo porque aparece en la lista. Revisa nombres, tipos y espesores frente al proyecto que vas a fabricar.
{% endhint %}

### Si un tablero o canto no coincide con el catálogo

1. **Contrasta la referencia de origen:** nombre, tipo de material, espesor, color o acabado y, cuando corresponda, orientación de veta. No equipares dos productos únicamente porque tienen nombres similares.
2. **Revisa la asociación propuesta:** comprueba que el registro público o privado elegido describe el material que efectivamente utilizarás. Si hay varias opciones parecidas, utiliza la ficha o especificación del proveedor como referencia.
3. **Comprueba el canto por separado:** identifica su tipo, nombre y espesor, y verifica después los cuatro lados de las piezas a los que se aplica. Un nombre de canto correcto no garantiza que se haya asignado al borde adecuado.
4. **Detén la preparación si no puedes acreditar la equivalencia:** revisa los datos de origen o el registro de material con las herramientas y permisos disponibles antes de fabricar. No fuerces una asociación solo para poder continuar.

{% hint style="info" %}
**Sobre `CART`:** esta lección conserva `CART` como ejemplo de tipo de tablero mostrado en el recorrido. Su definición técnica exacta y cualquier regla de espesor o cálculo asociada no están acreditadas aquí; no las deduzcas de la abreviatura.
{% endhint %}

## 2. Revisar los totales

En la parte inferior de la ventana se muestran las cantidades de **tableros** y **cantos** encontrados en el archivo. Compáralas con la información que esperabas importar para identificar posibles diferencias.

**Distingue identificación de consumo:** estos totales de materiales detectados no deben interpretarse automáticamente como cantidad de planchas que comprar ni como metros de canto necesarios. La estimación y optimización de materiales es una comprobación posterior.

<figure><img src="../.gitbook/assets/image (56).png" alt=""><figcaption></figcaption></figure>

## 3. Elegir los archivos complementarios y continuar

Antes de pulsar **Continuar**, selecciona los archivos de **herrajes y perfilerías** que deseas cargar junto con la producción. También puedes utilizar **Cargar todos automáticamente** si corresponde a tu trabajo.

Antes de elegir **Cargar todos automáticamente**, comprueba que los archivos de la carpeta pertenecen al mismo **cliente y ambiente** y que realmente deseas incorporar todos los complementos. Si los seleccionas manualmente, comprueba que no falte ninguno necesario y que no se carguen partidas duplicadas.

Una vez verificados los materiales, los totales y los archivos complementarios, pulsa **Continuar**. En el [Reporte de Producción](reporte-de-produccion.md), contrasta las piezas cargadas con el origen: material, espesor, veta, cantos por lado y cantidades. Si detectas una diferencia, corrígela antes de generar u optimizar el RP.

Consulta también la [referencia oficial del Reporte de Producción](https://cabinet-report.gitbook.io/cabinet-report-docs/funcionalidades-de-cabinet-report/reporte-de-produccion) y el [Stock de tableros](https://cabinet-report.gitbook.io/cabinet-report-docs/funcionalidades-de-cabinet-report/stock-de-tableros) para distinguir el catálogo técnico del consumo real.

---

[← Parámetros de Producción](parametros-de-produccion.md) · [Reporte de Producción →](reporte-de-produccion.md) · [Archivos generados](archivos-de-reportes-generados.md) · [🏠 Portal principal](https://danielmelendez-pma.github.io/cabinet-report-partners/)
