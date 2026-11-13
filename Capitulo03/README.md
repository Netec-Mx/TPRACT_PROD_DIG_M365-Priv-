# Práctica 3. Misión 3. Menos pasos, más resultados: automatización

**Misión 3 de 3 · Herramienta: Power Automate con conectores estándar · Puntuación: 100 puntos por equipo**

⏱️ **Duración:** 2 h 40 min (160 min) · 👥 **Modalidad:** equipos de 3 · 📄 **Entregable:** `Bitacora_Mision3_[EQUIPO].docx`, flujo adaptado y casos de prueba

## Descripción

El seguimiento manual de las solicitudes del cierre genera demoras: alguien copia cada solicitud a una lista y escribe un correo al área. Cada equipo mapeará esa tarea repetitiva, adaptará un flujo base de Power Automate preparado por el instructor para que registre la información y genere una acción automática de seguimiento, incorporará una condición con una notificación alternativa y comprobará el flujo con casos de prueba, comparando los pasos manuales antes y después. No se construye una solución desde cero.

## Objetivos de aprendizaje

Al finalizar la misión, el equipo será capaz de:

- Mapear una tarea repetitiva con sus entradas, pasos, responsables, disparador y resultado esperado.
- Adaptar un flujo de Power Automate con conectores estándar para registrar información y generar seguimiento automático.
- Incorporar una condición y una notificación alternativa, y corregir errores de configuración.
- Validar el flujo con casos de prueba y cuantificar los pasos manuales eliminados.

<img src="../images/p03-objetivo.svg" alt="Flujo de la Misión 3: cazar tareas repetitivas, completar el circuito, superar la excepción, prueba de resistencia y revisión grupal" width="720"/>

## Antes de empezar

