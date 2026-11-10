---
description: Aprende a identificar variables dimensionales, espesores, cantos y luces, y a comprobar fórmulas de piezas antes de utilizarlas en producción.
---

# Fórmulas y Variables

Las fórmulas permiten que las medidas de una pieza se recalculen al cambiar las dimensiones o los parámetros del módulo. Antes de crear una pieza, distingue **la variable que se escribe en la fórmula** del **valor que toma esa variable** al trabajar con un módulo concreto.

**Recorrido de aprendizaje:** identifica las dimensiones del módulo → distingue espesores y tipos de canto → verifica rieles y luces → rastrea los valores efectivos → calcula un caso de ensayo → comprueba las piezas en el módulo y en el RP.

**Convención:** las medidas de los ejercicios se expresan en **milímetros (mm)**. En una pieza, **espesor, ancho y largo** son campos distintos; una expresión escrita para uno no determina automáticamente los otros dos. Cuando se mencione una fórmula del ejemplo histórico, se indicará su origen. Las operaciones nuevas de esta lección serán ejercicios aritméticos, no reglas afirmadas del motor de Cabinet Report.

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

**De dónde salen:** consulta `PROF`, `ANCHO` y `ALTO` en las dimensiones del **módulo concreto** que estás preparando. La pieza puede tener dimensiones finales menores, mayores o distintas por su construcción y por las expresiones asignadas; no sustituyas las dimensiones del módulo por una medida visible de otra pieza.

Una misma fórmula puede producir resultados distintos si cambian `PROF`, `ANCHO` o `ALTO`.

## 2. Espesores y respaldo

| Variable | Qué representa |
| --- | --- |
| `ESPC` | Espesor del tablero del cuerpo o cajón del mueble, en las partes que no quedan vistas tras la instalación. |
| `ESPV` | Espesor del tablero de partes visibles, como puertas y costados vistos. |
| `RESP` | Espesor del tablero delgado que se inserta en ranuras para respaldos o fondos de gavetas. |

**No son intercambiables.** `ESPC` y `ESPV` designan usos distintos según la pieza; `RESP` describe el espesor del material de respaldo o fondo en la definición documentada. Para conocer su **valor numérico efectivo**, consulta el tablero seleccionado y la configuración realmente aplicada. El tipo de tablero `CART` mencionado en [Creación de Tableros](creacion-de-tableros.md) no define por sí mismo una variable dimensional con ese mismo nombre.

La elección del tablero y su espesor debe corresponder a la pieza real. `ESPC` y `ESPV` pueden tener valores diferentes.

{% hint style="warning" %}
**Variable histórica sin definición comprobada:** la fórmula de la `BASE` en [Creación de Piezas](creacion-de-piezas.md) contiene `CART`, pero esta lección no acredita su significado técnico. No sustituyas `CART` por `RESP` ni le atribuyas **3 mm** o **4 mm** por inferencia. Comprueba su procedencia y valor efectivo en la versión y el catálogo utilizados.
{% endhint %}

## 3. Cantos

| Variable | Uso documentado |
| --- | --- |
| `CVISTO` | Canto o cintillo utilizado en los lados frontales o visibles. |
| `CCAJON` | Canto o cintillo para lados internos, traseros o no visibles. |

En el [Catálogo de Módulos](catalogo-de-modulos.md) también se revisa el **espesor físico del canto**. El tipo de canto (`CVISTO` o `CCAJON`) y una posible reducción dimensional por canteo son conceptos distintos: no agregues un descuento a la fórmula solo por el nombre de la referencia.

Estas referencias **identifican el canto que se asigna a un borde**; no deben confundirse con `ANCHO`, `LARGO` ni con una luz en milímetros. Revisa qué lado de la pieza corresponde a cada canto en el [Creador de Piezas](creacion-de-piezas.md).

## 4. Rieles de gavetas

| Variable | Uso documentado |
| --- | --- |
| `RE` | Espesor o espacio consumido por el riel al calcular anchos internos de gaveta. |
| `RL` | Largo del riel para calcular laterales de gaveta. |
| `RA` | Altura del riel cuando se utiliza un riel lateral metálico. |

