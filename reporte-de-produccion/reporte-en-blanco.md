---
description: Crea un Reporte de Producción manual desde cero, agrega piezas sueltas o módulos y verifica el archivo TXT resultante.
---

# Reporte en Blanco

Desde **Reporte Manual** puedes preparar un archivo TXT de producción sin partir de un reporte existente. También puedes abrir un TXT compatible para continuar el trabajo. **Crear uno nuevo y abrir uno existente son alternativas**, no pasos consecutivos.

## Antes de empezar

- Identifica el **cliente y ambiente** de esta producción.
- Ten a mano las medidas del despiece y los **materiales, espesores, vetas y cantos** previstos.
- Decide si trabajarás con **piezas sueltas** o con piezas de **un módulo**: la cantidad y el contexto de medidas se revisan de manera distinta.
- Si continuarás un TXT anterior, conserva una copia y comprueba que corresponda a este proyecto.

Para preparar fórmulas reutilizables consulta [Creación de Piezas](../creacion-de-piezas.md) y [Fórmulas y Variables](../formulas-y-variables.md). Para comparar los puntos de entrada al RP consulta su [índice](README.md).

<figure><img src="../.gitbook/assets/image (9) (1) (1) (1) (1).png" alt="Pantalla de entrada al Reporte Manual de Cabinet Report"><figcaption><p>Entrada para preparar piezas sin importar previamente un CSV o TXT.</p></figcaption></figure>

## 1. Identificar la producción

Elige **una sola** de estas rutas según tu punto de partida:

- **TXT nuevo:** escribe el **nombre del cliente** y el **ambiente** y selecciona **Crear Nuevo**.
- **TXT existente:** utiliza la opción para **abrir un archivo TXT** y confirma su cliente, ambiente y contenido antes de editarlo.

No es necesario crear otro archivo si vas a continuar una producción compatible que ya existe.

<figure><img src="../.gitbook/assets/image (1) (1) (1) (1) (1) (1) (1) (1) (1).png" alt="Campos de identificación del cliente y ambiente para crear un TXT nuevo"><figcaption><p>Identifica el cliente y el ambiente antes de seleccionar Crear Nuevo.</p></figcaption></figure>

{% hint style="warning" %}
**Campos obligatorios:** si intentas crear un TXT nuevo sin indicar cliente y ambiente, Cabinet Report no permite continuar. Completa ambos datos antes de volver a intentarlo.
{% endhint %}

<figure><img src="../.gitbook/assets/image (2) (1) (1) (1) (1) (1) (1).png" alt="Aviso por ausencia de datos necesarios al crear el archivo de producción"><figcaption><p>Completa los datos requeridos del trabajo antes de intentarlo nuevamente.</p></figcaption></figure>

## 2. Configurar los parámetros

Selecciona los parámetros de producción que correspondan al trabajo antes de agregar piezas. Contrasta las opciones disponibles en tu versión con los materiales y procesos previstos: **vetas, automatizaciones y tipo de reporte**, cuando apliquen. Consulta [Parámetros de Producción](parametros-de-produccion.md). Una automatización activada no valida las medidas por sí sola.

<figure><img src="../.gitbook/assets/image (3) (1) (1) (1) (1) (1) (1).png" alt="Ventana de selección de parámetros para el reporte manual"><figcaption><p>Comprueba vetas y automatizaciones aplicables a la producción de prueba.</p></figcaption></figure>

## 3. Elegir cómo incorporar las piezas

### Opción A: piezas sueltas

Activa la opción de **piezas sueltas** si vas a agregar piezas de forma independiente al listado.

<figure><img src="../.gitbook/assets/image (4) (1) (1) (1) (1) (1) (1).png" alt="Opción para trabajar con piezas sueltas en el reporte manual"><figcaption><p>Usa esta alternativa para piezas independientes del listado de módulos.</p></figcaption></figure>

### Opción B: piezas de un módulo

Si trabajarás con un **módulo completo**, activa esa opción e introduce las dimensiones del módulo. Confirma las referencias de **profundidad, ancho y alto** que se utilizarán para interpretar las piezas. No confundas las dimensiones exteriores del mueble con las medidas efectivas de cada pieza.

<figure><img src="../.gitbook/assets/image (5) (1) (1) (1) (1) (1) (1).png" alt="Opción de módulo completo con sus dimensiones de referencia"><figcaption><p>Confirma profundidad, ancho y alto como referencias del módulo.</p></figcaption></figure>

## 4. Agregar las piezas al listado

Puedes utilizar cualquiera de estos dos métodos:

### Método 1: ingreso manual

Agrega las piezas directamente en el listado de piezas.

<figure><img src="../.gitbook/assets/image (6) (1) (1) (1) (1) (1).png" alt="Listado del reporte manual para agregar piezas directamente"><figcaption><p>Revisa cantidad, medidas y material por pieza antes de incorporarla.</p></figcaption></figure>

