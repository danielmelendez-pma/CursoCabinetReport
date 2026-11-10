---
description: Verifica los tableros, cantos, tipos y archivos complementarios antes de continuar con la producción.
---

# Revisión de Tableros y Cantos

Después de abrir un archivo **TXT o CSV**, Cabinet Report presenta la ventana **Revisión de Tableros y Cantos**. Aquí debes comprobar que los materiales del archivo corresponden a los que realmente utilizarás.

<figure><img src="../.gitbook/assets/image (13) (1) (1).png" alt="Ventana de Revisión de Tableros y Cantos al importar un archivo"><figcaption><p>Identifica los materiales detectados antes de continuar.</p></figcaption></figure>

**Continuidad del recorrido:** esta revisión viene después de [Parámetros de Producción](parametros-de-produccion.md), al cargar un [TXT](cargar-txt.md), un [CSV](cargar-csv.md) o un TXT procedente de [RP a TXT](rp-a-txt.md). El paso siguiente es verificar cada pieza en el [Reporte de Producción](reporte-de-produccion.md). La revisión de materiales no reemplaza la conciliación de cantidades y medidas.

## 1. Comprobar los materiales encontrados

La ventana permite revisar los tableros y cantos detectados y verificar su correspondencia con los registros públicos o privados de la base de datos. Esta identificación se utiliza también en las comprobaciones posteriores de la Orden de Producción.

<figure><img src="../.gitbook/assets/image (55).png" alt="Listado para cotejar tableros y cantos con referencias de catálogo"><figcaption><p>Valida tipo, nombre y espesor de cada material.</p></figcaption></figure>

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

<figure><img src="../.gitbook/assets/image (56).png" alt="Totales de tableros y cantos detectados en el archivo"><figcaption><p>Estos totales indican referencias detectadas, no consumo de planchas o canto.</p></figcaption></figure>

## 3. Elegir los archivos complementarios y continuar

Antes de pulsar **Continuar**, selecciona los archivos de **herrajes y perfilerías** que deseas cargar junto con la producción. También puedes utilizar **Cargar todos automáticamente** si corresponde a tu trabajo.

Antes de elegir **Cargar todos automáticamente**, comprueba que los archivos de la carpeta pertenecen al mismo **cliente y ambiente** y que realmente deseas incorporar todos los complementos. Si los seleccionas manualmente, comprueba que no falte ninguno necesario y que no se carguen partidas duplicadas.

Una vez verificados los materiales, los totales y los archivos complementarios, pulsa **Continuar**. En el [Reporte de Producción](reporte-de-produccion.md), contrasta las piezas cargadas con el origen: material, espesor, veta, cantos por lado y cantidades. Si detectas una diferencia, corrígela antes de generar u optimizar el RP.

