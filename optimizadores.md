---
description: >-
  Guía práctica para elegir y comprobar los optimizadores de tableros, perfiles
  y superficies antes de entregar archivos de corte a fabricación.
---

# Optimizadores

**Curso de Cabinet Report · Preparación del corte**

Después de revisar el [Reporte de Producción](reporte-de-produccion/README.md), puedes utilizar los optimizadores para planificar el aprovechamiento de materiales. **Optimizar no equivale a fabricar:** una distribución calculada necesita comprobarse con las medidas, la orientación de las piezas, el material realmente disponible y las condiciones del taller.

{% hint style="warning" %}
**Antes de comenzar:** identifica qué material vas a cortar y confirma el origen de las piezas. Los optimizadores de tableros, perfiles y superficies trabajan con restricciones distintas; no se debe aplicar automáticamente el mismo procedimiento a los tres.
{% endhint %}

## 1. Elige la herramienta adecuada

| Material | Herramienta y comprobación principal |
| --- | --- |
| **Tableros y retazos** | Optimización de tableros: ancho y largo de piezas y planchas, espesor, veta, giro, sierra y resane. |
| **Tubos, golas, zócalos y perfiles** | Optimización de perfiles: longitudes útiles, cantidad de tramos y pérdida de corte. |
| **Sobres y superficies** | Optimización de superficies: tamaño de planchas, orientación, resane y compatibilidad de piezas y formatos. |

