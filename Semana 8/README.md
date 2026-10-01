# Sistema de Gestión de Pagos de Gastos Comunes — Edificio Nuevos Horizontes

Proyecto de la asignatura Ingeniería de Software II (Duoc UC), desarrollado en dupla. Documenta el análisis, diseño de arquitectura y prototipado de un sistema para automatizar el cobro de gastos comunes, reducir la morosidad y entregar mayor transparencia a la administración y los residentes del edificio.

## Estructura del repositorio

```
/Documentacion
  Acta de cierre del proyecto_Grupo1.docx
  Documento de Arquitectura de Software (DAS)_Grupo1.docx
  Informe de lecciones aprendidas_Grupo1.docx

/Prototipos
  /Alta fidelidad
  /Anexo Prototipo Alta Fidelidad
  /Baja fidelidad
  link_figma.txt

/Diagramas
  Diagrama_Arquitectura.drawio
```

## Contenido

### 📄 Documentacion

- **Documento de Arquitectura de Software (DAS)_Grupo1** — Requisitos funcionales y no funcionales, las cinco vistas del modelo 4+1, decisiones arquitectónicas, patrones y estilo, prototipos de interfaz y el Anexo A con la especificación completa de los 35 casos de uso.
- **Informe de lecciones aprendidas_Grupo1** — Reflexión sobre el proceso de desarrollo: aspectos positivos, desafíos enfrentados y mejoras identificadas para una futura iteración del proyecto.
- **Acta de cierre del proyecto_Grupo1** — Descripción y alcance del proyecto, criterios de término, estado de entregables y aprobaciones.

### 🎨 Prototipos

Prototipo de baja y alta fidelidad, con dos roles de usuario sobre una pantalla de inicio de sesión compartida:

- **Login** — pantalla compartida por ambos roles (1 pantalla en común).
- **Flujo Administrador** (5 pantallas) — Registro de Residentes, Departamentos y Residentes, Gestión de Gastos Comunes, Notificaciones, Crear Notificación.
- **Flujo Residente** (7 pantallas) — Mis Gastos Comunes, Detalle del Gasto Común (pendiente y pagado), Confirmación de Pago, Notificaciones, Perfil.
- **6 pantallas complementarias con mensajes de confirmación** — distribuidas entre ambos flujos, ante acciones críticas del usuario (por ejemplo, registro de un residente o descarga de un comprobante).

En alta fidelidad, la navegación de ambos flujos quedó conectada de forma interactiva mediante el modo Prototype de Figma, enlazando cada pantalla con la siguiente a través de sus botones y elementos de acción, de modo que el prototipo permite simular la experiencia real de navegación mediante clics, y no solo presentar imágenes estáticas.

Carpetas:

- **/Alta fidelidad** — capturas del prototipo de alta fidelidad de ambos roles, incluyendo las pantallas complementarias de confirmación.
- **/Baja fidelidad** — capturas del wireframe inicial de baja fidelidad.
- **/Anexo Prototipo Alta Fidelidad** — composiciones de referencia generadas con IA, utilizadas como apoyo visual para algunas vistas del prototipo que no corresponden a diagramas estructurales del DAS, orientando el sistema visual de alta fidelidad (paleta de colores, tipografía, iconografía y disposición de las pantallas) antes de recrear cada una manualmente en Figma. No forman parte del prototipo entregable, se incluyen como material de apoyo del proceso de diseño.
- **link_figma.txt** — enlace al archivo editable en Figma, con el prototipo interactivo.

### 🗺️ Diagramas

- **Diagrama_Arquitectura.drawio** — Archivo con las cinco vistas del modelo 4+1: diagrama de contexto, casos de uso (nivel 1 y nivel 2), diagrama de clases, diagrama de actividad, diagrama de componentes, diagrama de paquetes y diagrama de despliegue.

## Tecnologías y herramientas utilizadas

- **Arquitectura:** AWS serverless (API Gateway, Lambda, DynamoDB, Cognito, S3, CloudFront, Route 53, SES, EventBridge Scheduler).
- **Backend:** Node.js con TypeScript.
- **Frontend:** React (TypeScript).
- **Diagramación:** Draw.io.
- **Prototipado:** Figma.
- **Control de versiones:** Git / GitHub.

## Autores

- Jorge Gallardo Heck
- Pedro Breit Lira
