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

### Comprueba la importación, no solo la apertura

- **TXT de piezas del RP:** utiliza la entrada admitida por el optimizador de tableros o perfiles. Identifica el TXT correcto y revisa columnas, unidades, cantidad por pieza, material y medidas *después* de cargarlo. Un **TXT de parámetros**, un listado de materiales y un archivo específico de seccionadora no son sustitutos automáticos del TXT de piezas. Consulta [Cargar TXT](reporte-de-produccion/cargar-txt.md) para conocer la distinción entre origen, estructura y datos recuperados del RP.
- **CSV de superficies:** verifica el esquema que admite esa herramienta y observa cómo interpreta identificadores, cantidades, dimensiones y materiales. Comprueba también separador, formato numérico y unidades del archivo concreto; **no existe aquí una especificación universal de CSV**. La lección [Cargar CSV al RP](reporte-de-produccion/cargar-csv.md) describe *otro* punto de entrada y no certifica la compatibilidad con el optimizador de superficies.
- **Control posterior:** compara el número de referencias y las **cantidades efectivas por referencia** con el origen, no solamente el número de filas visibles. Si una pieza desaparece, se multiplica, cambia de material o presenta medidas inválidas, detén el ensayo y corrige la fuente o la configuración antes de optimizar.

Cambiar la extensión de un archivo a `.txt` o `.csv` **no convierte** su estructura. Conserva el original inalterado y documenta cualquier transformación de datos realizada fuera de Cabinet Report.

## 3. Optimizar tableros y retazos

Esta modalidad organiza piezas rectangulares sobre planchas o retazos compatibles. **Una pieza no es intercambiable solo por tener la misma medida:** comprueba material, espesor, acabado y veta cuando corresponda. Los retazos introducidos son candidatos al cálculo; su posibilidad real de reutilización depende de dimensiones útiles, estado físico e identificación.

El procedimiento general documentado es el siguiente:

1. Carga un **TXT de piezas del RP** compatible o incorpora las piezas en la grilla, según la opción disponible.
2. Define las **planchas o retazos** que se considerarán para el cálculo y comprueba sus dimensiones y cantidades.
3. Verifica la correspondencia de **material, espesor, veta y orientación** de cada pieza. Establece el **espesor o ancho de sierra**, el **resane** y las reglas de **giro** aplicables a esa máquina y material. No autorices un giro que cambie la veta exigida ni des por supuesto que el optimizador admite todos los giros o restricciones.
4. Ejecuta la optimización. En las versiones que los ofrecen, los métodos de ordenamiento incluyen **Guillotina, MenosMas y MasMenos**; la selección no reemplaza la validación del plano de corte.
5. Examina las **planchas empleadas, sobrantes y piezas sin colocar**. Concilia cada referencia y cantidad con el TXT o la grilla original: **requeridas = colocadas + pendientes**, siempre que todas las categorías estén correctamente identificadas en el resultado. Si la salida no permite comprobar esa igualdad por pieza, consérvala como **no verificada** hasta hacer el cotejo manual. Solo entonces revisa la exportación disponible, como Excel.

{% hint style="info" %}
**Stock del optimizador ≠ inventario físico.** La cantidad de tableros indicada en la herramienta es una entrada para planificar el corte. No demuestra que esas planchas existan en el almacén ni registra por sí sola su consumo.
{% endhint %}

**Control de ejemplo:** si el resultado presenta piezas sin colocar, no entregues únicamente las planchas optimizadas como si fueran el trabajo completo. Revisa la disponibilidad de material, las restricciones y el listado pendiente; vuelve a calcular si corresponde.

### Registro de conciliación por referencia

| Campo de control | Acción manual |
| --- | --- |
| **Origen** | Anota identificador o agrupación demostrablemente equivalente, material, espesor, dimensiones y cantidad requerida. |
| **Colocadas** | Comprueba las unidades efectivamente presentes en el plano o reporte de la ejecución elegida. |
| **Pendientes** | Identifica las no colocadas y evita interpretarlas como piezas cortadas o descartadas. |
| **Diferencias** | Investiga piezas repetidas, ausentes, modificadas o atribuidas al material equivocado, aunque coincida el total general. |

Cuando una salida agrupa referencias idénticas y no conserva el módulo, **no reconstruyas una procedencia que el archivo no demuestra**. Contrasta las agrupaciones con el RP original y guarda la evidencia del cotejo.

