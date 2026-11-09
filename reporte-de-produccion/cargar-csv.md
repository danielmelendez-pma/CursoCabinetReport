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

## 5. Ensayo verificable: CSV de origen → RP abierto

Este ejercicio verifica **una importación concreta** antes de utilizarla en fabricación. No acredita que todos los CSV de un programa sean compatibles con Cabinet Report ni establece un formato nuevo de columnas. La lista de campos históricos anterior es una referencia; **no debe utilizarse para reconstruir el importador por suposición**.

### A. Conserva la fuente y prepara una referencia

1. Elige un **CSV realmente exportado** por el programa de origen y guarda una copia intacta. Registra exportador, versión si se conoce, opción de exportación, fecha y nombre del archivo. Marca como **no comprobado** cualquier dato desconocido.
2. Consulta el archivo sin modificarlo. Registra cliente, ambiente, módulo y pieza **cuando estén disponibles**; además, anota cantidades efectivas, espesor, ancho, largo, material, veta y cantos por lado. No cambies encabezados, separadores, codificación ni orden de columnas para forzar una supuesta compatibilidad.
3. Prepara una **hoja de referencia** a partir del CSV y el diseño autorizado. Si el exportador no proporciona un campo, marca **no disponible en origen**; no completes vacíos por deducción.
4. Anota los [Parámetros de Producción](parametros-de-produccion.md) seleccionados: vetas, traducción técnica, redondeo, inversión de medidas y otras automatizaciones. Así podrás distinguir una transformación esperada de una pérdida de datos.
5. Ejecuta la prueba sobre un trabajo de ensayo y selecciona **Generar Nuevo RP** cuando la versión instalada lo permita. **Modificar RP Anterior** solo corresponde a un cambio real de un RP existente, después de comprobar número, cliente, ambiente y respaldo.

{% hint style="warning" %}
**Procedencia no acreditada:** la guía histórica cita **Promob**, pero el control documentado se llama **«Importar CSV de CutPro»**. Registra cuál utilizaste y lo que sucedió. No supongas equivalencia de formatos ni compatibilidad universal entre exportadores.
{% endhint %}

### B. Concilia los datos después de importar

Utiliza esta tabla como hoja de verificación. Conserva una referencia a cada pieza o grupo identificable en el origen.

| Comprobación | Fuente CSV o diseño aprobado | RP después de importar | Estado |
| --- | --- | --- | --- |
| Cliente, ambiente y módulo, cuando existan | Identificar trabajo | Comparar identificación | Coincide / Diferencia / No comprobado |
| Pieza y **cantidad efectiva** | Contar unidades previstas | Contar unidades cargadas | Coincide / Diferencia / No comprobado |
| Espesor, ancho, largo y orientación | Registrar cada valor | Revisar cada valor | Coincide / Diferencia / No comprobado |
| Tablero, acabado y veta | Registrar material previsto | Verificar material asignado | Coincide / Diferencia / No comprobado |
| Canto superior, inferior, derecho e izquierdo | Registrar lados existentes | Revisar cada lado | Coincide / Diferencia / No comprobado |
| Parámetros que transforman información | Anotar opciones activadas | Explicar diferencias observadas | Explicado / Pendiente |

**Ejemplo didáctico de conteo:** si el diseño de referencia contiene dos costados, una base y una tapa, se esperan **cuatro unidades físicas**, aunque el CSV y el RP muestren un número diferente de filas. No es una plantilla CSV válida ni demuestra que todos los exportadores acepten esa composición.

Registra por separado **filas del archivo, tipos de pieza y unidades efectivas**. Si un campo no es visible o no puede verificarse en la aplicación, márcalo como **no comprobado**; no interpretes su ausencia como coincidencia.

### C. Comprueba materiales y diagnostica discrepancias

1. Continúa en [Revisión de Tableros y Cantos](revision-de-tableros-y-cantos.md). Verifica nombre, tipo, espesor, veta y cada borde; que dos materiales tengan nombres parecidos no demuestra equivalencia.
2. Si una dimensión, nombre u orientación cambia, comprueba las **automatizaciones registradas** y documenta la diferencia de origen y destino antes de atribuirla al importador.
3. Si faltan piezas o aparecen unidades adicionales, consulta la fuente y la representación del RP. **No confundas filas con unidades** ni ajustes el total para ocultar una discrepancia.
4. Revisa **por separado** accesorios, ferretería, golas, tubos y zócalos cuando correspondan. Importar un CSV de piezas **no acredita** la recuperación de complementarios; consulta [Archivos de Reportes Generados](archivos-de-reportes-generados.md).
5. Si se rechaza el archivo, falta una columna reconocible o aparece un campo vacío, registra **el comportamiento y el aviso exacto**. Conserva la fuente intacta y no atribuyas una causa específica sin evidencia.

### D. Decide si puedes continuar

| Resultado de la prueba | Decisión |
| --- | --- |
| Se verifica identidad, unidades, medidas, materiales, vetas y cantos frente a la fuente aprobada | Documenta la prueba y continúa con la validación técnica habitual |
| La diferencia corresponde a una transformación configurada y fue contrastada pieza por pieza | Registra la explicación y vuelve a comprobar el despiece |
| Se pierden piezas, sobran unidades, cambia un material o persiste una discrepancia | **Detén generación, optimización y entrega** hasta resolverla |
| El formato no es compatible o no hay datos esenciales para conciliar | **No afirmes compatibilidad ni aprobación**; revisa el archivo de origen y el importador |

**Evidencia mínima:** conserva el CSV original, la copia ensayada, el exportador y la versión conocidos, los parámetros seleccionados, la identificación del RP de prueba, la tabla de comparación, los avisos o capturas relevantes y la decisión final. Un resultado correcto avala **ese archivo y esa configuración**, no cualquier CSV futuro. Antes de fabricar, continúa con la [guía del Reporte de Producción](reporte-de-produccion.md).

---

[← Opciones del Reporte de Producción](README.md) · [Cargar TXT →](cargar-txt.md) · [Parámetros de producción](parametros-de-produccion.md) · [🏠 Portal principal](https://danielmelendez-pma.github.io/cabinet-report-partners/)
