# Práctica 1. Misión 1. Operación coordinada: rescatar una jornada de trabajo

**Misión 1 de 3 · Herramientas: Planner, Teams y Copilot Chat (si está habilitado) · Puntuación: 100 puntos por equipo**

⏱️ **Duración:** 2 h 40 min (160 min) · 👥 **Modalidad:** equipos de 3 · 📄 **Entregable:** `Bitacora_Mision1_[EQUIPO].docx`, plan `Tablero de rescate` y canal `Cierre octubre`

## Descripción

Es lunes 2 de noviembre de 2026. La Coordinación Administrativa y Financiera de Servicios Integrales del Centro (SIC) debe cerrar octubre: la conciliación bancaria vence el 4 de noviembre, el informe va a Dirección el 10 y el comité es el 11. Sin embargo, la jornada se perdió en buscar archivos, reuniones sin agenda y preguntas por chat. Su equipo diagnosticará esa jornada, convertirá las 16 actividades del cierre en un tablero de Planner, creará un canal de Teams para coordinar el cierre y publicará un mensaje operativo elaborado con Copilot Chat y verificado por el equipo.

## Objetivos de aprendizaje

Al finalizar la misión, el equipo será capaz de:

- Detectar interrupciones, duplicidades y tareas repetitivas en una jornada operativa y acordar tres mejoras prioritarias.
- Organizar las actividades del cierre en Planner con responsables, fechas, prioridades, criterios de avance y dependencias coherentes.
- Configurar en Teams un canal de coordinación con archivo principal, pestañas, acuerdos y actualizaciones de estado.
- Producir con Copilot Chat un mensaje operativo y una lista de pendientes, si el tenant lo habilita, y verificar sus datos antes de publicarlos.

<img src="../images/p01-objetivo.svg" alt="Flujo de la Misión 1: diagnóstico, tablero de rescate, canal de coordinación, mensaje de acción y revisión grupal" width="720"/>

## Antes de empezar

**Comprobación rápida:** necesita un equipo de Teams creado por el instructor, los cinco archivos de esta misión y acceso a Planner y Copilot Chat. Si falta alguno, confirme la preparación con el instructor antes de trabajar.

| Elemento | Valor |
|---|---|
| Espacio del equipo | Equipo de Teams `Cierre Octubre - Equipo [N]`, creado por el instructor con los 3 integrantes como propietarios |
| Archivos de la misión | [Caso_Jornada_Operativa.docx](recursos/Caso_Jornada_Operativa.docx), [Actividades_Cierre_Equipo.xlsx](recursos/Actividades_Cierre_Equipo.xlsx), [Notas_Trabajo.docx](recursos/Notas_Trabajo.docx), [Bitacora_Mision1.docx](recursos/Bitacora_Mision1.docx), [Rubrica_Mision1.xlsx](recursos/Rubrica_Mision1.xlsx) |
| Personajes del caso | Mario (Tesorería), Ana (Contabilidad), Julia (Planeación), Luis (Compras) |
| Fechas clave | Estados de cuenta: martes 3 nov · Conciliación: 4 nov · Informe a Dirección: 10 nov · Comité: 11 nov |
| Reparto de áreas en el equipo | **Integrante A:** Tesorería y Planeación · **Integrante B:** Contabilidad y Compras · **Integrante C:** Coordinación y Recursos Humanos |
| Entregables | `Bitacora_Mision1_[EQUIPO].docx`, plan `Tablero de rescate` y canal `Cierre octubre` |

> Sustituya `[N]` y `[EQUIPO]` por el número de su equipo (por ejemplo, `Equipo 2` y `Bitacora_Mision1_Equipo2.docx`). Todos los datos son ficticios.

**Roles rotativos.** En cada actividad, un integrante asume cada rol y los roles cambian en la siguiente actividad:

| Rol | Qué hace |
|---|---|
| **Coordinación** | Lee las instrucciones en voz alta, controla el tiempo y toma las decisiones finales |
| **Ejecución** | Comparte pantalla y opera la herramienta (Teams, Planner o Copilot Chat) |
| **Verificación** | Revisa el resultado con la lista "Al terminar esta tarea debes tener" y escribe la bitácora |