## 4. Optimizar tubos, golas y otros perfiles

Los perfiles requieren un **cálculo lineal**, diferente de la distribución de piezas sobre tableros.

1. Selecciona la modalidad de perfiles y carga los datos admitidos por tu versión, por ejemplo un TXT compatible.
2. Comprueba el **tipo de perfil**, la **longitud de cada pieza**, la **cantidad requerida** y la **longitud comercial o útil** del material.
3. Revisa la **pérdida de corte**, los extremos que requieren preparación cuando aplique y el número de barras o tramos introducidos para el cálculo. Comprueba que la longitud útil permita obtener los cortes propuestos; no inventes una fórmula de descuento fija para todos los perfiles o máquinas.
4. Compara el resultado con las longitudes pedidas **por tipo de perfil y cantidad**; revisa cortes colocados, pendientes y sobrantes identificables. Un total de metros parecido no demuestra equivalencia de secciones o acabados.
5. Examina el reporte exportado cuando la herramienta permita generar un Excel.

{% hint style="warning" %}
No sustituyas un perfil por otro solo porque sus longitudes coincidan. Revisa denominación, sección, acabado, compatibilidad y existencia física antes de autorizar el corte.
{% endhint %}

**Antes de cortar barras:** verifica con el responsable de máquina la longitud útil real, topes, sujeción, orden de cortes y desperdicio. Una distribución lineal calculada no certifica la seguridad de sujeción ni reemplaza las instrucciones de fabricación.

## 5. Optimizar sobres y superficies

Esta herramienta contempla piezas de superficies, como **sobres, zócalos, fascias y backsplash**, de acuerdo con los datos admitidos.

1. Revisa las piezas y el formato de entrada que exige tu versión; el flujo documentado contempla **importación y exportación CSV**.
2. Define dimensiones de las planchas, **espesor de corte**, **resane** y **orientación o veta**.
3. Ejecuta el cálculo y examina el aprovechamiento, la distribución y los resultados de exportación disponibles.
4. Comprueba por separado las **uniones, biseles, mecanizados y requisitos de manipulación** que afecten a la fabricación.

El hecho de que el programa distribuya una pieza en una plancha no acredita automáticamente esos trabajos complementarios.

**Control del CSV y de las superficies:** antes de utilizar la salida, comprueba piezas importadas frente al archivo original, unidades y formato, planchas efectivamente consideradas, orientación y pendientes. En el taller valida además uniones, cantos vistos, plantillas, cortes especiales y manipulación. **No atribuyas al optimizador el cálculo de biseles o uniones si no se han comprobado para la versión y el material.**

## 6. Verifica los archivos y las condiciones de trabajo

| Elemento | Qué comprobar antes de entregar a corte |
| --- | --- |
| **Listado de piezas** | Correspondencia con el RP revisado, cantidades y materiales, incluidas las piezas que no pudieron colocarse. |
| **Plano o resultado** | Orientación, veta, giro, retazos, resane y pérdida de corte acordes con la máquina y el operario. |
| **Disponibilidad** | Que las planchas, barras o superficies existan realmente; las cantidades introducidas no son una constatación de inventario. |
| **Exportación** | Que el archivo se abra, contenga el resultado esperado y sea compatible con la herramienta o maquinaria de destino. |
| **Cambios posteriores** | Si corriges medidas, cantidades o materiales del RP, vuelve a validar la optimización antes de distribuirla. |

### Interpreta el aprovechamiento y los archivos de salida

**Planchas utilizadas** indica el material que el cálculo asignó al plano; **retazos o sobrantes mostrados** no prueban que su recuperación sea rentable, segura o físicamente posible. Una tasa de aprovechamiento debe leerse con el **denominador, unidades y alcance que informe la herramienta**: no confundas área ocupada con rendimiento económico ni compares porcentajes calculados con bases diferentes. Si esos datos no aparecen, registra **«no informado»** en lugar de estimarlos como resultados del programa.

| Formato o intercambio | Verificación necesaria |
| --- | --- |
| **TXT de piezas RP** | Origen, estructura admitida, medidas, materiales y cantidades importadas. |
| **CSV de superficies** | Columnas y unidades reconocidas por ese importador; integridad de la entrada y salida. |
| **Excel (.xlsx)** | Que abra, corresponda a la corrida elegida y conserve piezas y parámetros necesarios para su uso. |
| **Optiplanning e Itemizer** | Formato y modalidad concreta disponible, versión y aceptación de importación por el destino. |