Consulta también la [referencia oficial del Reporte de Producción](https://cabinet-report.gitbook.io/cabinet-report-docs/funcionalidades-de-cabinet-report/reporte-de-produccion) y el [Stock de tableros](https://cabinet-report.gitbook.io/cabinet-report-docs/funcionalidades-de-cabinet-report/stock-de-tableros) para distinguir el catálogo técnico del consumo real.


## 4. Ensayo reproducible: conciliar materiales antes de cortar

Este ensayo verifica una **transferencia de información**, no el consumo de planchas: una referencia de tablero y canto elegida durante la revisión debe corresponder con las piezas que se observan después en el RP. Realízalo en un **cliente y ambiente de prueba**, nunca sobre un pedido liberado para fabricación.

### Preparar dos piezas que pueden confundirse

Crea una **copia de un TXT compatible** para el ensayo (puedes consultar [Cargar TXT](cargar-txt.md) y [Reporte en Blanco](reporte-en-blanco.md)). Registra dos piezas con el mismo ancho y largo, pero con material y canto diferentes. La tabla es un **ejemplo didáctico**, no un catálogo real ni una regla de cálculo:

| Referencia de ensayo | Cantidad y dimensiones de origen | Tablero previsto | Canto previsto |
| --- | --- | --- | --- |
| A · COSTADO PRUEBA | 1 pieza · 600 × 400 mm | Roble gris, **15 mm** | **Superior:** Roble gris, **0,45 mm**; demás bordes sin canto |
| B · FRENTE PRUEBA | 1 pieza · 600 × 400 mm | Roble gris, **18 mm** | **Derecho:** Roble gris, **2 mm**; demás bordes sin canto |

Antes de importar, registra también la **veta** indicada en el TXT y la identidad exacta de las referencias disponibles en el catálogo (fabricante, código o ficha, si existen). Sustituye los nombres didácticos si no hay materiales equivalentes registrados; **no inventes asociaciones** ni alteres una producción real para completar la prueba. Conserva una copia intacta del TXT de entrada y una lista de resultados esperados.

### Ejecutar y comprobar el traspaso al RP

1. Abre el TXT de prueba mediante **Cargar TXT** y confirma que corresponde al cliente y ambiente de ensayo.
2. En **Revisión de Tableros y Cantos**, compara cada tablero detectado con su ficha: **material, espesor de 15 o 18 mm, color, tipo y referencia**, sin aceptar una coincidencia solo por «Roble gris».
3. Comprueba por separado los **dos cantos de distinto espesor**. Confirma que la elección de tipo **CANTO**, nombre y espesor respeta las referencias previstas; no intercambies 0,45 mm y 2 mm.
4. Revisa los totales mostrados. Si el programa identifica menos referencias de las que esperabas, investiga si combinó nombres o si faltan registros; **el número mostrado no acredita por sí mismo las piezas ni el consumo**.
5. No actives **Cargar todos automáticamente** para completar el ensayo salvo que hayas verificado los complementarios del mismo cliente y ambiente. Continúa con los archivos que correspondan, o sin complementarios si el flujo de prueba lo permite.
6. En el [Reporte de Producción](reporte-de-produccion.md), localiza **A y B** y contrasta con la copia de origen: cantidad **1 + 1**, dimensiones **600 × 400 mm**, espesor de cada pieza, material, veta y **borde exacto** con su respectivo canto.
7. Registra cualquier diferencia y vuelve al origen o al catálogo para corregirla mediante los controles disponibles. **No generes, optimices ni envíes el trabajo a corte** mientras exista una discrepancia sin resolver.

### Resultado esperado y evidencia

| Control | Resultado esperado | Evidencia que debes anotar |
| --- | --- | --- |
| Identidad | Cliente, ambiente y piezas A/B corresponden a la copia de ensayo. | Nombre de archivo, cliente, ambiente y fecha |
| Tableros | A conserva **15 mm** y B **18 mm**, con las referencias correctas. | Material de origen frente a material observado en RP |
| Cantos | A tiene canto **superior de 0,45 mm** y B **derecho de 2 mm**; no aparecen cantos adicionales. | Borde y espesor por pieza antes y después |
| Geometría y cantidades | Ambas piezas siguen con **600 × 400 mm** y cantidad **1** cada una. | Dos filas de origen y filas verificadas en RP |
| Veta y complementarios | No cambia la veta prevista ni se incorporan complementos ajenos al ensayo. | Veta de cada pieza y archivos adicionales seleccionados |

Califica el ensayo como **CONFORME** solo si todas las comparaciones coinciden; **NO CONFORME** si hay una diferencia sin resolver; o **NO EJECUTADO** si faltan referencias, permisos o un TXT de prueba compatible. Anota el resultado observado, la acción correctiva y la persona que verificó. No modifiques el TXT de evidencia para que coincida artificialmente con el RP.

{% hint style="warning" %}
**Límite del ensayo:** demuestra una comprobación manual de asociación y continuidad de datos en una instalación concreta. No acredita una equivalencia comercial de materiales, el comportamiento de todos los importadores, las dimensiones finales tras mecanizado, la optimización ni la autorización de fabricación.
{% endhint %}

---

[← Parámetros de Producción](parametros-de-produccion.md) · [Reporte de Producción →](reporte-de-produccion.md) · [Archivos generados](archivos-de-reportes-generados.md) · [🏠 Portal principal](https://danielmelendez-pma.github.io/cabinet-report-partners/)
