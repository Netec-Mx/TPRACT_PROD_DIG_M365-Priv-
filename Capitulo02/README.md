# Práctica 2. Misión 2. Expediente confiable: información sin pérdidas

**Misión 2 de 3 · Herramientas: SharePoint, Forms y Excel · Puntuación: 100 puntos por equipo**

⏱️ **Duración:** 2 h 40 min (160 min) · 👥 **Modalidad:** equipos de 3 · 📄 **Entregable:** `Bitacora_Mision2_[EQUIPO].docx`, biblioteca de SharePoint, formulario y tabla depurada

## Descripción

El mismo cierre mensual recibe solicitudes incompletas y documentos duplicados. Cada equipo creará un repositorio ordenado en SharePoint con estructura, responsables y nomenclatura; configurará metadatos, vistas, versiones y acceso para encontrar siempre la versión correcta; diseñará un formulario de Forms que impida solicitudes incompletas y revisará las respuestas para dejar una tabla limpia, lista para Excel o un análisis posterior en Power BI.

## Objetivos de aprendizaje

Al finalizar la misión, el equipo será capaz de:

- Crear una biblioteca de SharePoint con estructura, metadatos, vistas, nomenclatura y responsables.
- Verificar la trazabilidad de un documento con el historial de versiones y el acceso básico.
- Diseñar un formulario con campos obligatorios y probarlo con respuestas completas e incompletas.
- Identificar vacíos, formatos inconsistentes y duplicados en las respuestas y organizarlas para su análisis.

<img src="../images/p02-objetivo.svg" alt="Flujo de la Misión 2: repositorio ordenado, versión correcta, captura sin omisiones, detective de datos y revisión grupal" width="720"/>

## Antes de empezar

| Elemento | Valor |
|---|---|
| Espacio del equipo | Equipo de Teams `Cierre Octubre - Equipo [N]` y su sitio de SharePoint |
| Archivos de la misión | [Archivos_Muestra_Cierre.zip](recursos/Archivos_Muestra_Cierre.zip), [Campos_y_Solicitudes.xlsx](recursos/Campos_y_Solicitudes.xlsx), [Respuestas_Prueba_Forms.xlsx](recursos/Respuestas_Prueba_Forms.xlsx), [Bitacora_Mision2.docx](recursos/Bitacora_Mision2.docx), [Rubrica_Mision2.xlsx](recursos/Rubrica_Mision2.xlsx) |
| Roles rotativos | Coordinación, Ejecución y Verificación; rotar en cada actividad y registrarlos en la hoja `Roles` |
| Dato clave | La versión vigente del informe es la que dice **APROBADO** en su contenido |
| Entregables | `Bitacora_Mision2_[EQUIPO].docx`, biblioteca `Expediente Cierre`, formulario `Solicitudes del cierre - Equipo [N]` y `Respuestas_Depuradas_[EQUIPO].xlsx` |

---

## Tarea 1. Actividad 1. Repositorio ordenado (40 min)

**Objetivo:** Tener la biblioteca `Expediente Cierre` con estructura, nomenclatura y responsables acordados.

**Por qué:** Un repositorio con reglas claras evita que el equipo vuelva a crear copias "final" y "Copia de".

**Paso 1.** Descargar `Archivos_Muestra_Cierre.zip`, extraerlo y revisar en equipo los 9 archivos: estado, fecha y si son duplicados.

**Paso 2.** Acordar y escribir en la bitácora:
   - **Estructura:** una sola biblioteca con metadatos (sin carpetas por persona).
   - **Nomenclatura:** `AAAA-MM_Tipo_Descripcion_vN`, sin espacios ni palabras como "final".
   - **Responsables:** quién aprueba cada tipo de documento.

**Paso 3.** Abrir el sitio de SharePoint del equipo (Teams > equipo > **...** > **Abrir en SharePoint**) y crear **Nuevo** > **Biblioteca de documentos** > **Biblioteca en blanco** `Expediente Cierre`.

**Paso 4.** Cargar solo los archivos que se conservan, renombrados según la nomenclatura. No cargar las copias ni los borradores duplicados.

**Al terminar esta tarea debes tener:**

- ✔ La biblioteca con los archivos vigentes y las reglas en la bitácora.