**Secuencia de comprobación:** identifica el riel seleccionado en el catálogo o módulo, anota su referencia y sus valores, verifica que la **pieza correspondiente** utilice esa variable en la dimensión prevista y contrasta las medidas calculadas con la ficha real del herraje. No presupongas que todo sistema de gavetas usa el mismo riel, holgura o fórmula.

### Variantes de nombre y expresiones pendientes de contraste

Los identificadores `REGR`, `RLGR` y `RAGR` se han señalado para revisión de variantes de riel, pero **su disponibilidad, significado exacto y equivalencia con `RE`, `RL` y `RA` no quedan acreditados por las lecciones públicas contrastadas**. Si aparecen en tu versión, registra el nombre literal, el control donde se muestran, el valor aplicado y la fórmula de la pieza antes de documentar su semántica. **No los sustituyas** por la variable sin sufijo por similitud del nombre.

Algunas definiciones pueden incorporar operaciones alrededor del largo de riel. Como **ejercicio de cálculo manual**, si una ficha de ensayo establece `RL = 450 mm`, entonces `RL - 10` daría `440 mm`. Esto **no verifica** que el editor de tu versión admita expresiones, signos `+`, `-`, `*`, `/`, paréntesis o una variante `RLGR`. Comprueba su sintaxis aceptada y el resultado mostrado **en una copia de ensayo**; no guardes cambios sobre piezas compartidas para averiguarlo.

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

### Parámetro general, valor efectivo y datos no recuperados

| Concepto | Qué se puede afirmar | Comprobación necesaria |
| --- | --- | --- |
| **Nombre de variable** | Identifica el término escrito en la fórmula (`LIZ`, `ESPV`, `RL`…). | Copiar la expresión exacta de **esa pieza**. |
| **Definición general o de catálogo** | Sirve de referencia para preparar estructuras. | Consultar el catálogo y la definición seleccionada. |
| **Valor efectivo del cliente/módulo** | Es el número realmente aplicado al cálculo de ese trabajo. | Identificar cliente, módulo, versión, tablero, herraje y parámetros seleccionados. |
| **Valor no recuperado o no comprobable** | **No equivale a cero** y no prueba que se haya aplicado una referencia general. | Registrar **PENDIENTE**, conservar la evidencia y no aprobar el cálculo. |
| **Resultado calculado o editado** | Es la dimensión que se está revisando; por sí sola no revela qué valores se utilizaron. | Contrastar fórmula, sustitución de variables, orientación y edición posterior. |

**El cero es un dato válido.** Si `LIZ = 0 mm` es el valor efectivo comprobado, la fórmula debe evaluarse con **0**, no con otra luz sugerida por una tabla general. A la inversa, si falla la consulta del parámetro del cliente, **no escribas 0 ni uses un valor público como si estuviera acreditado**. Registra el fallo y vuelve a comprobar los datos en la aplicación.

**Procedencia mínima:** anota versión instalada, cliente y ambiente, catálogo y módulo, pieza identificable, expresiones de espesor/ancho/largo, valor y origen de cada variable utilizada, resultado calculado, resultado visible y ajustes manuales conocidos. Los parámetros pueden variar entre proyectos, incluso si se reutiliza un nombre de pieza.

