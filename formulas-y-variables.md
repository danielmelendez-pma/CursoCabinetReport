---
description: Aprende a identificar variables dimensionales, espesores, cantos y luces, y a comprobar fórmulas de piezas antes de utilizarlas en producción.
---

# Fórmulas y Variables

Las fórmulas permiten que las medidas de una pieza se recalculen al cambiar las dimensiones o los parámetros del módulo. Antes de crear una pieza, distingue **la variable que se escribe en la fórmula** del **valor que toma esa variable** al trabajar con un módulo concreto.

{% hint style="warning" %}
**No copies un resultado numérico como si fuera una regla universal.** Los espesores, rieles, luces y demás parámetros deben revisarse en el catálogo, módulo y configuración del cliente que se está utilizando. Antes de fabricar, confirma las medidas obtenidas.
{% endhint %}

## 1. Dimensiones del módulo

Estas variables describen las dimensiones de referencia del mueble. No son descuentos ni luces.

| Variable | Qué representa |
| --- | --- |
| `PROF` | Profundidad del cuerpo del mueble, sin contar puertas o frentes de gavetas. |
| `ANCHO` | Ancho terminado del cuerpo del mueble. |
| `ALTO` | Altura terminada del mueble, sin considerar las patas. |

Una misma fórmula puede producir resultados distintos si cambian `PROF`, `ANCHO` o `ALTO`.

## 2. Espesores y respaldo

| Variable | Qué representa |
| --- | --- |
| `ESPC` | Espesor del tablero del cuerpo o cajón del mueble, en las partes que no quedan vistas tras la instalación. |
| `ESPV` | Espesor del tablero de partes visibles, como puertas y costados vistos. |
| `RESP` | Espesor del tablero delgado que se inserta en ranuras para respaldos o fondos de gavetas. |

La elección del tablero y su espesor debe corresponder a la pieza real. `ESPC` y `ESPV` pueden tener valores diferentes.

{% hint style="warning" %}
**Variable histórica sin definición comprobada:** la fórmula de la `BASE` en [Creación de Piezas](creacion-de-piezas.md) contiene `CART`, pero esta lección no acredita su significado técnico. No sustituyas `CART` por `RESP` ni le atribuyas **3 mm** o **4 mm** por inferencia. Comprueba su procedencia y valor efectivo en la versión y el catálogo utilizados.
{% endhint %}

## 3. Cantos

| Variable | Uso documentado |
| --- | --- |
| `CVISTO` | Canto o cintillo utilizado en los lados frontales o visibles. |
| `CCAJON` | Canto o cintillo para lados internos, traseros o no visibles. |

Estas referencias **identifican el canto que se asigna a un borde**; no deben confundirse con `ANCHO`, `LARGO` ni con una luz en milímetros. Revisa qué lado de la pieza corresponde a cada canto en el [Creador de Piezas](creacion-de-piezas.md).

## 4. Rieles de gavetas

| Variable | Uso documentado |
| --- | --- |
| `RE` | Espesor o espacio consumido por el riel al calcular anchos internos de gaveta. |
| `RL` | Largo del riel para calcular laterales de gaveta. |
| `RA` | Altura del riel cuando se utiliza un riel lateral metálico. |

Comprueba que el riel seleccionado sea el que corresponde al sistema de gavetas, incluso cuando reutilices un módulo existente.

## 5. Luces, ranuras y otros descuentos

Las **luces** son separaciones que se consideran en las fórmulas de puertas, frentes y respaldos según el diseño.

| Variable | Uso documentado |
| --- | --- |
| `LSU` | Luz superior para puertas y frentes de gavetas. |
| `LIN` | Luz inferior para puertas y frentes de gavetas. |
| `LCE` | Luz central entre puertas. |
| `LIZ` | Luz izquierda para puertas y frentes de gavetas. |
| `LDE` | Luz derecha para puertas y frentes de gavetas. |
| `LGA` | Luz entre frentes de gavetas. |
| `GOL` | Luz asociada a tiradores tipo Gola. |
| `PIN` | Descuento correspondiente al pin de soporte de tablillas móviles. |
| `RAN` | Profundidad de la ranura donde se inserta un respaldo delgado. |
| `LIR` | Luz inferior del respaldo delgado. |
| `LSR` | Luz superior del respaldo delgado. |

{% hint style="info" %}
**La procedencia de cada valor importa.** Una variable puede conservar su nombre mientras su valor cambia de un módulo o cliente a otro. Revisa los parámetros aplicados antes de interpretar un resultado como incorrecto.
{% endhint %}

## 6. Ejemplo de lectura de una fórmula

En la lección [Creación de Piezas](creacion-de-piezas.md) se documenta una puerta de un módulo con dos hojas. Su **ancho** se expresa así:

```text
(ANCHO - LIZ - LDE - LCE) / 2
```

Y su **alto**, así:

```text
ALTO - LSU - LIN
```

Como ejemplo **didáctico**, no como valores predeterminados del programa, considera:

- `ANCHO = 900 mm`, `LIZ = 2 mm`, `LDE = 2 mm` y `LCE = 2 mm`.
- `ALTO = 780 mm`, `LSU = 2 mm` y `LIN = 2 mm`.
- `ESPV = 18 mm`.

El resultado sería un **ancho de 447 mm por hoja**: `(900 - 2 - 2 - 2) / 2 = 447`; y un **alto de 776 mm**: `780 - 2 - 2 = 776`. El espesor de 18 mm se indica en el campo correspondiente de la pieza.

**Comparación con Creación de Piezas:** el ejemplo histórico muestra **448 mm** por puerta, pero no documenta los valores efectivos de todas sus luces. Los **447 mm** de este ejercicio solo resultan de los valores didácticos indicados arriba; la diferencia **no demuestra por sí sola** un error en la fórmula histórica.

{% hint style="warning" %}
**Comprueba qué representa cada descuento.** El ancho del cuerpo del mueble no equivale necesariamente al ancho de una puerta. Tampoco debe suponerse que las luces de este ejemplo sean las configuradas para otro cliente, catálogo o tipo de apertura.
{% endhint %}

## 7. Comprobación antes de guardar una pieza

1. Identifica el módulo y confirma sus valores de `PROF`, `ANCHO` y `ALTO`.
2. Revisa los tableros seleccionados y sus espesores `ESPC`, `ESPV` y `RESP`.
3. Comprueba los parámetros de luces, ranuras, rieles y pines que intervienen en la fórmula.
4. Introduce o revisa por separado las expresiones de **espesor, ancho y largo** de la pieza.
5. Verifica el resultado calculado, la orientación, el material y los cantos por lado.
6. Si interviene una variable sin definición o valor comprobable, **no deduzcas un resultado numérico definitivo** hasta verificar su procedencia.
7. Contrasta las medidas con el diseño y vuelve a revisarlas en el **Reporte de Producción**.

Consulta también la [Documentación oficial del Reporte de Producción](https://cabinet-report.gitbook.io/cabinet-report-docs/funcionalidades-de-cabinet-report/reporte-de-produccion) para entender las comprobaciones del despiece y de los parámetros por cliente.

## Continúa el aprendizaje

[Creación de Piezas →](creacion-de-piezas.md) · [Creación de Módulos](creacion-de-modulos.md) · [Catálogo de Módulos](catalogo-de-modulos.md) · [Reporte de Producción](reporte-de-produccion/README.md)

---

[← Portada del Curso](README.md) · [🏠 Portal principal](https://danielmelendez-pma.github.io/cabinet-report-partners/)