### Método 2: selección desde la base de datos

Coloca el listado de piezas de la base de datos junto al área de trabajo y agrega desde allí las piezas que necesites.

<figure><img src="../.gitbook/assets/image (7) (1) (1) (1) (1) (1).png" alt="Selección de piezas guardadas en la base de datos para el reporte manual"><figcaption><p>La pieza elegida desde el catálogo aún requiere comprobación técnica.</p></figcaption></figure>

Cuando hayas incorporado todas las piezas del módulo que estás preparando, revisa el listado antes de continuar. Tanto para el ingreso manual como para la selección desde la base de datos, comprueba:

1. **Nombre y función:** que no falten piezas necesarias ni haya duplicados accidentales.
2. **Cantidad y pertenencia:** unidades correctas y clasificación coherente como módulo o pieza suelta.
3. **Medidas:** espesor, ancho, largo y orientación compatibles con el diseño.
4. **Material y acabado:** tablero, veta y cantos de cada borde.

Una definición guardada en la base de datos **no queda validada automáticamente** para un módulo con parámetros distintos.

<figure><img src="../.gitbook/assets/image (8) (1) (1) (1) (1) (1).png" alt="Listado de piezas preparadas antes de incorporarlas al TXT"><figcaption><p>Concilia el listado de piezas del módulo con el diseño de referencia.</p></figcaption></figure>

## 5. Incorporar las piezas al archivo TXT

Utiliza la acción indicada en la pantalla para añadir las piezas al reporte. **Incorporar piezas al TXT no equivale a generar u optimizar la producción final**: el resultado debe comprobarse antes de continuar con el RP.

<figure><img src="../.gitbook/assets/image (12) (1) (1) (1).png" alt="Control para incorporar las piezas preparadas al archivo TXT"><figcaption><p>Incorpora las piezas al archivo; esta acción no genera el RP final.</p></figcaption></figure>

Si todavía no has creado un archivo TXT ni has abierto uno existente, Cabinet Report solicitará hacerlo antes de continuar.

<figure><img src="../.gitbook/assets/image (13) (1) (1) (1).png" alt="Aviso para crear o abrir un TXT antes de incorporar piezas"><figcaption><p>Identifica el TXT de destino para evitar trabajar sobre un archivo equivocado.</p></figcaption></figure>

Cuando el proceso se completa, se muestra el mensaje de confirmación de incorporación de piezas.

<figure><img src="../.gitbook/assets/image (14) (1) (1).png" alt="Mensaje de confirmación de incorporación de piezas al TXT"><figcaption><p>El mensaje confirma la operación, pero no valida automáticamente el contenido.</p></figcaption></figure>

## 6. Verificar el resultado

Comprueba que el archivo TXT se haya creado o actualizado correctamente y que incluya las piezas previstas.

| Comprobación | Qué contrastar |
| --- | --- |
| **Identificación** | Cliente, ambiente y archivo nuevo o existente según el recorrido elegido. |
| **Integridad** | Piezas previstas, sin omisiones ni duplicados accidentales. |
| **Cantidades** | Unidades de cada pieza y módulo acordes con el proyecto. |
| **Datos técnicos** | Espesor, ancho, largo, material, veta y cantos por lado. |
| **Resultado** | El TXT actualizado se localiza y pertenece a la producción preparada. |

## Ensayo reproducible: comprobar un reporte creado manualmente

Este ejercicio verifica la **captura, incorporación y lectura posterior** de piezas en un TXT creado desde Reporte Manual. Los valores son **didácticos**: no proceden de una fórmula del software ni representan un diseño autorizado para cortar.

### 1. Preparar una producción de prueba

1. Trabaja con un **cliente y ambiente de ensayo claramente identificados**, distintos de cualquier orden real. Selecciona **Crear Nuevo**; no abras ni modifiques el único TXT de una producción en curso.
2. En los parámetros de producción, anota las opciones que puedan cambiar nombres, orientación, medidas o cantidades. Para comparar contra los datos originales, registra cualquier automatización que permanezca activa en tu versión.
3. Elige la ruta **piezas sueltas** y localiza en tu catálogo un tablero y un canto válidos. Anota sus referencias y el espesor. Si el material no existe o no coincide con el previsto, no lo sustituyas silenciosamente.
4. Prepara esta hoja de control **antes** de introducir datos. La referencia del catálogo utilizada será la misma en las dos piezas, pero los lados de canto previstos serán diferentes.

### 2. Introducir datos y calcular el total esperado

