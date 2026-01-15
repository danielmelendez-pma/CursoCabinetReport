# Creación de Piezas

{% columns %}
{% column %}
<figure><img src=".gitbook/assets/image.png" alt=""><figcaption></figcaption></figure>
{% endcolumn %}

{% column %}
Una vez aprendido las variables para crear formulas de calculo de piezas, puede adentrarse a la sección de

## <mark style="color:$primary;">Creador de Piezas</mark>

<mark style="color:$primary;">Donde puede crear sus piezas o utilizar las piezas ya creadas dentro de Cabinet Report</mark>

> 💡 **Importante**\
> Un Creador de Piezas bien configurado garantiza que Cabinet Report genere información confiable, minimizando errores humanos y mejorando la eficiencia en el proceso productivo.
{% endcolumn %}
{% endcolumns %}

***

La sección de creador de piezas se divide en 3 partes:

{% columns %}
{% column %}
<figure><img src=".gitbook/assets/image (22).png" alt=""><figcaption></figcaption></figure>
{% endcolumn %}

{% column %}
## <mark style="color:$primary;">Lista de Piezas Guardadas</mark>

Aparecen las piezas existentes creadas y las nuevas que se creen con sus propias fórmulas

También tiene un campo para desactivar si desea editar una pieza creada.
{% endcolumn %}
{% endcolumns %}

{% columns %}
{% column width="50%" %}
## <mark style="color:$primary;">Área de Fórmulas</mark>

Para colocar el nombre de la pieza y sus fórmulas para las medidas de:

ESPESOR X ANCHO X LARGO
{% endcolumn %}

{% column width="50%" %}
<figure><img src=".gitbook/assets/image (23).png" alt=""><figcaption></figcaption></figure>
{% endcolumn %}
{% endcolumns %}

{% columns %}
{% column %}
<figure><img src=".gitbook/assets/image (24).png" alt=""><figcaption></figcaption></figure>
{% endcolumn %}

{% column %}
## <mark style="color:$primary;">Sección de Variables</mark>

Lista de variables que le ayuda a crear las formulas de cada una de sus piezas.
{% endcolumn %}
{% endcolumns %}

***

## <mark style="color:$primary;">Ejemplo de cómo se crean las fórmulas para diferentes piezas...</mark>

Para un mueble base de 580 x 900 x 780, con 2 puertas con 1 tablilla y respaldo de cartón 4mm, donde el cajon interno es color blanco 15mm y las partes vistas es color madera 18mm, tomando en cuenta que el costado izquierdo es visto:

<div data-with-frame="true"><figure><img src=".gitbook/assets/image (26).png" alt=""><figcaption></figcaption></figure></div>

<mark style="color:$primary;">**COSTADO IZQUIERDO**</mark>: ESPV <mark style="color:$primary;">**X**</mark> PROF <mark style="color:$primary;">**X**</mark> ALTO = <mark style="color:$warning;">18 X 580 X 780 MADERA</mark>

<mark style="color:$primary;">**COSTADO DERECHO**</mark>: ESPC <mark style="color:$primary;">**X**</mark> PROF <mark style="color:$primary;">**X**</mark> ALTO = <mark style="color:$warning;">15 X 580 X 780 BLANCO</mark>

<mark style="color:$primary;">**BASE**</mark>: ESPC <mark style="color:$primary;">**X**</mark> PROF-ESPC-CART <mark style="color:$primary;">**X**</mark> ANCHO-ESPV-ESPC =  <mark style="color:$warning;">15 X 562 X 867 BLANCO</mark>

<mark style="color:$primary;">**CADENA POST**</mark>: ESPC <mark style="color:$primary;">**X**</mark> 100 <mark style="color:$primary;">**X**</mark> ANCHO-ESPV-ESPC = <mark style="color:$warning;">15 X 100 X 867</mark>



