# Cargar CSV

**Curso de Cabinet Report · Importación CSV**

Esta lección explica la secuencia documentada para importar un CSV en el Reporte de Producción. Antes de usar el resultado, contrasta la estructura del archivo con el importador disponible en tu versión.

{% hint style="info" %}
**Compatibilidad:** verifica el formato del archivo de origen y las opciones disponibles en tu versión de Cabinet Report. Un archivo con la extensión correcta no garantiza que sus datos puedan importarse.
{% endhint %}

La documentación original presenta la importación de archivos procedentes de programas de diseño como **Promob**. La compatibilidad depende del formato exportado y de la opción de importación de Cabinet Report; no presupongas que cualquier CSV puede abrirse.

<figure><img src="../.gitbook/assets/image (12) (1) (1) (1) (1).png" alt=""><figcaption></figcaption></figure>

Si trabajas con un CSV generado por un programa de diseño, primero comprueba que las columnas y los valores correspondan con el formato que admite Cabinet Report. La importación es el punto de entrada; aún debes revisar las piezas antes de generar producción.

---
## Campos del formato documentado

La lección original muestra estos campos en este orden. Es una referencia para revisar el archivo de origen; **la presencia de los nombres por sí sola no confirma compatibilidad**:

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

<figure><img src="../.gitbook/assets/image (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1).png" alt=""><figcaption><p><a href="parametros-de-produccion.md">Ver Explicación</a></p></figcaption></figure>

### Antes de importar, verifica lo siguiente

1. Seleccionar los tipos de vetas que contienen los materiales de la producción.
2. Seleccionar las automatizaciones que necesita.
3. Activar Packing List si lo necesita.
4. Selecciona **Generar Nuevo RP** si vas a iniciar un reporte, o **Modificar RP Anterior** si corresponde continuar uno existente. Confirma la opción elegida para evitar mezclar producciones.
5. Haz clic en **Importar CSV de CutPro**, nombre del control documentado en esta lección.

{% hint style="warning" %}
**Nombre de la opción y origen del archivo:** esta página menciona archivos de Promob, pero el control se denomina «Importar CSV de CutPro». La coincidencia de formatos entre programas no queda demostrada aquí. Comprueba el archivo de prueba en la versión instalada; no renombres el control ni supongas compatibilidad universal.
{% endhint %}

## 2. Selecciona el archivo CSV

Después de configurar los parámetros, selecciona el **archivo CSV**:

<figure><img src="../.gitbook/assets/image (2) (1) (1) (1) (1) (1) (1) (1) (1) (1).png" alt=""><figcaption></figcaption></figure>

## 3. Abre el Reporte de Producción

Haz clic en **Abrir** para acceder al **Reporte de Producción**.

## 4. Comprueba la importación

Antes de generar el RP, compara el cliente, ambiente, cantidad de filas y piezas, dimensiones, tableros, vetas y cantos con el CSV original. Si hay diferencias, corrige el origen o revisa la compatibilidad antes de continuar con la [revisión de tableros y cantos](revision-de-tableros-y-cantos.md) y la [guía de la ventana](reporte-de-produccion.md).

---

[← Opciones del Reporte de Producción](README.md) · [Cargar TXT →](cargar-txt.md) · [Parámetros de producción](parametros-de-produccion.md) · [🏠 Portal principal](https://danielmelendez-pma.github.io/cabinet-report-partners/)
