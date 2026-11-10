---
description: >-
  Aprende a localizar una producción por sus referencias y a distinguir la
  consulta de proyectos de la recuperación mediante archivos compatibles.
---

# Explorador de Proyectos

**Etapa del curso · Consulta, recuperación y continuidad del trabajo**

El **Explorador de Proyectos** sirve para buscar y consultar información de trabajos registrados en Cabinet Report. Permite identificar una producción antes de decidir cómo continuarla, pero **encontrar un registro no garantiza que puedas abrir, editar o reconstruir todos sus archivos desde otro equipo**.

<figure><img src=".gitbook/assets/image (115).png" alt="Vista del Explorador de Proyectos de Cabinet Report"><figcaption><p>Localiza un registro; su aparición no garantiza que los archivos de producción estén recuperados.</p></figcaption></figure>

{% hint style="info" %}
**Alcance de esta lección:** la consulta por proyecto, planificador o número de RP está descrita en la [Documentación oficial del Explorador](https://cabinet-report.gitbook.io/cabinet-report-docs/funcionalidades-de-cabinet-report/explorador-de-proyectos). La importación directa de proyectos entre equipos y otras funciones avanzadas no están acreditadas allí como disponibles. No confundas la lista de proyectos con una copia de seguridad completa.
{% endhint %}

## Cuándo consultar el Explorador

Puedes acudir aquí **antes de preparar nuevos archivos** o cuando necesites ubicar una producción usada en [Reporte de Compras](reporte-de-compras.md) o [Orden de Producción](orden-de-produccion.md). La consulta solo identifica un registro; para continuar con fabricación, debes recuperar y revisar por separado los archivos que correspondan.

## 1. Localiza la producción correcta

1. Abre **Explorador de Proyectos** con una cuenta que tenga acceso al trabajo.
2. Utiliza el dato más preciso que conozcas: **nombre del proyecto**, **usuario planificador** o **número de RP**.
3. Revisa las coincidencias. Si aparecen varias, no selecciones una únicamente porque comparta un nombre o un planificador.
4. Contrasta la identificación del trabajo con el cliente, ambiente y número de RP que tengas en tus documentos o registros.
5. Comprueba qué acciones están **realmente habilitadas** para tu usuario y versión antes de intentar continuar.

| Criterio de búsqueda | Cuándo te ayuda | Qué debes comprobar |
| --- | --- | --- |
| **Proyecto** | Recuerdas el nombre del trabajo. | Que la coincidencia corresponda al cliente y ambiente esperados. |
| **Planificador** | Conoces quién preparó el proyecto. | Que no estés confundiendo diferentes trabajos de la misma persona. |
| **Número de RP** | Dispones de la referencia de un reporte. | Que el número corresponda a la producción que necesitas consultar. |

**Resultado esperado:** poder identificar el registro correcto y saber si la instalación ofrece una acción adicional. **Ver un resultado no es prueba de que el TXT, el Excel RP o los metadatos locales estén disponibles.**

## 2. Elige cómo continuar según lo que realmente tienes

El Explorador es una herramienta de **localización**. Cuando necesites retomar piezas o generar un nuevo archivo, distingue el registro consultado de los archivos que permiten introducir información en el Reporte de Producción.

| Situación | Ruta documentada | Límite importante |
| --- | --- | --- |
| **El proyecto aparece y existe una acción de apertura habilitada.** | Utiliza solo la acción que ofrezca tu versión y revisa lo que se cargó. | No presupongas que también se recuperaron archivos complementarios o cambios locales. |
| **El proyecto aparece, pero no puedes abrirlo o editarlo.** | Busca los archivos de origen o una copia respaldada del trabajo. | La consulta por sí sola no acredita recuperación completa ni permisos de edición. |
| **Conservas un TXT de piezas compatible.** | Sigue [Cargar TXT](reporte-de-produccion/cargar-txt.md). | Verifica la estructura, cliente, ambiente, módulos, piezas y cantidades después de importar. |
| **Conservas un Excel RP de Cabinet Report que fue editado.** | Sigue [RP a TXT](reporte-de-produccion/rp-a-txt.md) si mantiene el formato requerido. | La conversión depende de la estructura original del Excel; comprueba el TXT resultante. |
| **Tienes un CSV procedente de otra herramienta.** | Consulta [Cargar CSV](reporte-de-produccion/cargar-csv.md). | La extensión `.csv` no acredita compatibilidad con el importador. |
| **No dispones de un archivo recuperable.** | Consulta [Reporte en Blanco](reporte-de-produccion/reporte-en-blanco.md). | Crear piezas de nuevo no restaura automáticamente un proyecto anterior. |

{% hint style="warning" %}
**Evita sobrescribir o mezclar producciones.** Conserva una copia del origen antes de importar o convertir. Cuando el programa pida elegir entre **Generar Nuevo RP** y **Modificar RP Anterior**, verifica qué trabajo se verá afectado; la opción correcta depende de si estás iniciando o continuando una producción concreta.
{% endhint %}

## 3. Conserva los archivos que permiten comprobar el trabajo

Los archivos relacionados con una producción tienen funciones diferentes. No utilices uno como sustituto automático de otro.

- **TXT de producción:** contiene información de las piezas para retomar un flujo compatible. Comprueba que corresponda a la última versión que deseas continuar.
- **Excel RP (.xlsx):** se utiliza para revisar o entregar el reporte. No equivale directamente al TXT de entrada; si necesitas convertirlo, utiliza el procedimiento de **RP a TXT** y comprueba el resultado.
- **Archivos de herrajes, perfiles, materiales y parámetros:** pueden acompañar al trabajo según su contenido y la generación realizada. Verifica su pertenencia a la misma producción.
- **Metadatos técnicos y Auditoría RP en XML:** cuando existan, cumplen funciones de trazabilidad y revisión distintas del listado de piezas. No los edites ni sustituyas manualmente como si fueran un respaldo universal.

Para reconocer las salidas de una producción, abre [Archivos de Reportes Generados](reporte-de-produccion/archivos-de-reportes-generados.md). Para conocer la persistencia de revisiones, consulta [Auditoría RP y persistencia](https://cabinet-report.gitbook.io/cabinet-report-docs/funcionalidades-de-cabinet-report/auditoria-rp-persistencia).

## 4. Verifica el resultado antes de volver a generar

Después de localizar o reabrir un trabajo:

1. Comprueba **cliente, ambiente, referencia y número de RP**.
2. Compara **módulos, piezas sueltas y cantidades** con la fuente que conservaste.
3. Revisa **medidas, materiales, espesores, vetas y cantos** antes de corregir o generar.
4. Confirma si los **herrajes, perfiles y demás archivos complementarios** que necesitas están presentes.
5. Si la información no coincide, identifica cuál es la versión válida y vuelve al origen antes de continuar. No des por correcta una carga solo porque se abrió sin mostrar errores.

{% hint style="info" %}
**Si no encuentras el trabajo:** revisa el filtro aplicado, los identificadores utilizados y los permisos de la cuenta. Si necesitas soporte, comunica la versión del programa, la operación intentada y el mensaje de error, sin compartir contraseñas ni credenciales. La falta de un resultado no demuestra por sí sola pérdida definitiva de los archivos.
{% endhint %}

## Ejercicio práctico

Supón que recibes de otro colaborador un **número de RP** y necesitas retomar la revisión:

1. Busca primero ese número en el Explorador y confirma que el registro corresponda al proyecto esperado.
2. Identifica si puedes abrirlo desde la instalación o si solo está disponible su consulta.
3. Si debes continuar mediante un respaldo, decide entre **Cargar TXT**, **RP a TXT** o **Cargar CSV** según el archivo real disponible.
4. Abre el Reporte de Producción y compara las piezas y sus propiedades con el origen.
5. Documenta qué archivo utilizaste para que el siguiente responsable no confunda la producción consultada con la versión preparada para fabricación.

**Objetivo del ejercicio:** distinguir tres estados diferentes: *proyecto localizado*, *información recuperada* y *producción validada*. Uno no demuestra automáticamente los otros.

## Continúa tu recorrido

Una vez recuperado y revisado el RP correcto, consulta [Reporte de Compras](reporte-de-compras.md) si necesitas preparar insumos o [Orden de Producción](orden-de-produccion.md) si vas a agrupar reportes para fabricación. **Ninguno de esos procesos acredita por sí solo la recepción de materiales ni el avance físico en planta.**

Consulta el [**Reporte de Producción**](reporte-de-produccion/README.md) para preparar o reabrir los datos de piezas. Para los límites funcionales del Explorador, utiliza su [**Documentación oficial**](https://cabinet-report.gitbook.io/cabinet-report-docs/funcionalidades-de-cabinet-report/explorador-de-proyectos).

[← Portada del Curso](README.md) · [Catálogo de Módulos](catalogo-de-modulos.md) · [🏠 Portal principal](https://danielmelendez-pma.github.io/cabinet-report-partners/)
