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

<figure><img src="../.gitbook/assets/image (9) (1) (1) (1) (1).png" alt=""><figcaption></figcaption></figure>

## 1. Identificar la producción

1. Escribe el **nombre del cliente** y el **ambiente**.
2. Selecciona **Crear Nuevo** para comenzar el archivo TXT.
3. Si necesitas continuar una producción existente, utiliza la opción para **abrir un archivo TXT**. Verifica la identidad y el contenido de ese archivo antes de editarlo.

<figure><img src="../.gitbook/assets/image (1) (1) (1) (1) (1) (1) (1) (1) (1).png" alt=""><figcaption></figcaption></figure>

{% hint style="warning" %}
**Campos obligatorios:** si intentas crear un TXT nuevo sin indicar cliente y ambiente, Cabinet Report no permite continuar. Completa ambos datos antes de volver a intentarlo.
{% endhint %}

<figure><img src="../.gitbook/assets/image (2) (1) (1) (1) (1) (1) (1).png" alt=""><figcaption></figcaption></figure>

## 2. Configurar los parámetros

Selecciona los parámetros de producción que correspondan al trabajo antes de agregar piezas. Contrasta las opciones disponibles en tu versión con los materiales y procesos previstos: **vetas, automatizaciones y tipo de reporte**, cuando apliquen. Consulta [Parámetros de Producción](parametros-de-produccion.md). Una automatización activada no valida las medidas por sí sola.

<figure><img src="../.gitbook/assets/image (3) (1) (1) (1) (1) (1) (1).png" alt=""><figcaption></figcaption></figure>

## 3. Elegir cómo incorporar las piezas

### Opción A: piezas sueltas

Activa la opción de **piezas sueltas** si vas a agregar piezas de forma independiente al listado.

<figure><img src="../.gitbook/assets/image (4) (1) (1) (1) (1) (1) (1).png" alt=""><figcaption></figcaption></figure>

### Opción B: piezas de un módulo

Si trabajarás con un **módulo completo**, activa esa opción e introduce las dimensiones del módulo. Confirma las referencias de **profundidad, ancho y alto** que se utilizarán para interpretar las piezas. No confundas las dimensiones exteriores del mueble con las medidas efectivas de cada pieza.

<figure><img src="../.gitbook/assets/image (5) (1) (1) (1) (1) (1) (1).png" alt=""><figcaption></figcaption></figure>

## 4. Agregar las piezas al listado

Puedes utilizar cualquiera de estos dos métodos:

### Método 1: ingreso manual

Agrega las piezas directamente en el listado de piezas.

<figure><img src="../.gitbook/assets/image (6) (1) (1) (1) (1) (1).png" alt=""><figcaption></figcaption></figure>

### Método 2: selección desde la base de datos

Coloca el listado de piezas de la base de datos junto al área de trabajo y agrega desde allí las piezas que necesites.

<figure><img src="../.gitbook/assets/image (7) (1) (1) (1) (1) (1).png" alt=""><figcaption></figcaption></figure>

Cuando hayas incorporado todas las piezas del módulo que estás preparando, revisa el listado antes de continuar. Tanto para el ingreso manual como para la selección desde la base de datos, comprueba:

1. **Nombre y función:** que no falten piezas necesarias ni haya duplicados accidentales.
2. **Cantidad y pertenencia:** unidades correctas y clasificación coherente como módulo o pieza suelta.
3. **Medidas:** espesor, ancho, largo y orientación compatibles con el diseño.
4. **Material y acabado:** tablero, veta y cantos de cada borde.

Una definición guardada en la base de datos **no queda validada automáticamente** para un módulo con parámetros distintos.

<figure><img src="../.gitbook/assets/image (8) (1) (1) (1) (1) (1).png" alt=""><figcaption></figcaption></figure>

## 5. Incorporar las piezas al archivo TXT

Utiliza la acción indicada en la pantalla para añadir las piezas al reporte. **Incorporar piezas al TXT no equivale a generar u optimizar la producción final**: el resultado debe comprobarse antes de continuar con el RP.

<figure><img src="../.gitbook/assets/image (12) (1) (1) (1).png" alt=""><figcaption></figcaption></figure>

Si todavía no has creado un archivo TXT ni has abierto uno existente, Cabinet Report solicitará hacerlo antes de continuar.

<figure><img src="../.gitbook/assets/image (13) (1) (1) (1).png" alt=""><figcaption></figcaption></figure>

Cuando el proceso se completa, se muestra el mensaje de confirmación de incorporación de piezas.

<figure><img src="../.gitbook/assets/image (14) (1) (1).png" alt=""><figcaption></figcaption></figure>

## 6. Verificar el resultado

Comprueba que el archivo TXT se haya creado o actualizado correctamente y que incluya las piezas previstas.

| Comprobación | Qué contrastar |
| --- | --- |
| **Identificación** | Cliente, ambiente y archivo nuevo o existente según el recorrido elegido. |
| **Integridad** | Piezas previstas, sin omisiones ni duplicados accidentales. |
| **Cantidades** | Unidades de cada pieza y módulo acordes con el proyecto. |
| **Datos técnicos** | Espesor, ancho, largo, material, veta y cantos por lado. |
| **Resultado** | El TXT actualizado se localiza y pertenece a la producción preparada. |

Continúa con la [Revisión de Tableros y Cantos](revision-de-tableros-y-cantos.md) y la [ventana del Reporte de Producción](reporte-de-produccion.md) para comprobar el despiece antes de generar archivos.

<figure><img src="../.gitbook/assets/image (15) (1) (1).png" alt=""><figcaption></figcaption></figure>

{% hint style="info" %}
**Para más muebles:** repite el procedimiento por cada mueble que necesites incorporar desde el Catálogo de Módulos. Antes de generar la producción, comprueba cantidades, medidas, materiales y cantos.
{% endhint %}

---

[← Opciones del Reporte de Producción](README.md) · [Parámetros de Producción](parametros-de-produccion.md) · [Revisión de Tableros y Cantos →](revision-de-tableros-y-cantos.md) · [🏠 Portal principal](https://danielmelendez-pma.github.io/cabinet-report-partners/)