| Pieza didáctica | Cantidad | Espesor | Ancho | Largo | Canto de prueba |
| --- | ---: | ---: | ---: | ---: | --- |
| Pieza A | 2 | 18 mm | 300 mm | 400 mm | Canto seleccionado en el borde superior |
| Pieza B | 1 | 18 mm | 300 mm | 400 mm | Canto seleccionado en el borde inferior |
| **Total previsto** | **3 unidades** | | | | **2 referencias de pieza** |

Para que el ejercicio sea comparable, utiliza en ambas piezas el **mismo material real seleccionado del catálogo** y registra la veta de acuerdo con su ficha. Deja sin canto los otros bordes **solo en este ensayo**, no como regla para un mueble real. La orientación que convierte un borde en frontal depende de la pieza: no supongas que «superior» significa «frontal».

**Control clave:** dos piezas con las mismas tres dimensiones no son necesariamente intercambiables. El nombre, la cantidad y el **lado del canto** son datos independientes. El total esperado es de **tres unidades**, aunque el listado muestre dos referencias o agrupe filas de otra forma.

### 3. Incorporar y comprobar el TXT

1. Introduce cada referencia **una sola vez** con la cantidad indicada. Antes de incorporar, revisa material, veta y los cuatro lados de canto de cada pieza.
2. Ejecuta la acción documentada para **incorporar piezas al TXT** y confirma el resultado. Anota el nombre y la ubicación del archivo creado; no des por comprobado el contenido únicamente por el mensaje de éxito.
3. Conserva una **copia sin modificar** del TXT generado y una copia de la hoja de control. No agregues, quites ni reordenes columnas manualmente: el esquema puede variar según la versión.
4. Cuando necesites comprobar su lectura, utiliza una **copia del TXT** y sigue [Cargar TXT](cargar-txt.md) con una producción de prueba. No selecciones **Modificar RP Anterior** sobre una producción real para ejecutar este ensayo.
5. Contrasta lo recuperado en la [ventana del Reporte de Producción](reporte-de-produccion.md) con la hoja inicial, **antes** de generar u optimizar cualquier salida.

| Control | Resultado esperado | Si no coincide |
| --- | --- | --- |
| Identificación | Cliente y ambiente del ensayo, no los de una producción real | Detén la prueba y localiza el archivo correcto |
| Cantidades | Pieza A: 2; pieza B: 1; **total: 3 unidades** | Distingue cantidad de filas, piezas y módulos; revisa duplicaciones |
| Medidas | En cada pieza, **18 × 300 × 400 mm**, salvo transformación expresamente documentada | Revisa parámetros y dimensiones del origen, sin corregir a ciegas |
| Material y veta | Misma referencia elegida y orientación prevista para ambas piezas | Verifica la asociación con el catálogo |
| Cantos | Pieza A: borde superior; pieza B: borde inferior; los demás sin canto en el ensayo | Verifica pieza y borde por separado; no intercambies las referencias |
| Persistencia | La copia del TXT se localiza y permite contrastar los datos cargados | Conserva la evidencia y revisa compatibilidad y guardado |

### 4. Registrar el resultado y decidir

Registra **fecha, versión de Cabinet Report, cliente y ambiente de prueba, ruta de la copia TXT, parámetros activos, valores esperados, valores observados y responsable**. Clasifica el resultado como **CONFORME** cuando los controles coincidan o las diferencias estén justificadas y verificadas; en otro caso, **NO CONFORME** y detén su reutilización.

{% hint style="warning" %}
**Límite de la prueba:** este ensayo comprueba el flujo de piezas de un TXT manual, **no** certifica una fórmula, el armado de un módulo ni la recuperación de accesorios, ferretería, metadatos o decisiones de Auditoría RP. Si trabajas con un módulo completo, prepara **otro ensayo independiente** con su ficha dimensional y cantidades reales; no infieras esos valores de estas piezas sueltas. Un TXT comprobado tampoco equivale a autorización para fabricar.
{% endhint %}

Continúa con la [Revisión de Tableros y Cantos](revision-de-tableros-y-cantos.md) y la [ventana del Reporte de Producción](reporte-de-produccion.md) para comprobar el despiece antes de generar archivos.

<figure><img src="../.gitbook/assets/image (15) (1) (1).png" alt="Pantalla final del recorrido de Reporte Manual"><figcaption><p>Localiza el TXT resultante y continúa con la revisión de tableros y cantos.</p></figcaption></figure>

{% hint style="info" %}
**Para más muebles:** repite el procedimiento por cada mueble que necesites incorporar desde el Catálogo de Módulos. Antes de generar la producción, comprueba cantidades, medidas, materiales y cantos.
{% endhint %}

---

[← Opciones del Reporte de Producción](README.md) · [Parámetros de Producción](parametros-de-produccion.md) · [Revisión de Tableros y Cantos →](revision-de-tableros-y-cantos.md) · [🏠 Portal principal](https://danielmelendez-pma.github.io/cabinet-report-partners/)
