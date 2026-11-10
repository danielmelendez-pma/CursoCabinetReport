---
description: >-
  Aprende a identificar la licencia de usuario de Cabinet Report, reconocer
  los controles históricos y comprobar su configuración sin divulgar códigos.
---

# Licencia de Usuario

**Etapa del curso · Funciones de Ingreso y Licencias**

La **licencia de usuario** es la referencia asociada a una persona usuaria dentro del cliente titular de Cabinet Report, según la descripción del curso original y la [Documentación Oficial de Licencia de Cliente](https://cabinet-report.gitbook.io/cabinet-report-docs/funcionalidades-de-cabinet-report/licencia-de-cliente). La documentación histórica indica que la suministra el proveedor del software. Esta guía explica cómo reconocer el dato en la ventana de licencias, pero **no confirma un formato técnico ni el comportamiento de validación de todas las versiones Windows**.

## Distingue la licencia de usuario de los demás datos

| Dato | Qué identifica | No debe confundirse con… |
| --- | --- | --- |
| **Nombre del cliente** | Empresa o persona titular registrada para el uso de Cabinet Report. | El cliente o ambiente de un proyecto de fabricación. |
| **Licencia de Cliente** | Referencia asignada al cliente titular para su configuración. | La licencia particular de una persona usuaria. |
| **Licencia de Usuario** | Referencia asociada a un usuario dentro del cliente, de acuerdo con la documentación histórica. | Su nombre para iniciar sesión o su contraseña. |
| **Usuario y contraseña** | Credenciales asignadas para solicitar el inicio de sesión. | Los códigos de licencia de cliente y usuario. |

La **licencia de cliente no sustituye la licencia de usuario**, y ninguna de las dos debe tratarse como una contraseña. Si aún no has identificado al titular, comienza por [Nombre de Cliente](funciones-de-ingreso-y-licencias/nombre-de-cliente.md) y [Licencia de Cliente](licencia-de-cliente.md). Para ingresar después, consulta [Inicio de Sesión](inicio-de-sesion.md).

## Reconoce la ventana de licencias

<figure><img src=".gitbook/assets/image (2) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1).png" alt="Captura histórica de la ventana de licencias de Cabinet Report utilizada para localizar Licencia Usuario, los controles Cambiar y la información de vigencia de la licencia"><figcaption><p>Captura original conservada del curso. Sirve para reconocer los rótulos y controles documentados históricamente; no demuestra qué formatos, estados o fechas valida la versión actualmente instalada.</p></figcaption></figure>

| Elemento documentado | Función en la explicación histórica | Precaución |
| --- | --- | --- |
| **Cliente** | Identifica el nombre del titular de la instalación. | No es el nombre de un proyecto ni una licencia individual. |
| **Licencia Cliente** | Campo destinado a la referencia del cliente titular. | No introduzcas aquí una referencia de usuario. |
| **Licencia Usuario** | Campo donde el curso indica ingresar la licencia correspondiente al usuario. | No es el campo del nombre de usuario ni de la contraseña. |
| **Cambiar** | Acción descrita junto al campo para solicitar un cambio del dato introducido. | Pulsarlo no acredita por sí solo que el valor se guardó o fue aceptado. |
| **Rojo / verde** | Colores mencionados en el relato histórico como indicación del resultado. | Su significado y vigencia en versiones actuales requieren comprobación. |
| **Fecha de Vencimiento / Tiempo Restante** | Información que, según el texto antiguo, se mostraba debajo de la licencia. | No demuestra cómo se calculan esos valores ni las condiciones contractuales vigentes. |

**Nota:** los rótulos anteriores proceden del material histórico. La posición, disponibilidad y respuesta de los controles pueden cambiar entre versiones. Confirma siempre qué muestra tu propia instalación.

## Discrepancia histórica: «ocho dígitos» frente al ejemplo

El texto original afirma que el código de licencia de usuario tiene **ocho dígitos**, pero el ejemplo que presenta contiene **ocho caracteres: dos letras y seis cifras**. Por tanto, la expresión «ocho dígitos» no describe literalmente su propio ejemplo.

Se conserva a continuación el **encabezado histórico exacto**, para no romper posibles enlaces a su ancla. **No es una licencia válida confirmada ni un patrón para generar licencias.**

## CL000001

**Ejemplo exclusivamente histórico del curso.** La secuencia anterior comienza con las letras **CL** y continúa con seis cifras. No permite concluir que todas las licencias empiecen igual, que su longitud actual sea ocho ni que el programa admita ese patrón.

**No conviertas el ejemplo a ocho números, no elimines letras ni deduzcas un algoritmo de emisión.** Solo el proveedor, el administrador autorizado o una especificación técnica verificable pueden confirmar el dato que corresponde a cada usuario. Esta discrepancia permanece **pendiente de validación técnica y funcional**.

## Paso a paso: comprobación inicial de la licencia de usuario

1. **Identifica al cliente titular y al usuario autorizado.** Confirma con el responsable de licencias que ambos corresponden a la instalación que vas a utilizar; no confundas al titular con el cliente de un proyecto.
2. **Obtén la referencia de usuario por un canal autorizado.** No copies el ejemplo histórico ni utilices licencias mostradas en capturas ajenas.
3. **Abre Cabinet Report** y accede a la ventana de licencias cuando la instalación o el responsable te indique que debes configurar este dato.
4. **Localiza el campo Licencia Usuario.** Distingue este rótulo de **Cliente** y **Licencia Cliente** antes de escribir nada.
5. **Introduce el dato exactamente como lo suministró el emisor.** No cambies longitud, separadores, letras o cifras para ajustarlo al ejemplo antiguo.
6. **Utiliza el botón Cambiar correspondiente solo si estás autorizado y está disponible.** Es la acción citada en la guía histórica, pero no se presume que su mecánica actual sea idéntica.
7. **Comprueba la respuesta efectiva de la aplicación.** Lee cualquier aviso, verifica a qué campo se refiere y registra únicamente el resultado no sensible. No interpretes un clic o un color aislado como confirmación suficiente.
8. **Continúa al inicio de sesión** únicamente cuando el responsable confirme que las referencias requeridas están correctamente configuradas. Para ingresar se usan por separado las [credenciales de acceso](inicio-de-sesion.md).

Esta secuencia es una **orientación pedagógica basada en controles documentados**, no un ensayo ejecutado en Windows ni una garantía de activación.

## ¿Qué significan Cambiar y los colores rojo/verde?

La guía original dice que, al introducir la licencia de usuario y pulsar **Cambiar**, **un campo rojo pasaría a verde cuando el valor fuera correcto**. Esta es una **descripción histórica**, no una validación actual.

Conviene distinguir:

- **Evidencia del curso:** se nombra el botón **Cambiar** y se relata el paso de rojo a verde.
- **Resultado observado en la instalación:** el mensaje y el estado que realmente aparezcan tras la acción, asociados al campo que se intentó actualizar.
- **Pendiente de pruebas:** confirmar en Windows la lógica de aceptación, qué campo cambia de color, si existe algún paso adicional y qué ocurre ante valores no reconocidos.

Una indicación verde, por sí sola, **no confirma** que el usuario pueda iniciar sesión, que se haya renovado una suscripción ni que se hayan habilitado funciones o permisos adicionales.

## Vigencia, fecha de vencimiento y tiempo restante

El texto histórico señala que, después de ingresar la licencia, aparecerían una **fecha de vencimiento** y un **tiempo restante**. Estos rótulos son distintos de la licencia de usuario: describir una fecha o un contador **no define el formato ni demuestra la aceptación del código**.

La documentación consultada no permite confirmar para la versión actual cómo se obtienen o actualizan esos datos, si corresponden a la licencia del cliente o del usuario, ni qué ocurre al agotarse el tiempo mostrado. **No infieras fechas de cobro, renovaciones, períodos de gracia, desconexiones o bloqueos** a partir de la captura. Contrasta el estado con el administrador autorizado y las condiciones aplicables.

## Si la licencia de usuario no es reconocida

| Situación | Qué comprobar de forma segura |
| --- | --- |
| **El campo rechaza el dato o aparece un aviso.** | Confirma que escribiste la referencia de **Licencia Usuario** en su campo y que corresponde al usuario indicado por el responsable. No improvises otro formato. |
| **El nombre del cliente o la licencia de cliente no coinciden.** | Verifica primero [Nombre de Cliente](funciones-de-ingreso-y-licencias/nombre-de-cliente.md) y [Licencia de Cliente](licencia-de-cliente.md). Evita sustituir referencias entre titulares. |
| **Pulsaste Cambiar y el resultado es ambiguo.** | Lee el mensaje visible y distingue el indicador del campo concreto. No des por aceptado el valor solo por otro color de la pantalla. |
| **Aparece fecha de vencimiento o tiempo restante.** | Consulta su interpretación con quien administra las licencias; no presupongas vigencia contractual ni fecha de renovación. |
| **La licencia parece aceptada pero no puedes iniciar sesión.** | Revisa por separado el usuario y la contraseña en [Inicio de Sesión](inicio-de-sesion.md). |
| **Persiste el problema.** | Informa la versión instalada, el rótulo utilizado, la operación realizada y el texto **no sensible** del aviso. Contacta al administrador o al [soporte autorizado](https://cabinet-report.gitbook.io/cabinet-report-docs/politicas-de-soporte). |

Estas comprobaciones **no acreditan** una causa concreta como conexión a Internet, validación en servidor, restricciones por equipo o permisos particulares. Cualquier regla de ese tipo necesita documentación técnica o pruebas verificables.

## Protege los códigos y las credenciales

- **No publiques licencias completas**, contraseñas ni capturas que permitan copiarlas. Oculta los valores antes de compartir una imagen, video o reporte de incidencia.
- **No reutilices referencias ajenas ni intentes construir códigos** a partir del ejemplo histórico. Solicita cada asignación a la persona responsable.
- **Comparte solamente el contexto necesario** para soporte: versión del programa, campo afectado, operación y texto no sensible del aviso.
- **No confundas titular, usuario y proyecto.** Los datos de licenciamiento corresponden al acceso autorizado, no al identificador de un ambiente de fabricación.

## Ejercicio didáctico con datos ficticios

**Caso simulado, solo para practicar en papel; no introduzcas estos datos en Cabinet Report.** La empresa imaginaria **Taller Modelo** tiene una referencia de cliente ficticia **no reproducida**. Su colaboradora **Persona Ejemplo** dispone de otra referencia de usuario ficticia **no reproducida**, además de un nombre de acceso y una contraseña distintos.

1. Identifica qué dato pertenece al **cliente titular**, cuál identifica al **usuario licenciado** y cuáles son las **credenciales de inicio de sesión**.
2. Localiza en la captura el campo **Licencia Usuario** y describe cuál sería el control **Cambiar** asociado.
3. Explica por qué el encabezado histórico anterior **no prueba** que todas las licencias tengan ocho dígitos numéricos.
4. Si la aplicación no reconoce una referencia, redacta un reporte con **versión, campo, paso realizado y aviso**, sin incluir códigos completos ni contraseñas.
5. Señala por qué un cambio rojo/verde o una fecha visible **no bastan** para acreditar una sesión iniciada ni el estado contractual actual.

**Autoevaluación:** el ejercicio se supera cuando distingues los cuatro datos, reconoces el control histórico, identificas la discrepancia de formato y puedes comunicar una incidencia sin revelar secretos. No equivale a activar una licencia ni a ejecutar pruebas funcionales.

## Fuentes, comprobaciones y límites

- **Verificado en la lección original:** la frase «ocho dígitos», el ejemplo **CL000001**, la imagen conservada, la referencia al botón **Cambiar**, el relato rojo/verde y la mención de **Fecha de Vencimiento** y **Tiempo Restante**.
- **Contrastado con el curso:** [Funciones de Ingreso y Licencias](<README (1).md>), [Nombre de Cliente](funciones-de-ingreso-y-licencias/nombre-de-cliente.md), [Licencia de Cliente](licencia-de-cliente.md) e [Inicio de Sesión](inicio-de-sesion.md).
- **Contrastado con la documentación oficial:** [Licencia de Cliente](https://cabinet-report.gitbook.io/cabinet-report-docs/funcionalidades-de-cabinet-report/licencia-de-cliente), [Inicio de Sesión](https://cabinet-report.gitbook.io/cabinet-report-docs/funcionalidades-de-cabinet-report/inicio-de-sesion) y [Manual de Usuario](https://cabinet-report.gitbook.io/cabinet-report-docs/manual-de-usuario). Distinguen identificación, referencias y credenciales, pero no resuelven el patrón histórico de caracteres.
- **Alcance de la revisión técnica:** en la documentación técnica pública consultada no se encontró una especificación verificable del formato de licencia de usuario ni de la lógica actual del botón **Cambiar**. Esto **no prueba** que tal especificación no exista en el código o en documentación interna.
- **Pendiente de validar:** formato admitido, asignación efectiva, cambios de color, mensajes, vigencia, cálculos de fecha/tiempo, accesibilidad visual de GitBook, enlaces HTTP, Git Sync y comportamiento de la aplicación Windows.

Para seguir la secuencia del curso, vuelve a [Funciones de Ingreso y Licencias](<README (1).md>) y continúa con [Inicio de Sesión](inicio-de-sesion.md). Si ya tienes acceso y necesitas reportar un incidente, consulta [Reporte de Errores o Feedback](reporte-de-errores-o-feedback.md).

[← Licencia de Cliente](licencia-de-cliente.md) · [Inicio de Sesión →](inicio-de-sesion.md) · [Portada del Curso](README.md) · [🏠 Portal principal](https://danielmelendez-pma.github.io/cabinet-report-partners/)