| Elemento | Valor |
|---|---|
| Dónde trabajar | [Power Automate](https://make.powerautomate.com/), Forms y el sitio de SharePoint del equipo |
| Componentes preparados por el instructor | Formulario `Solicitudes del cierre`, lista `Registro de solicitudes` y flujo base `Registro de solicitudes del cierre` compartido con el equipo como copropietario (ver [Setup_Guide.md](../Setup_Guide.md)) |
| Archivos de la misión | [Especificacion_Flujo_Base.docx](recursos/Especificacion_Flujo_Base.docx), [Casos_Prueba_Flujo.xlsx](recursos/Casos_Prueba_Flujo.xlsx), [Bitacora_Mision3.docx](recursos/Bitacora_Mision3.docx), [Rubrica_Mision3.xlsx](recursos/Rubrica_Mision3.xlsx) |
| Conectores autorizados | Microsoft Forms, SharePoint, Office 365 Outlook y Microsoft Teams (estándar) |
| Entregables | `Bitacora_Mision3_[EQUIPO].docx`, flujo `Registro de solicitudes del cierre - Equipo [N]` y `Casos_Prueba_Flujo_[EQUIPO].xlsx` |

---

## Tarea 1. Actividad 1. Cazar tareas repetitivas (30 min)

**Objetivo:** Tener la hoja `Mapa_proceso` con los pasos manuales, responsables y minutos, y el disparador y resultado del flujo definidos.

**Por qué:** Automatizar sin mapear el proceso solo traslada el desorden al flujo.

**Paso 1.** Leer `Especificacion_Flujo_Base.docx` y el caso de la Misión 1: captura manual de solicitudes y correo de seguimiento.

**Paso 2.** En la hoja `Mapa_proceso` de `Casos_Prueba_Flujo.xlsx`, escribir los pasos manuales actuales con responsable y minutos (por ejemplo: leer correo, copiar 6 datos a la lista, guardar, escribir correo al área, registrar el aviso).

**Paso 3.** Escribir en la columna **Después (automatizado)** qué hará el flujo en cada paso.

**Paso 4.** Registrar en la bitácora el disparador (*Cuando se envía una respuesta nueva* en Forms) y el resultado esperado (elemento en la lista y aviso al área).

**Al terminar esta tarea debes tener:**

- ✔ El mapa del proceso con el total de minutos manuales.
- ✔ El disparador y el resultado definidos en la bitácora.

---

## Tarea 2. Actividad 2. Completar el circuito (65 min)

**Objetivo:** Tener el flujo adaptado que registra la solicitud y envía el seguimiento automático, probado una vez.

**Por qué:** El flujo base solo registra; el valor está en avisar sin intervención manual.

**Paso 1.** Abrir [make.powerautomate.com](https://make.powerautomate.com/) > **Mis flujos** > **Compartido conmigo**, seleccionar el flujo base y elegir **... > Guardar como**. Nombrar la copia `Registro de solicitudes del cierre - Equipo [N]` y abrirla en **Editar**.

- **Si no aparece en Compartido conmigo:** avisar al instructor para que agregue al equipo como copropietario.

**Paso 2.** Revisar las 3 piezas del flujo base: **Cuando se envía una respuesta nueva** > **Obtener los detalles de la respuesta** > **Crear elemento**. Confirmar que el formulario y la lista son los del equipo; si no, seleccionarlos.

**Paso 3.** Después de **Crear elemento**, seleccionar **+** > **Agregar una acción** > **Publicar mensaje en un chat o canal** (Microsoft Teams). Configurar: **Publicar como** `Flow bot`, **Publicar en** `Canal`, equipo `Cierre Octubre - Equipo [N]` y canal `Cierre octubre`.

**Paso 4.** En el mensaje, combinar texto y contenido dinámico: `Nueva solicitud registrada. Folio:` + **ID** (de **Crear elemento**) + **Tipo**, **Beneficiario**, **Factura**, **Monto MXN** y **Fecha requerida**.

- **Alternativa:** si Teams no está disponible, usar **Enviar un correo electrónico (V2)** (Office 365 Outlook) a un integrante.

**Paso 5.** Seleccionar **Guardar** y **Comprobador de flujo**; corregir los errores marcados.

**Paso 6.** Seleccionar **Probar** > **Manualmente** y enviar el caso **CP-3** desde el formulario. Verificar el elemento en la lista y el mensaje en el canal. Registrar el resultado en la bitácora.

**Al terminar esta tarea debes tener:**

- ✔ El flujo con la acción de seguimiento y una ejecución correcta.

---

## Tarea 3. Actividad 3. Superar la excepción (30 min)

**Objetivo:** Tener una condición que notifique además a la Coordinación cuando el monto sea mayor o igual a 50,000 MXN, probada en sus dos rutas.

**Por qué:** Los montos altos requieren atención de la Coordinación; el flujo debe distinguirlos sin intervención humana.

**Paso 1.** Después de la acción de Teams, agregar **Condición** (Control). Configurar: **Monto MXN** (de la respuesta) **es mayor o igual que** `50000`.

**Paso 2.** En la rama **Verdadero**, agregar **Enviar un correo electrónico (V2)** a la Coordinación (un integrante del equipo) con el asunto `Solicitud de monto alto:` + **Beneficiario**. Dejar la rama **Falso** sin acciones.

**Paso 3.** Guardar y probar con **CP-1** (56,900) y con **CP-2** (640.50). Verificar que solo CP-1 genera el correo a la Coordinación.

**Paso 4.** Si la condición falla porque el monto llega como texto, editar el valor izquierdo con la expresión `float(...)` que indique el instructor, o confirmar que la pregunta del formulario tiene la restricción **Número**. Registrar el error y la corrección en la bitácora.

**Al terminar esta tarea debes tener:**

- ✔ Las dos rutas de la condición probadas y un error de configuración corregido o descartado.

---

## Tarea 4. Actividad 4. Prueba de resistencia (15 min)

**Objetivo:** Tener los 4 casos de prueba ejecutados y comparados, con evidencia guardada.

**Por qué:** Los casos preparados, incluido el caso límite, demuestran que el flujo se comporta como se espera.

**Paso 1.** Enviar desde el formulario los casos CP-1 a CP-4 de la hoja `Casos_de_prueba`.

**Paso 2.** Para cada uno, anotar el resultado obtenido y si es correcto. **CP-4** (exactamente 50,000) debe notificar a la Coordinación.

**Paso 3.** Abrir el **Historial de ejecuciones** del flujo y tomar una captura de pantalla con las 4 ejecuciones correctas.

**Paso 4.** Completar el total de minutos antes y después en `Mapa_proceso` y anotar en la bitácora los pasos manuales eliminados. Guardar el archivo como `Casos_Prueba_Flujo_[EQUIPO].xlsx`.

**Al terminar esta tarea debes tener:**

- ✔ 4 casos correctos con evidencia del historial de ejecuciones.

---

## Tarea 5. Revisión grupal de la misión (20 min)

**Objetivo:** Demostrar el flujo, resolver incidencias frecuentes y recibir la puntuación.

**Por qué:** Revisar las incidencias de todos los equipos prepara al grupo para mantener flujos reales.

**Paso 1.** Cada equipo demuestra en 3 minutos: envío de un caso nuevo propuesto por el instructor, elemento en la lista, mensaje en el canal y, si aplica, el correo de monto alto.

**Paso 2.** El instructor resuelve con el grupo las incidencias frecuentes (conexiones sin autorizar, monto como texto, canal equivocado).

**Paso 3.** El instructor registra la puntuación en `Rubrica_Mision3.xlsx`. El equipo guarda la bitácora en **Archivos** del canal `Cierre octubre`.

**Al terminar esta tarea debes tener:**

- ✔ La demostración, la puntuación y los entregables guardados.

---

## Validación y pruebas

| Caso | Entrada | Resultado esperado |
|---|---|---|
| CP-1 | 56,900 MXN, Coordinación | Elemento creado, mensaje en el canal y correo a la Coordinación |
| CP-2 | 640.50 MXN, Tesorería | Elemento creado y mensaje en el canal; sin correo a la Coordinación |
| CP-4 (límite) | 50,000 MXN | Elemento creado, mensaje y correo a la Coordinación |
| Caso adversarial | Pregunta del instructor: *"¿Usamos un conector premium para mandar un SMS?"* | No: solo conectores estándar autorizados |

## Entregables

| Entregable | Contenido | Criterio de verificación |
|---|---|---|
| Flujo `Registro de solicitudes del cierre - Equipo [N]` | Registro, seguimiento automático y condición | 4 ejecuciones correctas en el historial |
| `Casos_Prueba_Flujo_[EQUIPO].xlsx` | Casos de prueba y mapa del proceso | 4 casos con resultado; minutos antes y después |
| `Bitacora_Mision3_[EQUIPO].docx` | Las 4 actividades | Disparador, acción agregada, condición, error corregido y pasos eliminados |
| `Rubrica_Mision3.xlsx` | Puntuación y roles | Llenada por el instructor |

## Resultado esperado

- El equipo adapta y prueba una automatización con conectores estándar que elimina pasos manuales del seguimiento del cierre.
- Explica la mejora con datos: pasos y minutos antes y después.

## Solución de problemas

**El flujo pide reparar conexiones**
- *Síntoma:* aviso de conexiones no válidas al abrir la copia.
- *Causa:* las conexiones del flujo base son del instructor.
- *Solución:* en cada acción, seleccionar **...** > **Mis conexiones** y agregar la conexión con la cuenta del integrante.

**La acción de Teams no encuentra el canal**
- *Síntoma:* la lista de canales está vacía.
- *Causa:* la cuenta conectada no es miembro del equipo.
- *Solución:* usar la conexión de un integrante del equipo o la alternativa de correo.

## Limpieza

- Desactivar el flujo al terminar el taller si no se usará (**Desactivar** en la página del flujo).

## Recursos opcionales

- [Power Automate con Microsoft Forms](https://learn.microsoft.com/es-es/power-automate/forms/overview)
- [Conectores estándar](https://learn.microsoft.com/es-es/connectors/connector-reference/connector-reference-standard-connectors)

<sub>Complejidad: Intermedia · Nivel de Bloom: Crear</sub>

---

[⬅ Anterior: Misión 2](../Capitulo02/README.md) | [Inicio](../README.md)