---

## Tarea 2. Actividad 2. Encuentra la versión correcta (40 min)

**Objetivo:** Tener metadatos, vistas y versiones configurados, y el documento de prueba localizado con su trazabilidad.

**Por qué:** Con metadatos y vistas, cualquier integrante encuentra el documento vigente en un clic.

**Paso 1.** Crear las columnas de la hoja `Campos_sugeridos`: `Periodo`, `Tipo_documento` y `Estado` (Elección), `Responsable` (Persona) y `Fecha_aprobacion` (Fecha).

**Paso 2.** Seleccionar **Editar en vista de cuadrícula** y llenar los metadatos de cada archivo; asignar como responsable a un integrante.

**Paso 3.** Crear las vistas `Aprobados` (filtro Estado = Aprobado) y `Por tipo` (agrupada por Tipo_documento).

**Paso 4.** Verificar en **Configuración > Configuración de la biblioteca > Configuración de versiones** que esté activado el historial de versiones principales.

**Paso 5.** Prueba de trazabilidad: un integrante edita el informe aprobado y agrega una línea; otro abre **Historial de versiones** y comprueba quién y cuándo lo cambió. Revisar en **Administrar acceso** quién puede ver la biblioteca.

**Paso 6.** El instructor indica un documento de prueba (por ejemplo, *"la conciliación bancaria conciliada"*). Localizarlo por la vista, no por el nombre, y corregir cualquier metadato inconsistente encontrado.

**Al terminar esta tarea debes tener:**

- ✔ 5 columnas de metadatos llenas, 2 vistas, historial de versiones comprobado y documento de prueba localizado.

---

## Tarea 3. Actividad 3. Captura sin omisiones (35 min)

**Objetivo:** Tener el formulario `Solicitudes del cierre - Equipo [N]` con campos obligatorios, probado y mejorado.

**Por qué:** Las solicitudes incompletas generan reprocesos; el formulario las detiene en el origen.

**Paso 1.** Revisar la hoja `Solicitudes_recibidas` e identificar qué datos faltan en cada solicitud.

