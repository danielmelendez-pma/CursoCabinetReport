# Cargar TXT

**Curso de Cabinet Report · Importación TXT**

Esta lección explica cómo abrir un TXT de producción compatible con Cabinet Report. Identifica la procedencia del archivo, revisa los parámetros de importación y confirma sus datos después de abrirlo.

{% hint style="info" %}
**Compatibilidad:** verifica el formato del archivo de origen y las opciones disponibles en tu versión de Cabinet Report. Un archivo con la extensión correcta no garantiza que sus datos puedan importarse.
{% endhint %}

Puedes utilizar un TXT generado por Cabinet Report o por el Catálogo de Módulos, así como un archivo de otro programa **si respeta la estructura compatible**. La extensión `.txt` no confirma por sí sola esa compatibilidad.

<figure><img src="../.gitbook/assets/image (3) (1) (1) (1) (1) (1) (1) (1) (1) (1).png" alt="Captura histórica de la entrada Cargar TXT en el Reporte de Producción"><figcaption><p>Ubica la opción Cargar TXT y comprueba que el archivo procede de una fuente compatible.</p></figcaption></figure>

---
## Campos del formato documentado

La lección original muestra estos campos en este orden. Compáralos con el archivo que vas a abrir y revisa también el contenido de cada fila:

CLIENTE;

AMBIENTE;

MODULO;

CANT;

PIEZA;

ESPESOR;

ANCHO;

LARGO;

MATERIAL;

VETA;

CANTO SUPERIOR;

CANTO INFERIOR;

CANTO DERECHO;

CANTO IZQUIERDO

---
## 1. Configura los parámetros de producción

Al hacer clic, primero debe seleccionar las opciones de **Parámetros de producción**:

<figure><img src="../.gitbook/assets/image (4) (1) (1) (1) (1) (1) (1) (1) (1) (1).png" alt="Ventana de Parámetros de Producción antes de importar TXT"><figcaption><p>Selecciona los parámetros y confirma si abrirás un RP nuevo o uno anterior. <a href="parametros-de-produccion.md">Consultar Parámetros de Producción</a>.</p></figcaption></figure>

### Antes de importar, verifica lo siguiente

1. Seleccionar los tipos de vetas que contienen los materiales de la producción.
2. Seleccionar las automatizaciones que necesita.
3. Activar Packing List si lo necesita.
4. Selecciona **Generar Nuevo RP** cuando inicies una producción, o **Modificar RP Anterior** cuando quieras continuar la existente. Verifica que el destino sea el correcto.
5. Haz clic en **Importar TXT**.

## 2. Selecciona el archivo TXT

Después de configurar los parámetros, selecciona el **archivo TXT**:

<figure><img src="../.gitbook/assets/image (5) (1) (1) (1) (1) (1) (1) (1) (1) (1).png" alt="Cuadro para seleccionar el archivo TXT de producción"><figcaption><p>Elige el TXT de producción y contrasta su contenido al abrir el reporte.</p></figcaption></figure>

## 3. Abre el Reporte de Producción

Haz clic en **Abrir** para acceder al **Reporte de Producción**.

## 4. Comprueba lo cargado

Compara cliente, ambiente, módulos, cantidades de piezas, medidas, materiales, vetas y cantos con el archivo TXT original. Si no coinciden, detén la generación y revisa el archivo. Luego continúa con la [revisión de tableros y cantos](revision-de-tableros-y-cantos.md) y la [guía detallada del reporte](reporte-de-produccion.md).


---

## 5. Ejercicio de recuperación controlada: del TXT al RP

Este ejercicio sirve para **verificar una recuperación**, no para crear un formato TXT nuevo ni para demostrar que la importación restaure todos los registros de la producción. Utiliza una copia de un **TXT de producción que Cabinet Report haya generado previamente** y conserva el original intacto.

### Prepara una referencia antes de abrirlo

1. Identifica el **cliente, ambiente, archivo original y número de RP**, si corresponde. Localiza también el Excel RP anterior y los archivos auxiliares disponibles en la carpeta del proyecto.
2. **Duplica el TXT de origen** en una carpeta de comprobación. No renombres ni sustituyas el original que respalda la producción.
3. Abre la copia únicamente para **consultar**, sin cambiar separadores, columnas, identificadores ni codificación. Registra por separado los módulos, tipos de pieza, cantidades, dimensiones, materiales, vetas y cantos que esperas recuperar.
4. Consulta [Parámetros de Producción](parametros-de-produccion.md). Anota las vetas y automatizaciones activadas: redondeo, traducción técnica, inversión de medidas y carga automática de complementarios pueden influir en la comparación.
5. Para una prueba independiente, elige **Generar Nuevo RP**. Utiliza **Modificar RP Anterior** solamente cuando la intención sea actualizar una producción real, después de confirmar su número, cliente y ambiente. No uses esta última opción como ensayo sobre el único registro disponible.