Consulta las características de cada modalidad en [Optimizadores — Documentación oficial](https://cabinet-report.gitbook.io/cabinet-report-docs/funcionalidades-de-cabinet-report/optimizadores).

## 2. Prepara los datos antes de optimizar

1. **Identifica la producción:** confirma cliente, ambiente, módulo y archivo de origen. Revisa que el RP corresponda a la versión de piezas que deseas cortar.
2. **Revisa piezas y cantidades:** comprueba ancho, largo, espesor, material, veta, cantos y cantidades. No confundas cantidad de piezas con cantidad de módulos.
3. **Comprueba el material de trabajo:** compara el formato comercial y las dimensiones disponibles con el material del RP. Una denominación similar no demuestra que dos tableros sean equivalentes.
4. **Define las restricciones de corte:** ajusta los parámetros que ofrezca el optimizador seleccionado; no des por supuestos el ancho de sierra, el resane, la posibilidad de giro ni la orientación.
5. **Conserva el origen:** guarda una copia identificable del RP y evita modificar simultáneamente dos versiones del listado que luego puedan confundirse.

Para localizar los archivos resultantes de una producción, consulta [Archivos de Reportes Generados](reporte-de-produccion/archivos-de-reportes-generados.md).

## 3. Optimizar tableros y retazos

Esta modalidad organiza piezas rectangulares sobre planchas o retazos compatibles. El procedimiento general documentado es el siguiente:

1. Carga un **TXT de piezas del RP** compatible o incorpora las piezas en la grilla, según la opción disponible.
2. Define las **planchas o retazos** que se considerarán para el cálculo y comprueba sus dimensiones y cantidades.
3. Verifica la correspondencia de **material, espesor, veta y orientación** de cada pieza. Establece el **espesor de sierra**, el **resane** y las reglas de **giro** aplicables.
4. Ejecuta la optimización. En las versiones que los ofrecen, los métodos de ordenamiento incluyen **Guillotina, MenosMas y MasMenos**; la selección no reemplaza la validación del plano de corte.
5. Examina las **planchas empleadas, sobrantes y piezas sin colocar**. Contrasta la distribución con el número de piezas de origen antes de exportar el resultado disponible, como Excel.

{% hint style="info" %}
**Stock del optimizador ≠ inventario físico.** La cantidad de tableros indicada en la herramienta es una entrada para planificar el corte. No demuestra que esas planchas existan en el almacén ni registra por sí sola su consumo.
{% endhint %}

**Control de ejemplo:** si el resultado presenta piezas sin colocar, no entregues únicamente las planchas optimizadas como si fueran el trabajo completo. Revisa la disponibilidad de material, las restricciones y el listado pendiente; vuelve a calcular si corresponde.

## 4. Optimizar tubos, golas y otros perfiles

Los perfiles requieren un **cálculo lineal**, diferente de la distribución de piezas sobre tableros.

1. Selecciona la modalidad de perfiles y carga los datos admitidos por tu versión, por ejemplo un TXT compatible.
2. Comprueba el **tipo de perfil**, la **longitud de cada pieza**, la **cantidad requerida** y la **longitud comercial o útil** del material.
3. Revisa la **pérdida de corte** y el número de barras o tramos introducidos para el cálculo.
4. Compara el resultado con las longitudes pedidas y verifica si queda algún tramo pendiente.
5. Examina el reporte exportado cuando la herramienta permita generar un Excel.

{% hint style="warning" %}
No sustituyas un perfil por otro solo porque sus longitudes coincidan. Revisa denominación, sección, acabado, compatibilidad y existencia física antes de autorizar el corte.
{% endhint %}

## 5. Optimizar sobres y superficies

Esta herramienta contempla piezas de superficies, como **sobres, zócalos, fascias y backsplash**, de acuerdo con los datos admitidos.

1. Revisa las piezas y el formato de entrada que exige tu versión; el flujo documentado contempla **importación y exportación CSV**.
2. Define dimensiones de las planchas, **espesor de corte**, **resane** y **orientación o veta**.
3. Ejecuta el cálculo y examina el aprovechamiento, la distribución y los resultados de exportación disponibles.
4. Comprueba por separado las **uniones, biseles, mecanizados y requisitos de manipulación** que afecten a la fabricación.

El hecho de que el programa distribuya una pieza en una plancha no acredita automáticamente esos trabajos complementarios.

## 6. Verifica los archivos y las condiciones de trabajo

| Elemento | Qué comprobar antes de entregar a corte |
| --- | --- |
| **Listado de piezas** | Correspondencia con el RP revisado, cantidades y materiales, incluidas las piezas que no pudieron colocarse. |
| **Plano o resultado** | Orientación, veta, giro, retazos, resane y pérdida de corte acordes con la máquina y el operario. |
| **Disponibilidad** | Que las planchas, barras o superficies existan realmente; las cantidades introducidas no son una constatación de inventario. |
| **Exportación** | Que el archivo se abra, contenga el resultado esperado y sea compatible con la herramienta o maquinaria de destino. |
| **Cambios posteriores** | Si corriges medidas, cantidades o materiales del RP, vuelve a validar la optimización antes de distribuirla. |

Los formatos como **TXT, CSV y Excel (.xlsx)** cumplen funciones distintas. También existen intercambios condicionados por herramientas externas, como **Optiplanning** e **Itemizer**. No presupongas compatibilidad universal con todo archivo o maquinaria.

{% hint style="info" %}
**Trabajo sin conexión:** algunos optimizadores pueden recurrir a copias locales de catálogos. Si no están disponibles o actualizadas, puede requerirse conexión previa. Comprueba los materiales cargados y no supongas que una sesión offline sincroniza automáticamente sus datos.
{% endhint %}

## 7. Ejercicio de comprobación

1. Elige una producción ya revisada y registra cuántas piezas corresponden a cada material.
2. Utiliza el optimizador adecuado e introduce las restricciones reales de corte.
3. Compara las piezas de entrada con las colocadas y las que quedaron pendientes.
4. Abre el archivo resultante y comprueba material, orientación y cantidades antes de entregarlo al taller.
5. Si encuentras una discrepancia, corrige el origen o el parámetro correspondiente y repite el control.

**Resultado esperado del ejercicio:** identificar claramente lo que se consiguió distribuir y lo que todavía requiere intervención. No se considera suficiente que el programa muestre una operación finalizada.

## Continúa tu recorrido

[Reporte de Producción](reporte-de-produccion/README.md) · [Archivos de reportes generados](reporte-de-produccion/archivos-de-reportes-generados.md) · [Orden de Producción](orden-de-produccion.md) · [Optimizadores — Documentación oficial](https://cabinet-report.gitbook.io/cabinet-report-docs/funcionalidades-de-cabinet-report/optimizadores)

---

[← Volver a la portada del Curso](README.md) · [🏠 Portal principal](https://danielmelendez-pma.github.io/cabinet-report-partners/)
