# Cargar TXT

**Curso de Cabinet Report · Importación TXT**

Esta lección explica cómo abrir un TXT de producción compatible con Cabinet Report. Identifica la procedencia del archivo, revisa los parámetros de importación y confirma sus datos después de abrirlo.

{% hint style="info" %}
**Compatibilidad:** verifica el formato del archivo de origen y las opciones disponibles en tu versión de Cabinet Report. Un archivo con la extensión correcta no garantiza que sus datos puedan importarse.
{% endhint %}

Puedes utilizar un TXT generado por Cabinet Report o por el Catálogo de Módulos, así como un archivo de otro programa **si respeta la estructura compatible**. La extensión `.txt` no confirma por sí sola esa compatibilidad.

<figure><img src="../.gitbook/assets/image (3) (1) (1) (1) (1) (1) (1) (1) (1) (1).png" alt=""><figcaption></figcaption></figure>

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

<figure><img src="../.gitbook/assets/image (4) (1) (1) (1) (1) (1) (1) (1) (1) (1).png" alt=""><figcaption><p><a href="parametros-de-produccion.md">Ver Explicación</a></p></figcaption></figure>

### Antes de importar, verifica lo siguiente

1. Seleccionar los tipos de vetas que contienen los materiales de la producción.
2. Seleccionar las automatizaciones que necesita.
3. Activar Packing List si lo necesita.
4. Selecciona **Generar Nuevo RP** cuando inicies una producción, o **Modificar RP Anterior** cuando quieras continuar la existente. Verifica que el destino sea el correcto.
5. Haz clic en **Importar TXT**.

## 2. Selecciona el archivo TXT

Después de configurar los parámetros, selecciona el **archivo TXT**:

<figure><img src="../.gitbook/assets/image (5) (1) (1) (1) (1) (1) (1) (1) (1) (1).png" alt=""><figcaption></figcaption></figure>

## 3. Abre el Reporte de Producción

Haz clic en **Abrir** para acceder al **Reporte de Producción**.

## 4. Comprueba lo cargado

Compara cliente, ambiente, módulos, cantidades de piezas, medidas, materiales, vetas y cantos con el archivo TXT original. Si no coinciden, detén la generación y revisa el archivo. Luego continúa con la [revisión de tableros y cantos](revision-de-tableros-y-cantos.md) y la [guía detallada del reporte](reporte-de-produccion.md).

---

[← Cargar CSV](cargar-csv.md) · [RP a TXT →](rp-a-txt.md) · [Parámetros de producción](parametros-de-produccion.md) · [🏠 Portal principal](https://danielmelendez-pma.github.io/cabinet-report-partners/)
