## Capítulo IV: Product Design

### 4.1. Style Guidelines

#### 4.1.1. General Style Guidelines
[Pendiente]

#### 4.1.2. Web Style Guidelines
[Pendiente]

### 4.2. Information Architecture

<p align="justify">
Esta sección detalla cómo se organiza, etiqueta y estructura la información dentro de la plataforma AutoService para garantizar que los diferentes segmentos de usuario puedan navegar intuitivamente. El objetivo es minimizar el esfuerzo cognitivo tanto del personal del taller al gestionar operaciones como del cliente final al consultar el estado de su vehículo.
</p>
<p align="justify">
Para AutoService, se han implementado diversos sistemas de organización que responden a las necesidades operativas y de consulta del negocio:
</p>

#### 4.2.1. Organization Systems

<p style="text-align: justify;">
  <ul>
    <li>
      <strong>Jerarquía Visual (Visual Hierarchy):</strong> Se aplica principalmente en el Dashboard Administrativo, donde los indicadores críticos (KPIs) como el número de vehículos en proceso, ingresos del día y órdenes pendientes se presentan en la parte superior con un diseño destacado para una rápida interpretación.
    </li>
    <li>
      <strong>Organización Secuencial (Step-by-step):</strong> Se utiliza estrictamente en el flujo de creación de una Orden de Trabajo y en el registro de servicios. El sistema guía al mecánico a través de pasos lógicos: Información del cliente &gt; Datos del vehículo &gt; Diagnóstico inicial &gt; Asignación de tareas y costos.
    </li>
    <li>
      <strong>Esquema Cronológico:</strong> Se emplea en el Historial de Servicios de cada vehículo. Los registros se organizan del más reciente al más antiguo, permitiendo que tanto el taller como el dueño del auto visualicen la evolución del mantenimiento en el tiempo.
    </li>
    <li>
      <strong>Categorización según Audiencia:</strong> La estructura se divide en dos grandes rutas de acceso:
      <ul>
        <li><strong>Panel Operativo (B2B):</strong> Orientado a mecánicos y administradores para la gestión de flota, personal y facturación.</li>
        <li><strong>Portal de Seguimiento (B2C):</strong> Una interfaz simplificada para el propietario del vehículo, centrada únicamente en el progreso y transparencia del servicio actual.</li>
      </ul>
    </li>
  </ul>
</p>

#### 4.2.2. Labeling Systems

<p style="text-align: justify;">
  El sistema de etiquetado utiliza términos técnicos automotrices estandarizados en inglés para mantener la consistencia con las convenciones de desarrollo del proyecto.
</p>

<ul style="text-align: justify;">
  <li>
    <strong>Etiquetas de Navegación (Sidebar/Navbar):</strong>
    <ul>
      <li>Dashboard: Vista general de métricas.</li>
      <li>Vehicles: Listado y gestión de unidades.</li>
      <li>Work Orders: Control de servicios activos.</li>
      <li>Staff: Gestión del personal mecánico.</li>
      <li>Billing: Generación de comprobantes y pagos.</li>
    </ul>
  </li>

  <li>
    <strong>Etiquetas de Acción (Botones/CTAs):</strong>
    <ul>
      <li>Register Vehicle: Iniciar registro de unidad.</li>
      <li>Update Status: Cambiar etapa del servicio (Pending, In Process, Ready).</li>
      <li>Generate Invoice: Crear comprobante de pago.</li>
      <li>Track My Vehicle: Acceso para el cliente final.</li>
    </ul>
  </li>

  <li>
    <strong>Etiquetas de Estado:</strong>
    <ul>
      <li>Diagnostic: Etapa de revisión inicial.</li>
      <li>In Repair: Ejecución de tareas mecánicas.</li>
      <li>Ready for Pickup: Vehículo listo para entrega.</li>
    </ul>
  </li>
</ul>

#### 4.2.3. SEO Tags and Meta Tags

<p style="text-align: justify;">
  A continuación, se definen los metadatos estratégicos para el posicionamiento y la identidad de la plataforma tanto en la Landing Page como en la Aplicación Web:
</p>