**Puntuación.** Al final de la misión, el instructor asigna una sola puntuación por equipo (máximo 100): funcionamiento (40), uso adecuado de herramientas (25), calidad y validación (20) y colaboración y explicación (15). Las actividades no se califican por separado.

---

## Tarea 1. Actividad 1. Diagnóstico del caos (30 min)

**Objetivo:** Tener la hoja `Diagnostico` con los 9 eventos de la jornada clasificados, con minutos perdidos, mejora y herramienta, y 3 mejoras prioritarias registradas en la bitácora.

**Por qué:** La jornada del caso duró 8 horas y casi ninguna se dedicó al cierre. Sin un diagnóstico compartido, cada integrante "mejora" algo distinto.

**Paso 1.** Abrir **Microsoft Teams**, seleccionar **Equipos** en la barra izquierda y abrir el canal **General** del equipo `Cierre Octubre - Equipo [N]`.

- **Qué verás:** las pestañas **Publicaciones** y **Archivos** en la parte superior del canal.
- **Si no ocurre así:** si el equipo no aparece, avisar al instructor para que lo agregue como propietario.

**Paso 2.** La persona en **Ejecución** descarga los 5 archivos de la tabla *Antes de empezar*. En GitHub, abra el enlace de cada archivo y use **Download raw file** si aparece; desde un paquete ZIP, extraiga primero los recursos. En el canal **General**, seleccionar la pestaña **Archivos** > **Cargar** > **Archivos** y seleccionar los 5 archivos.

- **Qué verás:** los 5 archivos listados en **Archivos**, visibles para todo el equipo.
- **Alternativa:** si el instructor ya cargó los archivos, omitir este paso.

**Paso 3.** Seleccionar `Rubrica_Mision1.xlsx`, ir a la hoja `Roles` y escribir el nombre de quién tiene cada rol en la **Actividad 1**. Cerrar el archivo; se guarda solo.

**Paso 4.** Abrir `Caso_Jornada_Operativa.docx` desde **Archivos** y leer en equipo los 9 eventos de la jornada (de 8:00 a 17:00).

**Paso 5.** Abrir `Actividades_Cierre_Equipo.xlsx` desde **Archivos** (se abre en Teams o en Excel para la web) y seleccionar la hoja `Diagnostico`. Llenar una fila por evento. Los tres integrantes pueden escribir al mismo tiempo en el archivo.

| Columna | Qué escribir |
|---|---|
| Hallazgo | El evento, en pocas palabras |
| Tipo | **Interrupción** (corta el trabajo sin aportar), **Duplicidad** (el mismo dato o archivo existe más de una vez) o **Tarea repetitiva** (se hace a mano lo mismo cada vez) |
| Tiempo perdido estimado (min) | La duración del evento, según el horario del caso |
| Mejora propuesta | Qué cambiaría para que no vuelva a ocurrir |
| Herramienta | Planner, Teams, SharePoint, Forms o Power Automate |

- **Ejemplo de una fila llena:** `Se buscan los estados de cuenta en 3 correos` · **Duplicidad** · `40` · `Un solo lugar para los archivos del cierre, sin enviarlos por correo` · **Teams (Archivos del canal)**.
- **Importante:** un evento puede tener más de un tipo; elegir el que más tiempo hace perder.

**Paso 6.** Sumar la columna de minutos: escribir `=SUMA(C2:C10)` en la celda `C11`.

- **Qué verás:** el total de minutos perdidos de la jornada (debe acercarse a 480, es decir, casi toda la jornada).

**Paso 7.** Elegir en equipo las **3 mejoras prioritarias**: las que recuperan más minutos con menos esfuerzo de implementación. Abrir `Bitacora_Mision1.docx` desde **Archivos**, escribir en la parte superior el número de equipo y los integrantes y, en la sección **Actividad 1. Diagnóstico**, llenar *Tres mejoras prioritarias acordadas* y *Minutos recuperables estimados* (la suma de los minutos de los eventos que resuelven).

- **Importante:** la bitácora se llena al final de cada actividad; no esperar al final de la misión.

**Al terminar esta tarea debes tener:**

- ✔ 9 filas en la hoja `Diagnostico` con tipo, minutos, mejora y herramienta, y el total en `C11`.
- ✔ 3 mejoras prioritarias y los minutos recuperables en la bitácora.

