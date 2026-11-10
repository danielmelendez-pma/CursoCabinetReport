# Reporte de Producción

**Etapa del curso · Preparación de la producción**

El Reporte de Producción agrupa distintas formas de comenzar o recuperar un trabajo. Identifica primero el origen de los datos y elige la lección que corresponda; las opciones no son pasos que debas ejecutar todas en orden.

**Accesos por objetivo:** [Cargar CSV](cargar-csv.md) · [Cargar TXT](cargar-txt.md) · [RP a TXT](rp-a-txt.md) · [Reporte en Blanco](reporte-en-blanco.md).

## Elige cómo comenzar

| Si tienes… | Utiliza… | Comprueba antes de continuar |
| --- | --- | --- |
| Un CSV exportado desde un programa de diseño | [Cargar CSV](cargar-csv.md) | La compatibilidad de los campos y del importador. |
| Un TXT de producción compatible | [Cargar TXT](cargar-txt.md) | Cliente, ambiente, columnas y datos de las piezas. |
| Un Excel RP de Cabinet Report que editaste | [RP a TXT](rp-a-txt.md) | Que la estructura original de la hoja se conserva. |
| Solo las medidas y los datos de piezas por ingresar | [Reporte en Blanco](reporte-en-blanco.md) | El cliente, ambiente y materiales que registrarás. |

**Importante:** estas son alternativas de entrada, no cuatro pasos consecutivos. Si buscas las herramientas de edición y generación, continúa en la [guía detallada de la ventana](reporte-de-produccion.md).

Al hacer clic en **Reporte de Producción** se despliega un menú con estas opciones. Cada apartado incluye su captura y el enlace a la explicación detallada:

<figure><img src="../.gitbook/assets/image (49).png" alt="Menú de Reporte de Producción con las diferentes opciones de entrada"><figcaption><p>Elige una alternativa según el origen de la información; no necesitas ejecutar las cuatro.</p></figcaption></figure>

## <mark style="color:$primary;">**Cargar CSV**</mark>

Permite importar un archivo CSV con la estructura admitida por el importador de Cabinet Report. **No basta que el archivo termine en `.csv`**: comprueba formato, procedencia y datos importados. La referencia histórica a Promob y el control «Importar CSV de CutPro» no demuestran equivalencia entre exportadores.

<figure><img src="../.gitbook/assets/image (50).png" alt="Opción Cargar CSV en el menú de Reporte de Producción" width="155"><figcaption><p>Entrada desde un CSV de diseño. <a href="cargar-csv.md">Abrir la guía Cargar CSV</a>.</p></figcaption></figure>

## <mark style="color:$primary;">**Cargar TXT**</mark>

Abre un TXT de producción compatible, incluido el generado por Cabinet Report o por el Catálogo de Módulos. Los TXT de otras aplicaciones requieren una estructura compatible; **abrirlo no confirma que se recuperaron todos los datos auxiliares**.

<figure><img src="../.gitbook/assets/image (51).png" alt="Opción Cargar TXT en el menú de Reporte de Producción" width="155"><figcaption><p>Entrada desde un TXT de producción. <a href="cargar-txt.md">Abrir la guía Cargar TXT</a>.</p></figcaption></figure>

## <mark style="color:$primary;">**RP a TXT**</mark>

Convierte un Excel RP previamente generado por Cabinet Report en un TXT de producción, por ejemplo después de editar datos del reporte. **Conserva el diseño original del Excel**, guarda una copia y verifica el TXT resultante antes de abrirlo.

<figure><img src="../.gitbook/assets/image (52).png" alt="Opción RP a TXT en el menú de Reporte de Producción" width="156"><figcaption><p>Conversión de un Excel RP a TXT. <a href="rp-a-txt.md">Abrir la guía RP a TXT</a>.</p></figcaption></figure>

## <mark style="color:$primary;">**Reporte en Blanco**</mark>

Prepara manualmente un TXT de producción incorporando piezas, sin partir de una importación CSV o de un Excel RP. Distingue entre **crear un TXT nuevo** y **abrir uno existente** antes de editar piezas sueltas o piezas de un módulo.

<figure><img src="../.gitbook/assets/image (53).png" alt="Opción Reporte en Blanco en el menú de Reporte de Producción" width="156"><figcaption><p>Entrada manual de piezas. <a href="reporte-en-blanco.md">Abrir la guía Reporte en Blanco</a>.</p></figcaption></figure>

## Completa el recorrido del Reporte de Producción

Una vez seleccionado el punto de entrada, continúa con las lecciones que correspondan a tu trabajo:

1. [**Parámetros de Producción**](parametros-de-produccion.md): consulta los parámetros aplicables.
2. [**Revisión de Tableros y Cantos**](revision-de-tableros-y-cantos.md): comprueba la información de materiales y cantos.
3. [**Reporte de Producción**](reporte-de-produccion.md): conoce la ventana y sus herramientas.
4. [**Archivos de Reportes Generados**](archivos-de-reportes-generados.md): identifica los documentos resultantes.

## Control de continuidad antes de generar

Tras completar **una sola ruta de entrada**, haz esta comprobación de aprendizaje sobre un trabajo de prueba o una copia respaldada:

1. **Conserva el origen:** identifica archivo o ficha manual, cliente, ambiente y parámetros aplicados. Evita sobrescribir la única versión de una producción real.
2. **Concilia lo cargado:** compara **unidades efectivas** por pieza (no solo filas), módulos o piezas sueltas, espesor, medidas, material, veta y **canto por lado** con la fuente aprobada.
3. **Revisa por separado los complementos:** el TXT de piezas no demuestra por sí mismo la recuperación de accesorios, ferretería, golas, tubos, zócalos o registros técnicos; consulta [Archivos de Reportes Generados](archivos-de-reportes-generados.md).
4. **Decide si continuar:** si aparecen piezas faltantes, cantidades diferentes o datos sin acreditar, detén la generación y corrige la causa. Solo después de conciliar la información continúa con la revisión de materiales y con la ventana del RP.

**Resultado del ejercicio:** anota «Coincide», «Diferencia justificada» o «Pendiente» para cada control. No marques «Coincide» cuando un dato no sea visible o no se haya podido comprobar.

Para una descripción funcional de las comprobaciones y del análisis asistido, consulta la [**Documentación oficial del Reporte de Producción**](https://cabinet-report.gitbook.io/cabinet-report-docs/funcionalidades-de-cabinet-report/reporte-de-produccion).

{% hint style="warning" %}
**Antes de fabricar:** revisa las medidas, cantidades, materiales, cantos y archivos exportados. Una generación o revisión completada no confirma por sí sola que toda la información sea correcta.
{% endhint %}

[← Portada del Curso](../README.md) · [Explorador de Proyectos](../explorador-de-proyectos.md) · [🏠 Portal principal](https://danielmelendez-pma.github.io/cabinet-report-partners/)
