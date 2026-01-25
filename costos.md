# Costos

<figure><img src=".gitbook/assets/image (123).png" alt=""><figcaption></figcaption></figure>

El módulo de Costos es para gestionar los calculos económicos de cada ambiente y generar los cuadros de costos y cotizaciones.

Funcionalidad de Costos

{% columns %}
{% column width="33.33333333333333%" %}
Inicia por el menú Opciones el cual tiene las siguientes funciones:
{% endcolumn %}

{% column width="66.66666666666667%" %}
<figure><img src=".gitbook/assets/image (126).png" alt=""><figcaption></figcaption></figure>
{% endcolumn %}
{% endcolumns %}

* Cargar reportes de compra XLSX: Es para seleccionar y cargar los Reportes de Compras generados por Cabinet Report
* Cargar archivos de ostos XML: Es para seleccionar y cargar los archivos de Costos Generados por Cabinet Report desde el módulo de Costos
* Agregar archivo Promob PDF: Es para selecionar los PDF de Promob con el contenido de materiales generados a partir del diseño
* Márgenes:
  * Tiene las opciones de Guardar Márgenes o Limpiar Márgenes ![](<.gitbook/assets/image (127).png>)
    * Guardar Márgenes: Es para guardar los archivos (MargenOperativo.xml y MargenProduccion.xml) en la carpeta "ArchivosCliente" ubicada en la misma ruta de la aplicación, los márgenes establecidos para que sean cargados cada vez que se abre la ventana de Costos
    * Limpíar Márgenes: Es para eliminar los archivos (MargenOperativo.xml y MargenProduccion.xml) de la carpeta "ArchivosCliente" ubicada en la misma ruta de la aplicación
* Notas Globales:
  * Tiene las opciones de Guardar Márgenes o Limpiar Márgenes <img src=".gitbook/assets/image (128).png" alt="" data-size="original">
    * Guardar Notas Globales: Es para guardar los archivos (NotasGlobales.xml) en la carpeta "ArchivosCliente" ubicada en la misma ruta de la aplicación, las Notas Globales establecidas para que sean cargadas cada vez que se abre la ventana de Costos
    * Limpíar Notas Globales: Es para eliminar los archivos (NotasGlobales.xml) de la carpeta "ArchivosCliente" ubicada en la misma ruta de la aplicación
* Cargar Precios Unitarios: Al activar esta opción, la aplicacion debe buscar en la base de datos la Tabla de Aglomerados "TblAglomerados" y la Tabla de Herrajes "TblAccHerrajes" cada item de la lista, tal cual están escritas sin curar texto, para buscar los valores de:&#x20;
  * Para la tabla de Herrajes  "IdAccesorio", "Tipo", "Costo", "Unidad", donde "Descripcion" sea igual a la columna DESCRIPCION del DataGridView de Materia Prima y cargar las columnas de ID, TIPO, COST-UNIT con los valores encontratos.
  * Para la tabla de Aglomerados "IdAglomerado", "PrecioProveedor"
* Limpiar