Los formatos **TXT, CSV y Excel** no son intercambiables por renombrado. Las rutinas relacionadas con **Optiplanning** e **Itemizer** están documentadas para ciertos flujos de producción; **no se garantiza que todas las versiones, formatos o máquinas los admitan**. Consulta también [Archivos de Reportes Generados](reporte-de-produccion/archivos-de-reportes-generados.md) para reconocer la salida específica de una seccionadora.

{% hint style="info" %}
**Trabajo sin conexión:** los optimizadores de **tableros y perfiles** contemplan rutas que recurren a copias locales de catálogos. Si faltan o están desactualizadas, puede requerirse conexión previa; las operaciones remotas pueden tener otras restricciones. Comprueba las referencias efectivamente cargadas y **no supongas sincronización automática**, ni extiendas este comportamiento a superficies sin evidencia.
{% endhint %}

### Recuperación ante resultados incompletos o errores

1. **Importación vacía, incompleta o incompatible:** conserva el TXT/CSV de origen; comprueba tipo de archivo, estructura, medidas, cantidades y versión antes de volver a importarlo. No edites el único original.
2. **Piezas pendientes o plano inviable:** identifica por referencia qué falta y qué restricción lo impide. Revisa material, espesor, planchas/tramos, veta, giro, sierra y resane; vuelve a calcular **solo después** de documentar los cambios.
3. **Catálogo no disponible o referencia dudosa:** verifica qué datos locales están cargados y la conexión si corresponde; no sustituyas silenciosamente materiales por otros supuestamente equivalentes.
4. **Exportación ausente o ilegible:** distingue fallo de cálculo, de generación y de apertura/lectura en destino. Conserva la última entrada válida y el resultado visible, sin dar por entregado un archivo que no se pudo comprobar.
5. **Registrar incidencia:** conserva versión del programa, modalidad/método, parámetros, identificadores del RP, entrada y salida **sin credenciales ni datos sensibles**, mensaje y pasos reproducibles. Consulta [Reporte de Errores o Feedback](reporte-de-errores-o-feedback.md). No atribuyas a la aplicación recuperaciones automáticas de sesiones o archivos no verificadas.

## 7. Ejercicio de comprobación

1. Elige una producción ya revisada y registra cuántas piezas corresponden a cada material.
2. Utiliza el optimizador adecuado e introduce las restricciones reales de corte.
3. Compara las piezas de entrada con las colocadas y las que quedaron pendientes.
4. Abre el archivo resultante y comprueba material, orientación y cantidades antes de entregarlo al taller.
5. Si encuentras una discrepancia, corrige el origen o el parámetro correspondiente y repite el control.

**Resultado esperado del ejercicio:** identificar claramente lo que se consiguió distribuir y lo que todavía requiere intervención. No se considera suficiente que el programa muestre una operación finalizada.

**Decisión documentada por el taller (no estado automático de Cabinet Report):** **APTO PARA REVISIÓN DE CORTE** cuando se conciliaron piezas, cantidades, materiales, restricciones y archivos; **DETENER ENTREGA** cuando existe una diferencia no resuelta; **NO VERIFICADO** cuando faltan datos, lectura de destino o autorización. Incluso una alternativa «apta para revisión» necesita aprobación del responsable y comprobación física antes de ejecutar el corte.

## 8. Ensayo comparativo: métodos de ordenamiento con el mismo lote

El optimizador de tableros documenta los métodos **Guillotina, MenosMas y MasMenos**. Este ensayo permite **comparar sus resultados bajo condiciones idénticas**, en vez de suponer que el método que utiliza menos planchas, o que termina primero, será necesariamente el adecuado para el taller. No presupone que los tres métodos entreguen distribuciones distintas ni que exista un método universalmente superior.

### Preparar una referencia única

1. Selecciona **una producción de prueba ya revisada**, con un TXT compatible, y conserva una copia intacta del archivo de origen. No uses como prueba un pedido que ya se haya liberado a fabricación.
2. Registra la **versión del programa, cliente, ambiente y referencia del RP**. Para cada pieza del lote, identifica módulo o pieza suelta, cantidad, ancho, largo, espesor, material, veta y orientación permitida. Conserva también los cantos por lado para cotejar la identidad de cada pieza con el RP, aunque el plano de optimización no muestre esos atributos.
3. Fija **el mismo conjunto de planchas y retazos** para las tres ejecuciones: material, dimensiones, cantidades introducidas, sierra, resane y reglas de giro. Las cantidades indicadas al optimizador **no acreditan existencias físicas**.
4. Utiliza el mismo archivo y la misma configuración en todas las corridas. Si necesitas cambiar un parámetro, inicia una **comparación nueva** y deja constancia del motivo; no mezcles resultados de configuraciones diferentes.