{% hint style="warning" %}
**Alcance de la evidencia:** la [Documentación Oficial del RP](https://cabinet-report.gitbook.io/cabinet-report-docs/funcionalidades-de-cabinet-report/reporte-de-produccion) exige contrastar los valores efectivos, pero estas páginas no certifican el mecanismo interno de prioridad, recuperación, caché ni sustitución automática de valores en todas las versiones. No atribuyas una discrepancia a ese mecanismo sin una prueba funcional.
{% endhint %}

## 6. Ejemplo de lectura de una fórmula

### Dos puertas: fórmula histórica y cálculo controlado

En [Creación de Piezas](creacion-de-piezas.md) se conserva la siguiente expresión de **ancho para cada hoja** del ejemplo de dos puertas:

```text
(ANCHO - LIZ - LDE - LCE) / 2
```

Y la siguiente expresión de **alto**:

```text
ALTO - LSU - LIN
```

La fórmula histórica utiliza `ESPV` para el **espesor** de ambas puertas. Son tres campos de pieza diferentes: **`ESPV` × ancho calculado × alto calculado**. Los valores de esta tabla son exclusivamente **didácticos**, no valores predeterminados del sistema:

| Dato del ensayo | Valor |
| --- | ---: |
| `ANCHO` del módulo | 900 mm |
| `LIZ`, `LDE` y `LCE` | 2 mm cada uno |
| `ALTO` del módulo | 780 mm |
| `LSU` y `LIN` | 2 mm cada uno |
| `ESPV` | 18 mm |

**Cálculo manual:** `(900 - 2 - 2 - 2) / 2 = 447 mm` por hoja; `780 - 2 - 2 = 776 mm` de alto. La pieza del ejercicio se describe como **18 × 447 × 776 mm**, siguiendo el orden espesor × ancho × largo del ejemplo histórico. Verifica la orientación real de ancho y largo en la pieza antes de transferirla al RP.

### Por qué 447 mm y 448 mm no son una contradicción demostrada

El resultado histórico de [Creación de Piezas](creacion-de-piezas.md) muestra **448 mm** por hoja, pero no acredita todos los valores de luz de ese caso. Con la **misma expresión**, las siguientes sustituciones matemáticas son posibles:

| Ensayo ilustrativo | `LIZ` | `LDE` | `LCE` | Suma de luces | Ancho por hoja |
| --- | ---: | ---: | ---: | ---: | ---: |
| A | 2 mm | 2 mm | 2 mm | 6 mm | 447 mm |
| B | 1 mm | 1 mm | 2 mm | 4 mm | 448 mm |

En ambos casos `ANCHO = 900 mm`. **El ensayo B no reconstruye ni demuestra los parámetros que realmente se usaron en la captura histórica**; solo explica qué sumas producirían matemáticamente ambos resultados. Falta acreditar la procedencia y el valor efectivo de las luces del ejemplo original.

**Puerta individual, otro ejemplo:** para una pieza de **una sola hoja** cuya fórmula verificada fuera `ANCHO - LIZ - LDE`, con `ANCHO = 450 mm` y luces **1,5 mm a cada lado**, el cálculo manual daría `450 - 1,5 - 1,5 = 447 mm`. Esta **no es la fórmula de dos hojas** ni prueba que una puerta real de 450 mm deba tener ese ancho; el tipo de apertura, el módulo, el sobre y las luces aplicables deben verificarse antes de aceptarla.

### Frentes de gavetas: ejercicio de separación, no fórmula del programa

`LGA` se documenta como luz **entre frentes de gavetas**. Para practicar cómo contabilizar espacios, supón una **abertura didáctica de 770 mm** con tres frentes iguales, luz superior de `2 mm`, inferior de `2 mm` y **dos** separaciones de `2 mm`:

```text
(770 - 2 - 2 - 2 × 2) / 3 = 254 mm por frente
```

Este cálculo es una **distribución geométrica ilustrativa**; **no se ha acreditado como fórmula existente ni como comportamiento automático** de Cabinet Report. No lo apliques a gavetas de alturas diferentes, rieles o variantes constructivas sin revisar la expresión de **cada frente**. Las golas (`GOL`) solo se descuentan si intervienen efectivamente en la fórmula aplicable, no por la presencia de un tirador en una imagen.

### Espesores y `CART`: otra diferencia histórica abierta

La descripción de [Creación de Piezas](creacion-de-piezas.md) habla de un respaldo de cartón de **4 mm**, pero el resultado «RESPALDO CART» muestra **3 mm**. Son evidencias incompatibles como **único valor efectivo** sin datos adicionales. Comprueba el tablero real, su espesor, `RESP` y la expresión usada antes de corregir una cifra.

En la `BASE`, la expresión histórica `PROF - ESPC - CART` presenta el término `CART` **sin definición técnica acreditada**. Aunque se pudiera despejar aritméticamente un número a partir del resultado impreso, ello **no determina qué representa `CART`** ni demuestra el origen del valor. No lo equipares automáticamente a `RESP` ni a la clasificación de material `CART`.

## 7. Comprobación antes de guardar una pieza

1. **Identifica el contexto:** versión, cliente, ambiente, tipo y variante del módulo, apertura, sobre y orientación, cuando correspondan. Confirma `PROF`, `ANCHO` y `ALTO` en su ficha.
2. **Rastrea la pieza exacta:** registra las tres expresiones de espesor, ancho y largo sin asumir que una pieza homónima utiliza la misma definición.
3. **Verifica los materiales:** contrasta `ESPC`, `ESPV`, `RESP`, tablero real y espesor; revisa la veta y el canto de cada lado.
4. **Identifica las variables usadas:** luces, golas, pines, ranuras, respaldo y rieles; no descuentes parámetros que **no figuren** en la expresión de la pieza.
5. **Acredita el valor efectivo:** registra origen y valor por cliente/módulo. Conserva el **0 válido** y marca como pendiente cualquier parámetro no recuperable.
6. **Recalcula manualmente:** sustituye los valores en el orden correcto, con paréntesis y unidades; si faltan variables o definiciones —como `CART`— **no presentes el resultado como verificado**.
7. **Contrasta lo visible:** revisa medida, cantidad, material, veta, cantos y cualquier edición manual de la pieza. Si no coincide, consulta **Mostrar Fórmulas** en el [Catálogo de Módulos](catalogo-de-modulos.md), sin asumir que cambiará una definición compartida.
8. **Comprueba el recorrido:** revisa la pieza en [Creación de Módulos](creacion-de-modulos.md), en el [Catálogo de Módulos](catalogo-de-modulos.md) y finalmente en el [Reporte de Producción](reporte-de-produccion/README.md), incluyendo el TXT si corresponde. No presupongas que un archivo ya generado se corrige por modificar después el catálogo.

### Registro sencillo de un ensayo reproducible

Trabaja con una copia de prueba y **dos configuraciones A/B** de la misma pieza identificada. Conserva los valores que realmente muestra el programa; no los reemplaces por los números didácticos anteriores.

| Evidencia | Configuración A | Configuración B |
| --- | --- | --- |
| Cliente, versión, módulo y pieza | Por registrar | Por registrar |
| Dimensiones del módulo y tipo de apertura | Por registrar | Por registrar |
| Fórmulas exactas y material de la pieza | Por registrar | Por registrar |
| Valores de variables y procedencia | Por registrar | Por registrar |
| Espesor, ancho y largo esperados por cálculo manual | Pendiente de cálculo | Pendiente de cálculo |
| Medidas realmente mostradas en el módulo/RP | Pendiente de observar | Pendiente de observar |
| Diferencia, explicación y evidencia | Pendiente de contrastar | Pendiente de contrastar |

**Resultado por control:** **CONFORME** si los datos y cálculos concuerdan con evidencia; **NO CONFORME** si existe una diferencia demostrada; **NO EJECUTADO** si la prueba no se realizó o faltan datos. No conviertas una operación didáctica en una prueba funcional del programa.

{% hint style="warning" %}
**Antes de fabricar:** un cálculo sin errores aparentes, una sugerencia del [Revisor IA](https://cabinet-report.gitbook.io/cabinet-report-docs/funcionalidades-de-cabinet-report/revisor-inteligencia-artificial) o un RP generado no sustituyen la comprobación de las medidas y condiciones reales de fabricación. Si hay incertidumbres técnicas, conserva la producción de ensayo y solicita la validación correspondiente.
{% endhint %}

## Continúa el aprendizaje

[Creación de Piezas →](creacion-de-piezas.md) · [Creación de Módulos](creacion-de-modulos.md) · [Catálogo de Módulos](catalogo-de-modulos.md) · [Reporte de Producción](reporte-de-produccion/README.md)

---

[← Portada del Curso](README.md) · [🏠 Portal principal](https://danielmelendez-pma.github.io/cabinet-report-partners/)