<table style="width: 100%; border-collapse: collapse; text-align: justify;">
  <thead>
    <tr style="background-color: #f2f2f2;">
      <th style="border: 1px solid #ddd; padding: 8px;">Página</th>
      <th style="border: 1px solid #ddd; padding: 8px;">Title Tag</th>
      <th style="border: 1px solid #ddd; padding: 8px;">Meta Description</th>
      <th style="border: 1px solid #ddd; padding: 8px;">Keywords</th>
      <th style="border: 1px solid #ddd; padding: 8px;">Author</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td style="border: 1px solid #ddd; padding: 8px;">Landing Page</td>
      <td style="border: 1px solid #ddd; padding: 8px;">AutoService - Digital Management for Workshops</td>
      <td style="border: 1px solid #ddd; padding: 8px;">
        Optimiza tu taller mecánico con seguimiento en tiempo real, gestión de órdenes y transparencia para el cliente.
      </td>
      <td style="border: 1px solid #ddd; padding: 8px;">
        workshop software, mechanic SaaS, vehicle tracking, taller digital, gestión automotriz
      </td>
      <td style="border: 1px solid #ddd; padding: 8px;">InnovaTech Studio</td>
    </tr>
    <tr>
      <td style="border: 1px solid #ddd; padding: 8px;">Web Application (Dashboard)</td>
      <td style="border: 1px solid #ddd; padding: 8px;">AutoService</td>
      <td style="border: 1px solid #ddd; padding: 8px;">
        Panel de control operativo para gestión integral de servicios automotrices.
      </td>
      <td style="border: 1px solid #ddd; padding: 8px;">app, workshop, management, ERP, automotive.</td>
      <td style="border: 1px solid #ddd; padding: 8px;">InnovaTech Studio</td>
    </tr>
  </tbody>
</table>

#### 4.2.4. Searching Systems

<p style="text-align: justify;">
  Para evitar que los usuarios se pierdan ante grandes volúmenes de datos, se han definido los siguientes mecanismos de búsqueda y filtrado:
</p>

<ul style="text-align: justify;">
  <li>
    <strong>Búsqueda Global por Placa (License Plate):</strong> El buscador principal permite localizar rápidamente cualquier vehículo en el sistema ingresando el número de placa, lo cual redirige al detalle de su Orden de Trabajo activa.
  </li>
  <li>
    <strong>Filtros de Estado en Tiempo Real:</strong> En el listado de órdenes, el usuario puede filtrar por "Pending", "In Process" o "Completed" para priorizar las tareas del día.
  </li>
  <li>
    <strong>Filtros por Rango de Fechas:</strong> Aplicable en la sección de reportes financieros y de productividad para analizar el desempeño del taller en periodos específicos.
  </li>
  <li>
    <strong>Presentación de Resultados:</strong> Los datos se muestran en formato de tarjetas (cards) o tablas interactivas con resaltado de sintaxis para los estados críticos.
  </li>
</ul>

#### 4.2.5. Navigation Systems

<p style="text-align: justify;">
  El sistema de navegación está diseñado para ser consistente entre la Landing Page y la Aplicación, guiando al usuario hacia sus objetivos finales:
</p>