{% hint style="warning" %}
**Formato de origen:** la lista de campos históricos de esta página es una guía de lectura, **no una plantilla universal para fabricar TXT a mano**. Otras descripciones del RP incluyen identificadores y nombres abreviados. No agregues, suprimas ni reordenes columnas por deducción: conserva el TXT exportado por una versión compatible y comprueba su importación antes de utilizarlo.
{% endhint %}

### Ejemplo reproducible para comprobar cantidades

Supón que tu proyecto original incluye **dos módulos iguales**, cada uno con dos costados, una base y una tapa. Esta es una **hoja de control teórica**, no un archivo TXT listo para importar:

| Pieza | Unidades por módulo | Módulos previstos | Total esperado |
| --- | ---: | ---: | ---: |
| Costado | 2 | 2 | **4** |
| Base | 1 | 2 | **2** |
| Tapa | 1 | 2 | **2** |
| **Total de piezas** | **4** | **2** | **8** |

Después de abrir el TXT, cuenta las **unidades efectivas** por tipo de pieza. Que el programa muestre filas separadas o cantidades agrupadas no cambia el objetivo: contrastar **4 costados, 2 bases y 2 tapas** con el proyecto original. No supongas que el campo de cantidad equivale siempre al número de módulos; revisa la representación que ofrece tu archivo.

### Concilia los datos recuperados

| Control | Qué comparar | Resultado que debe quedar documentado |
| --- | --- | --- |
| Identidad | Cliente, ambiente, número de RP cuando aplique | Mismo trabajo, sin confusión con otra producción |
| Integridad | Módulos, piezas sueltas, tipos de pieza y cantidades efectivas | Sin piezas omitidas ni unidades duplicadas |
| Geometría | Espesor, ancho, largo y orientación por pieza | Coincidencia con el origen o diferencia explicada |
| Materiales | Descripción del tablero, veta y canto por lado | Sin sustituciones implícitas ni pérdida de lados |
| Complementarios | Accesorios, ferretería, golas, tubos y zócalos que correspondan | Presencia comprobada en sus registros, **no inferida del TXT de piezas** |
| Entrega | Excel RP y demás salidas generadas a partir de la recuperación | Verificación independiente antes de enviarlas a fabricación |

La [guía de archivos generados](archivos-de-reportes-generados.md) diferencia el TXT de piezas, los TXT auxiliares, el Excel RP y los registros técnicos. **Importar el TXT de producción no prueba por sí solo la recuperación de herrajes, parámetros, metadatos XML ni decisiones de Auditoría RP.** Verifica cada componente por separado.

### Si el resultado no coincide

1. **Detén la generación u optimización** y conserva la copia importada y el origen sin cambios.
2. Comprueba si seleccionaste el **RP correcto**, un archivo compatible y las automatizaciones adecuadas. Distingue cambios esperables por configuración de pérdidas de datos.
3. Si faltan piezas, materiales o complementarios, revisa los archivos de procedencia y vuelve a probar con una **copia limpia**, sin sobrescribir el RP original.
4. Si la recuperación parte de un Excel RP editado, sigue primero [RP a TXT](rp-a-txt.md) y valida el archivo convertido antes de importarlo.
5. Registra el archivo utilizado, los valores esperados y las diferencias detectadas. Reanuda el flujo únicamente cuando la comprobación técnica sea satisfactoria.

{% hint style="info" %}
**Criterio de salida:** el TXT se considera **comprobado para este proyecto** cuando identidad, cantidades, dimensiones, materiales y cantos concuerdan con la fuente autorizada y los complementarios necesarios se han verificado aparte. Es una prueba documental de control, **no una certificación automática de compatibilidad ni de preparación para fabricar**.
{% endhint %}

---

[← Cargar CSV](cargar-csv.md) · [RP a TXT →](rp-a-txt.md) · [Parámetros de producción](parametros-de-produccion.md) · [🏠 Portal principal](https://danielmelendez-pma.github.io/cabinet-report-partners/)
