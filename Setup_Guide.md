<img src="images/neteclogo.png" alt="logo" width="300"/>

# Setup Guide General

## Talleres Aplicados de Productividad Digital con Microsoft 365 - Misiones colaborativas

| Control documental | Información |
|---|---|
| Clave del curso | TPRACT_PROD_DIG_M365 (Priv) |
| Versión del documento | 1.0 |
| Estado | BORRADOR: revisión documental completa; pendiente de validación en el tenant del cliente |
| Instructor responsable | Por asignar por Netec |
| Fecha de elaboración | 2026-11-13 |
| Fecha de última validación | 2026-11-13 (revisión de enlaces y documentación) |
| Repositorio de laboratorios | Repositorio de GitHub de Netec del taller (rama `main`) |
| Rama y revisión analizada | `main`, versión 1.0 |
| Alcance revisado | 3 misiones, 14 archivos de recursos, README principal y Setup Guide |
| Modalidad del entorno | Web (Microsoft 365 institucional del cliente), trabajo en equipos de 3 |

[Inicio](README.md)

# Objetivo

Dejar preparado, antes del taller, un espacio de trabajo por equipo en Microsoft 365: un equipo de Teams con sus 3 integrantes, su sitio de SharePoint con la lista `Registro de solicitudes` y un flujo base de Power Automate compartido, además de los archivos del caso. Así, los 480 minutos del taller se dedican a las misiones y no a configuración. El entorno se considera listo cuando se aprueban las validaciones de la sección [Validación del Entorno](#validacion-entorno) con la cuenta de un participante.

# Requisitos de Hardware

| Recurso | Mínimo requerido | Recomendado | Observaciones |
|---|---|---|---|
| Equipo | PC o laptop de 64 bits, 2 núcleos | 4 núcleos | Todas las aplicaciones se usan en la web o en escritorio |
| Memoria RAM | 8 GB | 16 GB | Teams, el navegador y Excel abiertos a la vez |
| Pantalla | 1366 × 768 | 1920 × 1080 o dos monitores | Facilita trabajar en equipo y seguir la sesión |
| Conectividad | 10 Mbps | 25 Mbps | Videoconferencia y aplicaciones en la nube al mismo tiempo |
| Audio | Audífonos con micrófono | — | Coordinación del equipo en llamadas o salas |

# Sistemas Operativos Compatibles

| Sistema operativo | Edición y versión | Arquitectura | Condición de soporte o validación |
|---|---|---|---|
| Windows | 10 u 11 | x64 | Plataforma base; compatible según fabricante; pendiente de validar en el tenant del cliente |
| macOS | 13 o posterior | Apple silicon o Intel | Compatible según fabricante; no validado |

# Software Requerido

| Componente | Edición y versión requerida | Arquitectura | Obligatorio u opcional | Fuente oficial |
|---|---|---|---|---|
| Navegador Microsoft Edge o Google Chrome | Versión estable vigente | x64 | Obligatorio | [microsoft.com/edge](https://www.microsoft.com/edge) |
| Microsoft Teams | Servicio administrado (escritorio o web) | x64 | Obligatorio (misiones 1 a 3) | [teams.microsoft.com](https://teams.microsoft.com/) |
| Microsoft Planner | Servicio administrado | N/A | Obligatorio (Misión 1) | [planner.cloud.microsoft](https://planner.cloud.microsoft/) |
| SharePoint | Servicio administrado | N/A | Obligatorio (misiones 2 y 3) | [m365.cloud.microsoft](https://m365.cloud.microsoft/) |
| Microsoft Forms | Servicio administrado | N/A | Obligatorio (misiones 2 y 3) | [forms.office.com](https://forms.office.com/) |
| Excel y Word | Microsoft 365 (escritorio o web) | x64 | Obligatorio | [m365.cloud.microsoft](https://m365.cloud.microsoft/) |
| Power Automate | Servicio administrado, conectores estándar incluidos en Microsoft 365 | N/A | Obligatorio (Misión 3) | [make.powerautomate.com](https://make.powerautomate.com/) |
| Microsoft 365 Copilot Chat (Copilot Chat básico) | Servicio administrado con protección de datos empresariales | N/A | Obligatorio (Misión 1) | [m365.cloud.microsoft/chat](https://m365.cloud.microsoft/chat) |
| Power BI | Solo como referencia de uso posterior de los datos | N/A | Opcional | No se usa en las misiones |

Las capacidades disponibles dependen de las licencias y políticas del tenant. Registrar en el [Registro de validación](#registro-validacion) la fecha, la edición visible y cualquier restricción.

# Herramientas y Dependencias

## Paquetes, frameworks y componentes adicionales

| Dependencia | Versión o restricción | Componente que la necesita | Método de instalación o habilitación |
|---|---|---|---|
| Conectores estándar: Microsoft Forms, SharePoint, Office 365 Outlook y Microsoft Teams | Incluidos en Microsoft 365 | Misión 3 | Disponibles en Power Automate; deben estar permitidos por la directiva de datos (DLP) del tenant |
| Carga de archivos en Copilot Chat | Según la política del tenant | Misión 1 | Botón **+** del cuadro de mensaje; alternativa: pegar el contenido |
| Archivos de las misiones | Versión 1.0 del repositorio | Misiones 1 a 3 | Carpetas `CapituloNN/recursos/` |

## Licencias, cuentas y permisos

| Recurso o servicio | Licencia o suscripción | Cuenta o rol requerido | Permiso mínimo | Responsable de habilitación |
|---|---|---|---|---|
| Microsoft 365 | Licencia del cliente con Teams, SharePoint, Forms y Planner | Cuenta institucional | Usuario | TI del cliente |
| Equipo de Teams por equipo de trabajo | Incluida (grupo de Microsoft 365) | Instructor o TI | Crear equipos; los 3 integrantes como **propietarios** | Instructor o TI del cliente |
| SharePoint del equipo | Incluida | Propietario del equipo | Crear bibliotecas, listas y columnas | Automático al crear el equipo |
| Power Automate | Incluido en Microsoft 365 (conectores estándar) | Cuenta institucional | Crear flujos de nube y ser copropietario | TI del cliente |
| Copilot Chat básico | Incluido para cuentas con Entra ID | Cuenta institucional | Usuario | TI del cliente |

Los accesos se entregan por el canal institucional del cliente. No registrar contraseñas ni códigos de verificación en el repositorio ni en los entregables.

# Instalación y Configuración

## 1. Obtener los materiales

- Repositorio autorizado: repositorio de GitHub del taller (botón **Code > Download ZIP**) o paquete ZIP del instructor.
- Revisión: rama `main`.
- Directorio de trabajo: **Archivos** del canal de cada equipo de Teams.

## 2. Instalar o habilitar los componentes

### Equipos de trabajo en Teams (instructor, antes del taller)

1. Formar los equipos de 3 integrantes (si el grupo no es múltiplo de 3, formar equipos de 2 o 4; en equipos de 2, una persona combina Ejecución y Verificación).
2. En Teams, **Equipos > + > Crear equipo** > **Desde cero** > **Privado**, con el nombre `Cierre Octubre - Equipo [N]`.
3. Agregar a los 3 integrantes y asignarles el rol de **Propietario**.

**Resultado esperado:** cada equipo tiene su espacio de Teams y su sitio de SharePoint, y todos sus integrantes son propietarios.

### Lista `Registro de solicitudes` (instructor, una por equipo)

1. En cada equipo, **...** > **Abrir en SharePoint** > **Nuevo** > **Lista** > **Lista en blanco** `Registro de solicitudes`.
2. Crear las columnas según [Especificacion_Flujo_Base.docx](Capitulo03/recursos/Especificacion_Flujo_Base.docx): `Title` renombrada a `Beneficiario`, `Tipo` (Elección: Pago a proveedor, Reembolso de gastos, Viáticos, Anticipo), `Factura` (Texto), `Monto_MXN` (Número, 2 decimales), `Fecha_requerida` (Fecha), `Area` (Elección: Tesorería, Contabilidad, Planeación, Compras, Coordinación) y `Estado` (Elección: Recibida, En revisión, Pagada; valor predeterminado Recibida).
3. Las opciones de `Tipo` y `Area` deben escribirse igual que en el formulario de la Misión 2; si difieren, **Crear elemento** falla.

**Resultado esperado:** la lista existe en el sitio de cada equipo con 7 columnas.

### Formulario y flujo base (instructor)

1. En [forms.office.com](https://forms.office.com/), crear el formulario `Solicitudes del cierre` con las mismas preguntas obligatorias que los equipos crean en la Misión 2: `Tipo`, `Beneficiario`, `Factura`, `Monto MXN` (Texto con restricción **Número**), `Fecha requerida` y `Área`.
2. En [make.powerautomate.com](https://make.powerautomate.com/), **+ Crear > Flujo de nube automatizado** con el nombre `Registro de solicitudes del cierre` y el desencadenador **Cuando se envía una respuesta nueva** (Microsoft Forms) sobre ese formulario.
3. Agregar **Obtener los detalles de la respuesta** (Id. de respuesta: contenido dinámico **Id. de respuesta**).
4. Agregar **Crear elemento** (SharePoint) sobre la lista `Registro de solicitudes` de un equipo y asignar cada columna con el contenido dinámico de la respuesta.
5. Guardar, enviar una respuesta de prueba y confirmar en el **Historial de ejecuciones** que se creó el elemento.
6. En la página del flujo, **Editar** en **Propietarios** y agregar a los integrantes de cada equipo (o al grupo de Microsoft 365 del equipo) como **copropietarios**.

**Resultado esperado:** el flujo base se ejecuta correctamente y aparece en **Mis flujos > Compartido conmigo** para todos los participantes. En la Misión 3 cada equipo guarda una copia y la apunta a su formulario y a su lista.

> **Monto como texto:** Forms entrega todas las respuestas como texto. En la Misión 3 los equipos provocan y corrigen ese error con la expresión `float()` aplicada al contenido dinámico **Monto MXN** (Tarea 3, pasos 4 y 5). Antes del taller, el instructor debe hacer ese ejercicio en su copia para conocer el mensaje de error que verá su tenant.

### Copilot Chat

1. Con una cuenta de participante, abrir [Copilot Chat](https://m365.cloud.microsoft/chat) y confirmar que muestra la protección de datos empresariales.

**Resultado esperado:** Copilot Chat responde con la cuenta institucional.

## 3. Preparar archivos de configuración

No se requieren archivos de configuración. El instructor puede cargar previamente los archivos de `recursos/` en **Archivos** del canal **General** de cada equipo para ahorrar tiempo de descarga.

# Variables de Entorno

No se requieren variables de entorno.

# Configuración Base para los Laboratorios

## Parámetros comunes

| Parámetro | Valor o convención | Observaciones |
|---|---|---|
| Equipo de Teams | `Cierre Octubre - Equipo [N]` (privado) | Uno por equipo; creado por el instructor |
| Canal de trabajo | `Cierre octubre` | Lo crea el equipo en la Misión 1 |
| Plan de Planner | `Tablero de rescate` | Misión 1 |
| Biblioteca | `Expediente Cierre` | Misión 2, en el sitio del equipo |
| Formulario del equipo | `Solicitudes del cierre - Equipo [N]` | Misión 2; se usa en la Misión 3 |
| Lista | `Registro de solicitudes` | Preparada por el instructor; Misión 3 |
| Flujo | `Registro de solicitudes del cierre - Equipo [N]` | Copia del flujo base; Misión 3 |
| Nombres de entregables | `Nombre_[EQUIPO].ext` | Sin espacios ni acentos |

## Estructura de carpetas

```text
Teams: Cierre Octubre - Equipo [N]
├── General\Archivos\        Recursos de las misiones
└── Cierre octubre\Archivos\ Bitácoras, tablas y evidencias del equipo
```

## Recursos compartidos

| Recurso | Nombre o identificador | Estructura o configuración base | Responsable de creación |
|---|---|---|---|
| Formulario base | `Solicitudes del cierre` | 6 preguntas obligatorias | Instructor |
| Flujo base | `Registro de solicitudes del cierre` | Forms > Obtener detalles > Crear elemento | Instructor |

## Preparación antes de cada práctica

| Misión | Preparación |
|---|---|
| 1 | Equipos de Teams creados con sus integrantes; Planner y Copilot Chat disponibles |
| 2 | Sitio de SharePoint de cada equipo accesible; Forms disponible |
| 3 | Lista `Registro de solicitudes` en cada sitio; flujo base compartido; ejercicio de `float()` probado por el instructor |

## Correcciones de coherencia

| Inconsistencia o dependencia omitida | Configuración unificada | Ajuste necesario en las copias de trabajo |
|---|---|---|
| El temario indica que el instructor prepara los espacios y el flujo base | Esta guía define el equipo, la lista, el formulario y el flujo base por preparar | Ninguno |
| La creación de equipos puede estar restringida en el tenant | El instructor o TI crea los equipos antes del taller | Confirmar con TI del cliente |
| El temario menciona Power BI como uso posterior | La Misión 2 deja los datos en una tabla lista para Power BI; Power BI no se usa | Ninguno |

# Servicios Externos Requeridos

| Servicio | URL, endpoint o región | Uso | Acceso requerido |
|---|---|---|---|
| Microsoft 365 | [m365.cloud.microsoft](https://m365.cloud.microsoft/) | Todas las misiones | Cuenta institucional |
| Power Automate | [make.powerautomate.com](https://make.powerautomate.com/) | Misión 3 | Cuenta institucional |
| GitHub | [github.com](https://github.com/) | Descarga de materiales | Lectura del repositorio |

## Configuración de red

| Origen | Destino | Protocolo y puerto | Sentido | Condición |
|---|---|---|---|---|
| Equipo del participante | Puntos de conexión de Microsoft 365 y github.com | HTTPS 443 | Saliente | Según la [lista oficial de URL y direcciones IP de Microsoft 365](https://learn.microsoft.com/es-es/microsoft-365/enterprise/urls-and-ip-address-ranges) |

# Creación de Entornos / Máquinas Virtuales / Emuladores

No aplica. El taller se realiza en el tenant de Microsoft 365 del cliente.

<a id="validacion-entorno"></a>

# Validación del Entorno

| ID | Componente o capacidad | Procedimiento | Resultado esperado | Evidencia mínima |
|---|---|---|---|---|
| V-01 | Cuenta | Iniciar sesión en m365.cloud.microsoft con una cuenta de participante | Aparecen las aplicaciones del taller | Captura |
| V-02 | Equipo de Teams | Abrir `Cierre Octubre - Equipo [N]` y agregar un canal | El canal se crea | Captura |
| V-03 | Planner | Agregar una pestaña de Planner con un plan nuevo | Plan creado | Captura |
| V-04 | SharePoint | En el sitio del equipo, crear una biblioteca con una columna de elección | Biblioteca con la columna | Captura |
| V-05 | Forms | Crear un formulario con una pregunta obligatoria | Formulario creado | Captura |
| V-06 | Flujo base | Abrir el flujo desde **Compartido conmigo**, **Guardar como** y probar con una respuesta | Elemento creado en la lista | Historial de ejecuciones |
| V-07 | Copilot Chat | Adjuntar `Notas_Trabajo.docx` y pedir un resumen | Responde con protección de datos empresariales | Captura |

**Criterio de entorno listo:** V-01 a V-07 aprobadas con una cuenta de participante de al menos un equipo.

# Comandos de Verificación

No aplica. El taller se valida en las interfaces web de Microsoft 365 con los procedimientos V-01 a V-07.

# Troubleshooting

| Síntoma | Causa probable | Comprobación | Corrección | Validación posterior |
|---|---|---|---|---|
| Un integrante no ve el equipo | No fue agregado o la sincronización tarda | Miembros del equipo | Agregarlo como propietario y esperar unos minutos | V-02 |
| El flujo no aparece en Compartido conmigo | No es copropietario | Propietarios del flujo | Agregar al integrante o al grupo del equipo | V-06 |
| La copia del flujo pide reparar conexiones | Las conexiones son del instructor | Mensaje del diseñador | Cada equipo agrega sus propias conexiones | V-06 |
| Power Automate marca un conector como Premium o bloqueado | Licencia o directiva de datos | Mensaje del diseñador | Usar solo Forms, SharePoint, Outlook y Teams; solicitar a TI ajustar la directiva | V-06 |
| Copilot Chat aparece sin protección de datos empresariales | Sesión con cuenta personal | Cuenta en la esquina superior | Iniciar sesión con la cuenta institucional | V-07 |

# Checklist Final

- [ ] Equipos de Teams creados con los integrantes como propietarios.
- [ ] Lista `Registro de solicitudes` en el sitio de cada equipo.
- [ ] Formulario base y flujo base probados y compartidos.
- [ ] Condición con `float()` probada por el instructor en su copia del flujo.
- [ ] Copilot Chat con protección de datos empresariales.
- [ ] Validaciones V-01 a V-07 aprobadas.

# Resumen

Antes del taller, el instructor crea un equipo de Teams por equipo de trabajo, la lista `Registro de solicitudes` en cada sitio y un flujo base compartido. Los participantes solo necesitan una cuenta institucional de Microsoft 365 con Teams, Planner, SharePoint, Forms, Excel, Power Automate con conectores estándar y Copilot Chat básico. No se instala software adicional.

<a id="registro-validacion"></a>

## Registro de validación

| Fecha | Responsable | Plataforma o entorno probado | Resultado | Limitaciones o acciones pendientes |
|---|---|---|---|---|
| 2026-11-13 | Desarrollo de contenido Netec | Revisión documental, enlaces y coherencia con el temario | APTO para publicación del repositorio | No se validó en el tenant del cliente. Pendiente: V-01 a V-07 con una cuenta de participante |

## Referencias oficiales

| Documento o recurso | URL | Fecha de consulta |
|---|---|---|
| Microsoft 365 Copilot Chat | https://learn.microsoft.com/es-es/copilot/overview | 2026-11-13 |
| Equipos y canales de Teams | https://learn.microsoft.com/es-es/microsoftteams/teams-channels-overview | 2026-11-13 |
| Ayuda de Planner | https://support.microsoft.com/es-es/planner | 2026-11-13 |
| Control de versiones en SharePoint | https://support.microsoft.com/es-es/office/habilitar-y-configurar-el-control-de-versiones-de-una-lista-o-biblioteca-1555d642-23ee-446a-990a-bcab618c7a37 | 2026-11-13 |
| Power Automate con Forms | https://learn.microsoft.com/es-es/power-automate/forms/overview | 2026-11-13 |
| Conectores estándar | https://learn.microsoft.com/es-es/connectors/connector-reference/connector-reference-standard-connectors | 2026-11-13 |

[Inicio](README.md)