<ul style="text-align: justify;">
  <li>
    <strong>Navegación Global (Navbar):</strong> Presente en la Landing Page para dirigir a los usuarios potenciales a las secciones de beneficios, precios y el acceso al sistema (Login).
  </li>
  <li>
    <strong>Navegación Vertical (Sidebar):</strong> Menú lateral persistente en la Web Application que permite el tránsito rápido entre los módulos operativos (Vehicles, Staff, Orders).
  </li>
  <li>
    <strong>Breadcrumbs (Migas de Pan):</strong> Utilizadas en las vistas de detalle (ej: Work Orders &gt; Order #1234 &gt; Task Update) para que el usuario siempre sepa en qué nivel de la jerarquía se encuentra.
  </li>
  <li>
    <strong>Navegación Contextual (CTAs):</strong> Enlaces directos desde el Dashboard hacia las acciones más frecuentes, como "Add New Vehicle" o "View Pending Tasks".
  </li>
</ul>

### 4.3. Landing Page UI Design

#### 4.3.1. Landing Page Wireframe
[Pendiente]

#### 4.3.2. Landing Page Mock-up
[Pendiente]

### 4.4. Web Applications UX/UI Design

#### 4.4.1. Web Applications Wireframes
[Pendiente]

#### 4.4.2. Web Applications Wireflow Diagrams

<table>
  <tr>
    <td class="header">User Persona</td>
    <td>Cliente - dueño del vehículo</td>
    <td class="header">Número</td>
    <td>1</td>
  </tr>
  <tr>
    <td class="header">User Goal</td>
    <td colspan="3" class="italic bold">
      Ingresar al sistema, visualizar y consultar el estado de mi vehículo mediante un código de seguimiento, para conocer el progreso del servicio, el diagnóstico y la fecha estimada de entrega sin necesidad de contactar directamente al taller.
    </td>
  </tr>
  <tr>
    <td class="header">Happy path</td>
    <td colspan="3">
       El usuario tiene la opción de acceder a la plataforma mediante el botón “Get Started”. Al seleccionarlo, el sistema redirige a la pantalla de inicio de sesión, en la cual el cliente ingresa sus credenciales (correo electrónico y contraseña).
Una vez autenticado correctamente, el sistema presenta la pantalla de ingreso de código de seguimiento, donde el usuario introduce el identificador proporcionado por el taller. Como paso adicional de validación, se muestra una segunda pantalla para el ingreso de un código de 4 dígitos, reforzando la seguridad del acceso.
Tras validar el código, el sistema redirige al usuario a la pantalla principal “Mi vehículo”, donde se visualiza un resumen del estado actual del servicio, incluyendo el progreso general, el estado (por ejemplo, en proceso) y accesos a información clave.
Finalmente, el usuario puede acceder al detalle completo del servicio, donde el sistema muestra información más específica como:

- Estado de cada etapa (recibido, diagnóstico, reparación, completado)
- Porcentaje de avance
- Técnico asignado
- Ubicación del vehículo dentro del taller
- Fecha estimada de entrega
    </td>
  </tr>
</table>

<div align="center">

![alt text](docs/assets/chapter4-designUX/wireflow-usergoal-1.png)
</div>


<table>
  <tr>
    <td class="header">User Persona</td>
    <td>Cliente - dueño del vehículo</td>
    <td class="header">Número</td>
    <td>2</td>
  </tr>
  <tr>
    <td class="header">User Goal</td>
    <td colspan="3" class="italic bold">
      Visualizar el detalle completo del servicio del vehículo y realizar el pago correspondiente, para entender los trabajos realizados, conocer los costos y completar el proceso de manera digital y segura.
    </td>
  </tr>
  <tr>
    <td class="header">Happy path</td>
    <td colspan="3">
Una vez iniciado sesion y validado el codigo, el usuario accede a la pantalla principal “Mi vehículo”, donde puede visualizar un resumen del estado del servicio. Desde esta vista, el cliente selecciona la opción “Ver detalles”, lo que lo dirige a la pantalla de detalle del servicio.

En esta sección, el sistema muestra información específica del vehículo y del proceso de mantenimiento, incluyendo:

- Lista de tareas realizadas o en progreso
- Estado de cada actividad
- Notas del técnico
- Evidencias visuales (imágenes de referencia)

Desde esta pantalla, el usuario puede acceder al resumen del servicio, donde se presenta un desglose claro de los costos, incluyendo:

- Tipo de servicios realizados
- Precio por cada tarea
- Subtotal o costo total
- Estado general del servicio

A continuación, el cliente tiene la opción de proceder con el pago mediante el botón “Pagar”, lo que lo redirige a la pantalla de método de pago. En esta vista, el usuario puede seleccionar entre distintas opciones (tarjeta, billeteras digitales o pago en taller).

Finalmente, al confirmar la transacción, el sistema muestra una pantalla de confirmación de pago exitoso, cerrando el flujo de manera satisfactoria.
    </td>
  </tr>
</table>

<div align="center">

![alt text](docs/assets/chapter4-designUX/wireflow-usergoal-2.png)
</div>
<table>
  <tr>
    <td class="header">User Persona</td>
    <td>Cliente - dueño del vehículo</td>
    <td class="header">Número</td>
    <td>3</td>
  </tr>
  <tr>
    <td class="header">User Goal</td>
    <td colspan="3" class="italic bold">
     Agendar cita de mantenimiento para un vehículo, para seleccionar una fecha y hora disponible de manera rápida y asegurar la atención en el taller sin necesidad de coordinación manual
    </td>
  </tr>
  <tr>
    <td class="header">Happy path</td>
    <td colspan="3">
     Tras completar el proceso de iniciar sesion e iniciar con el codigo de 4 digitos, el cliente accede a la pantalla principal “Mi vehículo”, donde puede visualizar el estado general del servicio. Desde esta vista, el usuario navega hacia la sección de notificaciones, donde el sistema muestra alertas y mensajes relevantes relacionados con su vehículo.

Dentro de esta sección, el usuario identifica una notificación asociada a mantenimiento preventivo y selecciona la opción “Agendar ahora”, lo que lo redirige a la pantalla de agendamiento de cita.

En esta pantalla, el sistema permite al cliente:

- Visualizar el tipo de servicio (por ejemplo, mantenimiento de neumáticos)
- Seleccionar una fecha mediante un calendario interactivo
- Elegir un horario disponible
- Confirmar el vehículo asociado al servicio

Una vez completados estos campos, el usuario presiona el botón “Confirmar cita”, lo que lleva a una pantalla de confirmación exitosa, indicando que la cita ha sido registrada correctamente.
    </td>
  </tr>
</table>

<div align="center">

![alt text](docs/assets/chapter4-designUX/wireflow-usergoal-3.png)
</div>


#### 4.4.3. Web Applications Mock-ups
[Pendiente]

#### 4.4.4. Web Applications User Flow Diagrams
[Pendiente]

### 4.5. Web Applications Prototyping
[Pendiente]

### 4.6. Domain-Driven Software Architecture

<p align="justify">
La arquitectura de software de AutoService se fundamenta en los principios de Domain-Driven Design (DDD), permitiendo una traducción directa entre las necesidades operativas del negocio automotriz y la estructura del sistema técnico. Mediante la aplicación del Modelo C4, representamos la arquitectura en distintos niveles de abstracción, asegurando que la solución sea escalable, mantenible y esté estrictamente alineada con los contextos delimitados identificados durante el proceso de EventStorming.
</p>

#### 4.6.1. Design-Level EventStorming

<p align="justify">
Para profundizar en la lógica de AutoService<, realizamos una sesión de Design-Level Event Storming. Esta técnica nos permitió transitar desde una visión general del negocio hacia un modelo técnico detallado, identificando los procesos críticos, las reglas de negocio y los límites de los módulos que compondrán nuestra arquitectura orientada a servicios.
</p>

<b>Step 1: Collect Domain Events (Big Picture)</b>
<p align="justify">
En esta fase inicial, realizamos una lluvia de ideas para identificar todos los Domain Events relevantes en el ciclo de vida del taller, desde el registro de la cuenta hasta el procesamiento de comprobantes. Los eventos se redactaron en tiempo pasado, enfocándonos exclusivamente en hechos significativos para el negocio sin preocuparnos por el orden cronológico.
</p>

<div align="center">

![alt text](docs/assets/chapter-4/event_storming_s1.jpg)
</div>

<b>Step 2: Refine Domain Events</b>
<p align="justify">
Organizamos los eventos identificados en una línea de tiempo horizontal para establecer el flujo lógico de la plataforma. Durante este proceso, refinamos la secuencia y detectamos eventos faltantes, como la generación automática de códigos de seguimiento y el disparo de notificaciones, asegurando una narrativa coherente de la experiencia del usuario.
</p>

<div align="center">

![alt text](docs/assets/chapter-4/event_storming_s2.jpg)
</div>

<b>Step 3: Track Causes (Process Modelling)</b>
<p align="justify">
En este paso, modelamos la causalidad de cada evento introduciendo <b>Actors</b> (quién realiza la acción), <b>Commands</b> (la acción ejecutada), <b>External Systems</b> y <b>Policies</b> (reglas automáticas). Esto nos permitió visualizar cómo interactúan los mecánicos y clientes con el sistema y qué procesos se disparan automáticamente tras un cambio de estado.
</p>

<div align="center">

![alt text](docs/assets/chapter-4/event_storming_s3.jpg)
</div>

<b>Step 4: Find Aggregates & Bounded Contexts (Software Modelling)</b>
<p align="justify">
Finalmente, agrupamos los comandos y eventos alrededor de sus <b>Aggregates</b> (entidades principales de datos) para definir los <b>Bounded Contexts</b>. Esta segmentación estratégica establece los límites de responsabilidad para nuestro API RESTful, identificando módulos clave como <i>Workshop Operations</i>, <i>Staff Management</i> y <i>Billing</i>.
</p>

<div align="center">

![alt text](docs/assets/chapter-4/event_storming_s4.jpg)
</div>

#### 4.6.2. Software Architecture Context Diagram

<p align="justify">
El diagrama de contexto representa el nivel más alto de abstracción de la solución AutoService Platform. Este diagrama permite visualizar cómo el sistema interactúa con su entorno, identificando a los actores principales: el Mecánico/Administrador, quien gestiona las operaciones del taller, y el Cliente Final, quien realiza el seguimiento de sus vehículos. Asimismo, se muestra la interacción con sistemas externos esenciales como el Messaging Service, encargado del envío automatizado de notificaciones de estado y comprobantes electrónicos de pago.
</p>

<div align="center">

![alt text](docs/assets/chapter-4/context_diagram_aw.png)
</div>

#### 4.6.3. Software Architecture Container Diagrams

<p align="justify">
A nivel de contenedores, la solución se descompone en aplicaciones independientes que colaboran para ofrecer la funcionalidad completa de la plataforma. Siguiendo un enfoque de arquitectura desacoplada, se han definido los siguientes contenedores:
</p>

<ul style="text-align: justify;">
<li><strong>Landing Page:</strong> Desarrollada con HTML5, CSS3 y JavaScript, se encarga de proveer información del producto y captar nuevos talleres hacia el modelo SaaS.</li>
<li><strong>Web Application (SPA):</strong> Construida con Vue.js, actúa como la interfaz principal donde los administradores gestionan el taller y los clientes finales consultan el progreso de sus reparaciones.</li>
<li><strong>API RESTful:</strong> Constituye el núcleo de la lógica de negocio, implementado con C# y ASP.NET Core. Centraliza todas las reglas de dominio y expone servicios web mediante el intercambio de JSON.</li>
<li><strong>Database:</strong> Una instancia de SQL Server encargada de la persistencia segura y relacional de la información de clientes, vehículos, órdenes y facturación.</li>
</ul>

<div align="center">

![alt text](docs/assets/chapter-4/containers_diagram_aw.png)
</div>

#### 4.6.4. Software Architecture Components Diagrams

<p align="justify">
Este diagrama profundiza en el contenedor API RESTful para exponer los bloques estructurales internos que implementan los casos de uso definidos en el dominio. La lógica interna se organiza a través de componentes especializados:
</p>

<ul style="text-align: justify;">
<li><strong>Security Layer:</strong> Basado en ASP.NET Identity, este componente gestiona la identidad, autenticación y autorización mediante tokens JWT, protegiendo el acceso a los recursos del sistema.</li>
<li><strong>Workshop Logic:</strong> Componente encargado de la orquestación de servicios de taller, incluyendo la gestión de flota, diagnósticos y el control de las órdenes de trabajo.</li>
<li><strong>Tracking Logic:</strong> Servicio dedicado a procesar y proveer la información de seguimiento en tiempo real, permitiendo a los clientes visualizar el avance de sus vehículos.</li>
<li><strong>Invoice Logic:</strong> Gestiona la generación de documentos financieros y la emisión de comprobantes digitales de pago una vez finalizados los servicios.</li>
<li><strong>Analytics Engine:</strong> Componente analítico que procesa los datos operativos para calcular métricas de productividad del staff y generar reportes financieros detallados para los administradores.</li>
</ul>

<div align="center">

![alt text](docs/assets/chapter-4/components_diagram_aw.png)
</div>

### 4.7. Software Object-Oriented Design

#### 4.7.1. Class Diagrams
[Pendiente]

### 4.8. Database Design

#### 4.8.1. Database Diagrams
[Pendiente]