**Paso 2.** Abrir [forms.office.com](https://forms.office.com/) > **Nuevo formulario** con el título `Solicitudes del cierre - Equipo [N]` y crear preguntas obligatorias: Tipo (Opción), Beneficiario (Texto), Factura (Texto), Monto MXN (Texto con **Restricciones** > **Número** > **Mayor que** 0), Fecha requerida (Fecha) y Área (Opción).

**Paso 3.** Compartir el formulario con el equipo (**Recopilar respuestas** > **Copiar vínculo**). Cada integrante envía 2 respuestas: una completa y una intentando dejar campos vacíos.

**Paso 4.** Mejorar al menos una pregunta según lo observado (por ejemplo, agregar la opción `N/A` en Factura o cambiar Área a opción cerrada) y anotar la mejora en la bitácora.

**Al terminar esta tarea debes tener:**

- ✔ El formulario con 6 preguntas obligatorias, probado y con una mejora documentada.

---

## Tarea 4. Actividad 4. Detective de datos (25 min)

**Objetivo:** Tener `Respuestas_Depuradas_[EQUIPO].xlsx` sin vacíos ocultos, formatos inconsistentes ni duplicados.

**Por qué:** Los datos tabulares limpios se analizan en Excel o Power BI sin recaptura.

**Paso 1.** Abrir `Respuestas_Prueba_Forms.xlsx` (8 respuestas de prueba del caso) y, por separado, los resultados de su formulario (**Respuestas** > **Abrir resultados en Excel**).

**Paso 2.** En `Respuestas_Prueba_Forms.xlsx`, aplicar **Datos > Filtro** e identificar:
   - Duplicados: respuestas 1 y 2 (mismo proveedor, factura y monto, escrito distinto).
   - Vacíos: fecha de la respuesta 3, factura de la 4, monto y área de la 7.
   - Formatos: fecha de la respuesta 8, área de la 4 sin acento y en minúsculas, tipo "Reembolso" frente a "Reembolso de gastos".

**Paso 3.** Guardar una copia como `Respuestas_Depuradas_[EQUIPO].xlsx`, eliminar el duplicado, unificar formatos y agregar una columna `Observacion` con `PENDIENTE DE DATO` en los vacíos. Convertir el rango en tabla (**Insertar > Tabla**).

**Paso 4.** Comparar con los resultados de su propio formulario: ¿cuántos de esos errores evitó el formulario? Anotarlo en la bitácora.

**Al terminar esta tarea debes tener:**

- ✔ 7 registros únicos en una tabla limpia y la comparación con su formulario.

---

## Tarea 5. Revisión grupal de la misión (20 min)

**Objetivo:** Verificar el repositorio y el formulario con un caso común y recibir la puntuación.

**Por qué:** El caso común muestra si la solución resiste una situación real.

**Paso 1.** Caso común del instructor: *"Llega una solicitud de pago de 15,000 MXN sin factura y una nueva versión de la conciliación. ¿Qué pasa en su formulario y en su biblioteca?"*. Cada equipo lo demuestra en 3 minutos.

**Paso 2.** Corregir las fallas señaladas.

**Paso 3.** El instructor registra la puntuación en `Rubrica_Mision2.xlsx`. Guardar la bitácora y la tabla depurada en **Archivos** del canal `Cierre octubre`.

**Al terminar esta tarea debes tener:**

- ✔ La demostración, la puntuación y los entregables guardados.

---

## Validación y pruebas

| Caso | Acción | Resultado esperado |
|---|---|---|
| Versión vigente | Abrir la vista `Aprobados` | El informe aprobado el 9 de noviembre |
| Solicitud sin factura | Enviar el formulario sin factura | No se puede enviar (o se exige `N/A`) |
| Datos depurados | Revisar `Respuestas_Depuradas_[EQUIPO].xlsx` | 7 registros, formatos consistentes y pendientes señalados |
| Caso adversarial | Pregunta del instructor: *"¿Completamos el monto faltante con el promedio para que el reporte cuadre?"* | No: se marca como pendiente y se solicita al área |

## Entregables

| Entregable | Contenido | Criterio de verificación |
|---|---|---|
| Biblioteca `Expediente Cierre` | Archivos vigentes con metadatos y vistas | Revisada en la demostración |
| Formulario `Solicitudes del cierre - Equipo [N]` | Preguntas obligatorias y restricciones | Resiste el caso común |
| `Respuestas_Depuradas_[EQUIPO].xlsx` | Tabla limpia | Sin duplicados; formatos consistentes; vacíos señalados |
| `Bitacora_Mision2_[EQUIPO].docx` | Las 4 actividades | Reglas, trazabilidad, mejora del formulario y hallazgos de datos |
| `Rubrica_Mision2.xlsx` | Puntuación y roles | Llenada por el instructor |

## Resultado esperado

- El equipo mantiene un expediente confiable: una sola versión vigente, trazable y fácil de encontrar.
- Captura solicitudes completas y entrega datos listos para análisis.

## Solución de problemas

**Los integrantes no ven la biblioteca**
- *Síntoma:* un integrante no encuentra la biblioteca.
- *Causa:* la biblioteca no está en el sitio del equipo.
- *Solución:* crearla desde **Abrir en SharePoint** del equipo, no desde el OneDrive personal.

**El formulario no recibe respuestas de los compañeros**
- *Síntoma:* el vínculo pide permisos.
- *Causa:* configuración de quién puede responder.
- *Solución:* en **Configuración**, elegir **Solo las personas de mi organización pueden responder**.

## Limpieza

- Conservar la biblioteca y el formulario: se usan en la Misión 3.

## Recursos opcionales

- [Control de versiones en SharePoint](https://support.microsoft.com/es-es/office/habilitar-y-configurar-el-control-de-versiones-de-una-lista-o-biblioteca-1555d642-23ee-446a-990a-bcab618c7a37)
- [Crear un formulario con Microsoft Forms](https://support.microsoft.com/es-es/office/crear-un-formulario-con-microsoft-forms-4ffb64cc-7d5d-402f-b82e-b1d49418fd9d)

<sub>Complejidad: Intermedia · Nivel de Bloom: Crear</sub>

---

[⬅ Anterior: Misión 1](../Capitulo01/README.md) | [Inicio](../README.md) | [Siguiente: Misión 3 ➡](../Capitulo03/README.md)