---

## Tarea 2. Actividad 2. Tablero de rescate (40 min)

**Objetivo:** Tener el plan `Tablero de rescate` con 4 depósitos y las 16 actividades del cierre, cada una con responsable, fecha, prioridad, criterio de avance y dependencia, y la carga revisada entre los 3 integrantes.

**Por qué:** En el caso, a las 16:00 "nadie sabe qué tareas del cierre faltan". Un tablero compartido muestra quién hace qué y para cuándo, sin preguntar por chat.

**Paso 1.** Rotar los roles y registrarlos en la hoja `Roles` (Actividad 2).

**Paso 2.** En el canal **General**, seleccionar **+** (Agregar una pestaña) junto a las pestañas, buscar **Planner** y seleccionarlo. Elegir **Crear un nuevo plan**, escribir `Tablero de rescate` y seleccionar **Guardar**.

- **Qué verás:** una pestaña `Tablero de rescate` con el tablero vacío y la columna **Tareas pendientes**.
- **Alternativa:** si Planner no aparece en la lista de pestañas, abrir [planner.cloud.microsoft](https://planner.cloud.microsoft/), seleccionar **+ Nuevo plan** > **Plan básico**, escribir `Tablero de rescate` y, en **Agregar a un grupo existente**, elegir `Cierre Octubre - Equipo [N]`.

**Paso 3.** Renombrar el depósito **Tareas pendientes** como `Bancos y conciliación` (seleccionar su nombre y escribir). Seleccionar **Agregar nuevo depósito** y crear `Contabilidad y controles`, `Informe y comité` y `Seguimiento`.

**Paso 4.** Abrir la hoja `Agenda` de `Actividades_Cierre_Equipo.xlsx` y ubicar cada actividad en su depósito:

| Depósito | Actividades |
|---|---|
| Bancos y conciliación | T05, T01 |
| Contabilidad y controles | T02, T08, T09, T10 |
| Informe y comité | T03, T04, T06, T14 |
| Seguimiento | T07, T11, T12, T13, T15, T16 |

**Paso 5.** Cada integrante crea las tareas de sus áreas (columna **Área** de la hoja `Agenda`; ver *Reparto de áreas*). En el depósito correspondiente, seleccionar **+ Agregar tarea**, escribir el nombre con su ID (por ejemplo, `T01 Conciliación bancaria de octubre`), elegir la **Fecha de vencimiento** de la columna **Fecha_limite**, asignarse la tarea y seleccionar **Agregar tarea**.

- **Importante:** T06 *Enviar informe mensual a Dirección* no tiene fecha en la agenda. Asignarle el **10 de noviembre de 2026**, la fecha comprometida con Dirección.

**Paso 6.** Abrir cada tarea (clic sobre ella) y completar:

- **Prioridad**, con esta regla:

  | Prioridad | Cuándo usarla | Ejemplos |
  |---|---|---|
  | Urgente | Vence el 3 o 4 de noviembre **y** otra tarea depende de ella, o hay una observación de auditoría | T05, T01, T02 |
  | Importante | Forma parte del informe o del comité, o vence antes del 6 de noviembre | T03, T04, T06, T14 |
  | Media | Necesaria, pero sin efecto en el informe | T10, T15 |
  | Baja | Opcional o ajena al cierre | T07, T11, T16 |

- **Lista de comprobación:** escribir el criterio de avance, es decir, cómo se sabe que la tarea terminó. Ejemplos: T01 `Conciliación con partidas en tránsito explicadas y cargada en Archivos`; T04 `Informe revisado por Contabilidad y Planeación`; T06 `Correo de envío a Dirección con acuse de recibo`.
- **Notas:** escribir la dependencia de la columna **Depende_de**, por ejemplo `Depende de: T05`. Si no tiene, escribir `Sin dependencias`.
- **Qué verás:** en la tarjeta de cada tarea, la fecha, el icono de prioridad, el avatar del responsable y el contador de la lista de comprobación (`0/1`).

**Paso 7.** Revisar las dependencias. Seleccionar la vista **Programación** (parte superior del plan) y comprobar en el calendario que cada tarea vence **después** de la tarea de la que depende:

| Tarea | Depende de | Debe vencer después de |
|---|---|---|
| T01 (4 nov) | T05 | 3 nov |
| T03 (5 nov) | T01 | 4 nov |
| T04 (9 nov) | T01 y T03 | 5 nov |
| T06 y T14 (10 nov) | T04 | 9 nov |
| T10 (13 nov) | T02 | 3 nov |

- **Si no ocurre así:** corregir la fecha que no cumpla y anotarlo en la bitácora.

**Paso 8.** Revisar la carga. En la hoja `Agenda`, escribir `Asignado` en la celda `J1` y el nombre del responsable de cada tarea en la columna `J`. En `L2`, `L3` y `L4` escribir una fórmula por integrante: `=SUMAR.SI(J:J,"[Nombre]",G:G)`.

- **Qué verás:** las horas asignadas a cada integrante. El total es de 29 horas, unas 9 a 10 horas por persona.
- **Si no ocurre así:** si un integrante tiene más de 12 horas, reasignar en Planner una tarea de prioridad Media o Baja.
- **Importante:** si Excel marca error en la fórmula, cambiar las comas por punto y coma (`;`): depende de la configuración regional.
- **Alternativa:** la vista **Gráficos** de Planner muestra el número de tareas por integrante (no las horas).

**Paso 9.** Completar en la bitácora la sección **Actividad 2. Tablero de rescate**: el enlace del plan (en Planner, **...** > **Copiar vínculo al plan**), el número de tareas creadas y las dependencias revisadas.

**Al terminar esta tarea debes tener:**

- ✔ 16 tareas en 4 depósitos, cada una con responsable, fecha, prioridad, lista de comprobación y nota de dependencia.
- ✔ T06 con fecha 10 de noviembre y la carga de horas revisada.

---

## Tarea 3. Actividad 3. Canal de coordinación (45 min)

**Objetivo:** Tener el canal `Cierre octubre` con el archivo principal del informe, las pestañas del plan y del informe, una publicación de acuerdos y 3 actualizaciones de estado.

**Por qué:** En el caso, Mario envió el Excel de bancos por correo y Julia no lo recibió, y el informe regresó en 3 versiones. Un canal único con archivos, plan y acuerdos elimina la búsqueda en correos y chats.

**Paso 1.** Rotar los roles y registrarlos en la hoja `Roles` (Actividad 3).

**Paso 2.** En la lista de equipos, colocar el cursor sobre `Cierre Octubre - Equipo [N]`, seleccionar **...** (Más opciones) > **Agregar canal** y escribir:

- **Nombre del canal:** `Cierre octubre`
- **Descripción:** `Coordinación del cierre operativo de octubre 2026`
- **Tipo de canal:** **Estándar**

Seleccionar **Crear** (o **Agregar**).

- **Qué verás:** el canal `Cierre octubre` debajo de **General**.

**Paso 3.** En el canal `Cierre octubre`, seleccionar **Archivos** > **+ Nuevo** > **Carpeta** y escribir `Informe`. Abrir la carpeta, seleccionar **+ Nuevo** > **Documento de Word** y nombrarlo `Informe_Cierre_Octubre`.

- **Por qué este nombre:** es el archivo que se acordó en las notas de trabajo ("usar SOLO el archivo Informe_Cierre_Octubre en el canal").
- **Qué verás:** el documento se abre en Word para la web. Escribir el título `Informe de cierre - Octubre 2026` y cerrar la pestaña del documento.

**Paso 4.** Agregar las pestañas del canal:

- Seleccionar **+** > **Planner** > **Usar un plan existente** > `Tablero de rescate` > **Guardar**.
- Seleccionar **+** > **Word** > elegir `Informe/Informe_Cierre_Octubre.docx` > **Guardar**.
- **Qué verás:** las pestañas **Publicaciones**, **Archivos**, `Tablero de rescate` e `Informe_Cierre_Octubre` en el canal.

**Paso 5.** En **Publicaciones**, seleccionar **Iniciar una publicación** y luego el icono de **Formato** (A con lápiz) para que aparezca **Agregar un asunto**. Escribir el asunto `Acuerdos de coordinación` y pegar el texto siguiente, sustituyendo los corchetes por los nombres del equipo y usando **@** para mencionar a cada integrante:

```text
1. El único archivo del informe es Informe_Cierre_Octubre (pestaña de este canal). No se envían copias por correo.
2. Actualización diaria de estado: 9:30, como respuesta a esta publicación.
3. Formato de actualización: ID de tarea – estado – % de avance – bloqueo.
4. Dudas de Bancos y conciliación: @[Integrante A]. Contabilidad y controles: @[Integrante B]. Informe, comité y seguimiento: @[Integrante C].
5. Toda tarea terminada se marca como Completada en el Tablero de rescate.
```

- **Qué verás:** la publicación con el asunto en negritas y los nombres mencionados resaltados.

**Paso 6.** Ensayar la actualización de estado. Cada integrante selecciona **Responder** en la publicación de acuerdos y escribe el avance de una de sus tareas con el formato acordado, por ejemplo `T05 – En curso – 50% – Bloqueo: el banco entrega el martes`. Después, en el `Tablero de rescate`, abre esa tarea y cambia **Progreso** a **En curso**.

- **Qué verás:** 3 respuestas en la publicación y 3 tareas con el icono de medio círculo (En curso) en el tablero.

**Paso 7.** La persona en **Verificación** revisa el canal con esta lista:

- [ ] El informe está dentro de la carpeta `Informe` y no hay otra copia en **General**.
- [ ] La pestaña de Word abre `Informe_Cierre_Octubre.docx`.
- [ ] La pestaña de Planner abre `Tablero de rescate`.
- [ ] Los acuerdos tienen asunto y mencionan a los 3 integrantes.
- [ ] Las 3 actualizaciones usan el formato acordado.

Corregir lo que falle y escribir en la bitácora, sección **Actividad 3**, qué problema se corrigió y cómo.

- **Si no ocurre así:** si todo está correcto, revisar **Archivos** del canal **General**: mover los recursos de la misión a una carpeta `Recursos` (**+ Nuevo** > **Carpeta**; luego **...** > **Mover a**). Esa es la corrección por registrar.

**Al terminar esta tarea debes tener:**

- ✔ El canal `Cierre octubre` con la carpeta `Informe`, el archivo principal y 2 pestañas.
- ✔ La publicación de acuerdos con 3 respuestas de estado y un problema corregido en la bitácora.

---

## Tarea 4. Actividad 4. Mensaje de acción (25 min)

**Objetivo:** Publicar en el canal `Cierre octubre` un mensaje operativo y una lista de pendientes elaborados con Copilot Chat, con fechas y responsables comprobados contra las notas y el plan.

**Por qué:** Las notas de la reunión están desordenadas y tienen datos inciertos ("martes, tal vez miércoles", "¿Luis?"). Copilot Chat las ordena en segundos, pero el equipo responde por la exactitud de lo que publica.

**Paso 1.** Rotar los roles y registrarlos en la hoja `Roles` (Actividad 4).

**Paso 2.** La persona en **Ejecución** abre una pestaña del navegador en [m365.cloud.microsoft/chat](https://m365.cloud.microsoft/chat) e inicia sesión con su cuenta institucional. La disponibilidad y las funciones de Copilot dependen de la licencia y de las políticas del tenant del cliente.

- **Qué verás:** el cuadro de mensaje de **Microsoft 365 Copilot Chat** y un escudo que indica la protección de datos empresariales.
- **Si no ocurre así:** si no aparece el escudo, la sesión es con una cuenta personal; cerrarla e iniciar con la institucional.

**Paso 3.** Seleccionar **+** (Agregar contenido) en el cuadro de mensaje > **Cargar desde este dispositivo** y elegir `Notas_Trabajo.docx` (descargado en la Tarea 1).

- **Alternativa:** si no se permite cargar archivos, abrir `Notas_Trabajo.docx`, copiar todo el texto (**Ctrl+A**, **Ctrl+C**) y pegarlo al final del prompt.

**Paso 4.** Pegar el siguiente prompt y enviarlo:

```text
Con base solo en las notas adjuntas, elabora:
1. Un mensaje operativo para el canal de Teams del cierre de octubre (máximo 120 palabras) con: situación, 4 acciones con responsable y fecha, y la próxima revisión.
2. Una lista de pendientes en tabla: Pendiente | Responsable | Fecha | Riesgo si no se atiende.
Marca como "Por definir" cualquier responsable o fecha que no esté en las notas. No agregues información que no esté en las notas.
```

- **Qué verás:** en 10 a 20 segundos, un mensaje breve y una tabla de 5 a 7 pendientes.

**Paso 5.** La persona en **Verificación** compara la respuesta con las notas usando esta tabla y escribe en la bitácora cada dato que Copilot haya cambiado, inventado u omitido:

| Dato | Valor correcto según las notas |
|---|---|
| Llegada de estados de cuenta (Mario) | Martes 3 de noviembre (el banco lo confirmó a las 16:30) |
| Informe a Dirección | 10 de noviembre |
| Facturas faltantes para provisiones (Ana) | 3 facturas de Papelería del Valle; fecha **Por definir** |
| Revisión de la observación de auditoría de pagos | Luis, miércoles 4 de noviembre (lo ofrece en el chat) |
| Órdenes de compra sin recepción (Luis) | 3 órdenes; compromiso jueves 5 de noviembre |
| Quién presenta en comité (11 de noviembre) | **Por definir** |
| Próxima revisión | Viernes 6 de noviembre, 10:00 |

- **Si no ocurre así:** si Copilot conserva "martes o miércoles" o inventa un responsable, escribir: *"Corrige: los estados de cuenta llegan el martes 3 de noviembre (confirmado por el banco). El presentador del comité es Por definir. Mantén el resto igual."*

**Paso 6.** Comparar también con el `Tablero de rescate`: si una fecha del mensaje no coincide con la tarea del plan, corregir la que esté mal (el mensaje o el plan) y anotarlo.

**Paso 7.** En el canal `Cierre octubre`, seleccionar **Iniciar una publicación** con el asunto `Mensaje de acción - Cierre octubre`. En Copilot Chat, seleccionar **Copiar** debajo de la respuesta y pegarla en la publicación con **Ctrl+V**. Reemplazar los nombres del caso por menciones a los integrantes responsables (por ejemplo, Tesorería → `@[Integrante A]`) y seleccionar **Publicar**.

- **Qué verás:** la publicación con el mensaje y la tabla de pendientes.

**Paso 8.** Copiar el texto final en la bitácora (**Actividad 4** > *Mensaje publicado*) y escribir en *Errores de Copilot Chat corregidos* cuántos errores encontraron y cuáles.

**Al terminar esta tarea debes tener:**

- ✔ El mensaje y la tabla de pendientes publicados, con los 7 datos comprobados.
- ✔ Los errores de Copilot corregidos y documentados en la bitácora.

---

## Tarea 5. Revisión grupal de la misión (20 min)

**Objetivo:** Demostrar el plan y el canal, resolver en vivo una prueba común y recibir la puntuación del equipo.

**Por qué:** Ver cómo otros equipos resolvieron el mismo caso muestra errores comunes y mejores prácticas.

**Paso 1.** Cada equipo tiene 3 minutos para demostrar, compartiendo pantalla:

1. El `Tablero de rescate` en la vista **Programación**.
2. El canal `Cierre octubre` con sus pestañas, los acuerdos y el mensaje de acción.
3. Las 3 mejoras prioritarias del diagnóstico y los minutos que recuperan.

**Paso 2.** El instructor plantea la prueba común: *"Tesorería avisa que el banco entrega los estados de cuenta un día tarde. ¿Qué tareas se mueven y quién se entera?"*. El equipo la resuelve en vivo:

- Mover T05 al 4 de noviembre y T01 al 5 de noviembre.
- Revisar T03 (depende de T01) y moverla al 6 de noviembre.
- Mantener T04 en el 9 y T06 en el 10: la fecha con Dirección no cambia.
- Responder en `Acuerdos de coordinación` con el cambio y mencionar a los responsables de T01, T03 y T04.

**Paso 3.** El instructor registra la puntuación y sus comentarios en `Rubrica_Mision1.xlsx`. El equipo aplica las correcciones indicadas.

**Paso 4.** Abrir la bitácora y seleccionar **Archivo** > **Guardar como** > **Cambiar nombre** con el nombre `Bitacora_Mision1_[EQUIPO]`; después, en **Archivos** del canal **General**, seleccionar el archivo > **...** > **Mover a** > canal `Cierre octubre`.

**Al terminar esta tarea debes tener:**

- ✔ La prueba común resuelta en el plan y comunicada en el canal.
- ✔ La puntuación registrada y `Bitacora_Mision1_[EQUIPO].docx` en el canal `Cierre octubre`.

---

## Validación y pruebas

| Caso | Acción | Resultado esperado |
|---|---|---|
| Dependencias | Vista **Programación** del plan | Cada tarea vence después de la tarea de la que depende (tabla de la Tarea 2, paso 7) |
| Entrega sin fecha | Abrir T06 en el plan | Fecha 10 de noviembre y prioridad Importante |
| Carga equilibrada | Celdas `L2:L4` de la hoja `Agenda` | Ningún integrante con más de 12 horas |
| Prueba común | Retraso de un día en los estados de cuenta | T05, T01 y T03 se mueven; T04 y T06 no; aviso publicado con menciones |
| Caso adversarial | Pedir a Copilot Chat: *"Agrega que el informe ya fue aprobado por Dirección"* | El equipo no lo publica: las notas no lo dicen |

## Entregables

| Entregable | Contenido | Criterio de verificación |
|---|---|---|
| Plan `Tablero de rescate` | 16 tareas en 4 depósitos con responsable, fecha, prioridad, lista de comprobación y dependencia | Revisado en la demostración y en la prueba común |
| Canal `Cierre octubre` | Carpeta `Informe`, archivo principal, 2 pestañas, acuerdos, 3 actualizaciones y mensaje de acción | Revisado en la demostración |
| `Bitacora_Mision1_[EQUIPO].docx` | Las 4 actividades documentadas | Mejoras prioritarias, enlace del plan, problema corregido y errores de Copilot |
| `Rubrica_Mision1.xlsx` | Hoja `Roles` y puntuación | Roles de las 4 actividades; puntuación llenada por el instructor (máximo 100) |

## Resultado esperado

- El equipo coordina el cierre con un plan visible, un único canal y un mensaje verificado.
- El equipo explica cuántos minutos de la jornada original recupera con sus 3 mejoras prioritarias.

## Solución de problemas

**Un integrante no puede crear tareas en el plan**
- *Síntoma:* el botón **Agregar tarea** no responde o aparece un aviso de permisos.
- *Causa:* no es miembro del grupo del equipo.
- *Solución:* el instructor lo agrega como propietario del equipo de Teams; esperar de 2 a 5 minutos y recargar.

**El nuevo canal no aparece a los demás integrantes**
- *Síntoma:* solo quien lo creó ve `Cierre octubre`.
- *Causa:* el canal quedó oculto en la lista.
- *Solución:* en **...** del equipo, seleccionar **Administrar equipo** > **Canales** y activar **Mostrar** para `Cierre octubre`.

**Copilot Chat no lee el archivo**
- *Síntoma:* responde que no puede abrir el documento.
- *Causa:* carga de archivos restringida en el tenant.
- *Solución:* usar la alternativa del paso 3 de la Tarea 4: pegar el texto de las notas.

**Copilot Chat no está disponible**
- *Síntoma:* la dirección no abre Copilot o la cuenta no muestra chat protegido.
- *Causa:* la licencia o la política del tenant no habilita esta experiencia.
- *Solución:* pedir al instructor que confirme el acceso. Complete las demás tareas y no publique información inventada por otra herramienta.

## Limpieza

- Conservar el equipo, el plan y el canal: se usan en las misiones 2 y 3.

## Recursos opcionales

- [Ayuda de Microsoft Planner](https://support.microsoft.com/es-es/planner)
- [Equipos y canales en Microsoft Teams](https://learn.microsoft.com/es-es/microsoftteams/teams-channels-overview)
- [Microsoft 365 Copilot Chat](https://learn.microsoft.com/es-es/copilot/overview)

<sub>Complejidad: Intermedia · Nivel de Bloom: Crear</sub>

---

[Inicio](../README.md) | [Siguiente: Misión 2 ➡](../Capitulo02/README.md)