### Ejecutar y registrar la comparación

1. Ejecuta **Guillotina** y guarda su resultado o evidencia disponible; repite desde la **misma entrada** con **MenosMas** y después con **MasMenos**, únicamente si esos métodos están disponibles en tu versión. Los nombres A, B y C, si los utilizas para guardar copias, son etiquetas manuales del ensayo.
2. Para cada método, comprueba **qué piezas quedaron colocadas y cuáles pendientes**, por referencia y cantidad. Un total global idéntico no demuestra que se hayan distribuido las mismas piezas.
3. Compara **cantidad y formato de planchas empleadas, aprovechamiento o retazos informados, posición y giro de piezas, resanes y viabilidad del plano** para tu máquina y secuencia de corte. Anota solo las métricas que el resultado realmente muestre; no infieras desperdicios ni rendimiento a partir de una captura incompleta.
4. Si exportas a Excel, **abre cada archivo por separado** y comprueba que pertenece al método y al lote anotados. Un archivo exportado no valida automáticamente su compatibilidad con la seccionadora.
5. Solicita al responsable del corte que revise las alternativas **técnicamente completas**. Si se elige una, conserva la justificación de selección y evita entregar las otras al operario como si todas fueran órdenes vigentes.

| Control de comparación | Guillotina | MenosMas | MasMenos |
| --- | --- | --- | --- |
| Referencia del mismo TXT y parámetros | Registrar | Registrar | Registrar |
| Piezas colocadas y pendientes, por identificación | Registrar | Registrar | Registrar |
| Planchas, retazos y aprovechamiento mostrado | Registrar | Registrar | Registrar |
| Orientación, giro, sierra y resane | Verificar | Verificar | Verificar |
| Archivo o captura y conformidad del operador | Registrar | Registrar | Registrar |

**Cómo leer una diferencia:** si un método emplea menos planchas pero deja una referencia requerida sin colocar, **no es una solución completa** para el lote; si dos métodos completan todas las piezas, su elección puede depender de secuencia de corte, orientación, calidad de retazos, operario y máquina, no solo de un porcentaje. Estas son reglas del **ensayo manual**, no resultados atribuidos a Guillotina, MenosMas ni MasMenos.

**Interpretación del resultado:**

- **CONFORME:** se registraron las condiciones idénticas, se conciliaron las piezas de cada salida con el origen y la alternativa escogida fue revisada como viable por el responsable de corte. Que dos métodos generen planos diferentes **no significa por sí solo que uno tenga un error**.
- **NO CONFORME:** alguna salida omite piezas sin advertirlo, se compararon lotes o parámetros distintos, se eligió un plano incompatible con la veta o la máquina, o faltó resolver una discrepancia antes de entregar a fabricación.
- **NO EJECUTADO:** no se corrieron las opciones necesarias, alguna no existe en la versión instalada o faltan archivos y evidencias suficientes. Registra cualquier comparación parcial, pero **no declares validada la comparación de los tres métodos**.

{% hint style="warning" %}
**Alcance:** se trata de una comprobación manual reproducible con datos reales de ensayo, no de una certificación de algoritmos, una prueba funcional ya ejecutada ni una selección automática del mejor corte. Sigue siendo necesario comprobar el inventario físico y autorizar una única salida para fabricación.
{% endhint %}

## Continúa tu recorrido

[Reporte de Producción](reporte-de-produccion/README.md) · [Archivos de reportes generados](reporte-de-produccion/archivos-de-reportes-generados.md) · [Orden de Producción](orden-de-produccion.md) · [Reporte de Compras](reporte-de-compras.md) · [Reporte de Errores o Feedback](reporte-de-errores-o-feedback.md) · [Optimizadores — Documentación oficial](https://cabinet-report.gitbook.io/cabinet-report-docs/funcionalidades-de-cabinet-report/optimizadores)

---

[← Volver a la portada del Curso](README.md) · [🏠 Portal principal](https://danielmelendez-pma.github.io/cabinet-report-partners/)
