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
**1. Header / Navbar**
<br>

![alt text](docs/assets/chapter-4/landing-page-wireframe/header-navbar-landing-wireframe.png)

**2. Hero Section**
<br>

![alt text](docs/assets/chapter-4/landing-page-wireframe/hero-section-landing-wireframe.png)

**3. Key Features**
<br>

![alt text](docs/assets/chapter-4/landing-page-wireframe/key-features-landing-wireframe.png)

**4. Problem + Solution Section**
<br>

![alt text](docs/assets/chapter-4/landing-page-wireframe/problem+solution-section-landing-wireframe.png)

**5. Tools Section**
<br>

![alt text](docs/assets/chapter-4/landing-page-wireframe/tools-section-landing-wireframe.png)

**6. How it works Section**
<br>

![alt text](docs/assets/chapter-4/landing-page-wireframe/how-it-works-landing-wireframe.png)


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
Wireflow Diagram - 1<br><br>
<img src="docs/assets/chapter4-designUX/diagram-usergoal-1.png" width="800px">
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
Wireflow Diagram - 2 <br><br>
<img src="docs/assets/chapter4-designUX/diagram-usergoal-2.png" width="800px">
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
Wireflow Diagram - 3<br><br>
<img src="docs/assets/chapter4-designUX/diagram-usergoal-3.png" width="800px">
</div>

<table>
  <tr>
    <td class="header">User Persona</td>
    <td>Administrador - dueño del taller</td>
    <td class="header">Número</td>
    <td>4</td>
  </tr>
  <tr>
    <td class="header">User Goal</td>
    <td colspan="3" class="italic bold">
    </td>
  </tr>
  <tr>
    <td class="header">Happy path</td>
    <td colspan="3">
    El flujo inicia en la pantalla de bienvenida (Start), desde donde el usuario accede a la plataforma mediante el botón “Get Started”, siendo redirigido a la pantalla de inicio de sesión.

Una vez autenticado, el sistema dirige al administrador al panel de control (Dashboard), donde puede visualizar un resumen general del taller, incluyendo:

- Cantidad de vehículos activos
- Servicios en proceso
- Órdenes completadas
- Ingresos generados

Desde esta vista, el administrador accede a la sección de vehículos, donde el sistema muestra un listado completo con información resumida de cada unidad (placa, propietario, estado y progreso).

El usuario selecciona un vehículo específico mediante la opción “Ver detalles”, lo que lo redirige a la pantalla de detalle del vehículo. En esta vista, el sistema presenta:

- Información general del vehículo
- Estado actual del servicio
- Problema reportado
- Diagnóstico técnico
- Lista de tareas asociadas

Desde esta misma pantalla, el administrador puede presionar el botón “+ Agregar tarea”, lo que lo lleva a la pantalla de creación de nueva tarea.

En esta sección, el usuario registra:

- Nombre de la tarea
- Descripción del servicio
- Estado (pendiente, en proceso o completado)
- Tiempo estimado

Una vez completados los campos, el administrador presiona “Siguiente”, y el sistema lo redirige a la pantalla de orden de trabajo, donde se visualiza el conjunto completo de tareas asociadas al vehículo, junto con su estado actual y progreso global.
    </td>
  </tr>
</table>

<div align="center">

![alt text](docs/assets/chapter4-designUX/wireflow-usergoal-4.png)
Wireflow Diagram - 4<br><br>
<img src="docs/assets/chapter4-designUX/diagram-usergoal-4.png" width="800px">
</div>

<table>
  <tr>
    <td class="header">User Persona</td>
    <td>Administrador - dueño del taller</td>
    <td class="header">Número</td>
    <td>5</td>
  </tr>
  <tr>
    <td class="header">User Goal</td>
    <td colspan="3" class="italic bold">
    Registrar un nuevo vehículo en el sistema, ingresando la información del vehículo y del propietario, con el fin de gestionar correctamente los servicios y mantener actualizado el control de vehículos atendidos.
    </td>
  </tr>
  <tr>
    <td class="header">Happy path</td>
    <td colspan="3">
    El flujo inicia en la pantalla de bienvenida (Start), donde el usuario accede a la aplicación mediante el botón “Get Started”. A continuación, se presenta la pantalla de inicio de sesión (Login), en la cual el usuario ingresa su correo electrónico y contraseña para autenticarse en el sistema.

Una vez autenticado, el usuario es dirigido al panel de control (Dashboard), donde puede visualizar un resumen general del estado del taller, incluyendo vehículos activos, servicios en proceso, completados e ingresos. Desde esta pantalla, el usuario puede navegar hacia el módulo de gestión de vehículos.

Al ingresar a la sección “Vehículos”, se muestra una lista con los vehículos registrados, junto con su estado y detalles básicos. En esta pantalla, el usuario tiene la opción de presionar el botón “Agregar vehículo”, lo que lo dirige al formulario de registro.

En la pantalla de “Agregar vehículo”, el usuario completa los datos requeridos, los cuales están divididos en dos secciones:

- Información del vehículo (placa, marca, modelo, año).
- Información del propietario (nombre completo, teléfono, entre otros)

Una vez completados los campos, el usuario selecciona la opción “Guardar vehículo”. Como resultado de esta acción, el sistema procesa la información y muestra una nueva pantalla con el estado actualizado, confirmando que el vehículo ha sido registrado correctamente.

Finalmente, se presenta un mensaje de confirmación (“Vehículo registrado correctamente”) junto con una opción para aceptar, lo que permite al usuario regresar al sistema y continuar con otras tareas.
    </td>
  </tr>
</table>

<div align="center">

![alt text](docs/assets/chapter4-designUX/wireflow-usergoal-5.png)
Wireflow Diagram - 5<br><br>
<img src="docs/assets/chapter4-designUX/diagram-usergoal-5.png" width="800px">
</div>


<table>
  <tr>
    <td class="header">User Persona</td>
    <td>Administrador - dueño del taller</td>
    <td class="header">Número</td>
    <td>6</td>
  </tr>
  <tr>
    <td class="header">User Goal</td>
    <td colspan="3" class="italic bold">
    Seguimiento a las tareas y eliminar una orden de trabajo, para mantener actualizado el estado de los servicios y optimizar la gestión operativa del taller
    </td>
  </tr>
  <tr>
    <td class="header">Happy path</td>
    <td colspan="3">
    
El usuario al iniciar tendra que iniciar sesion para poder ingresar.
Una vez dentro del sistema, el usuario es dirigido al panel de control (panel), en el cual visualiza un resumen general del estado del taller, incluyendo vehículos activos, órdenes en proceso y métricas relevantes. Desde esta pantalla, el usuario navega hacia el módulo de “Órdenes”.

En la sección de órdenes de trabajo, el usuario accede al detalle de una orden específica, donde se muestra el identificador de la orden, el vehículo asociado y el progreso de las tareas asignadas. En esta vista, el usuario puede visualizar la lista de tareas, cada una con su estado (completada, en curso o pendiente).

El usuario puede gestionar estas tareas realizando diferentes acciones, como editar una tarea existente, marcar su estado o eliminarla mediante los controles disponibles en cada ítem. Asimismo, puede añadir nuevas tareas si es necesario.

Dentro de este flujo, también se contempla la posibilidad de eliminar una orden de trabajo, acción que se ejecuta a través de una opción disponible en la interfaz (generalmente asociada a un ícono de eliminación). Al realizar esta acción, el sistema actualiza el estado eliminando la orden del listado y reflejando el cambio en la interfaz.
Finalmente, el sistema mantiene actualizado el progreso de la orden en función de las tareas gestionadas, permitiendo al usuario tener control completo sobre el ciclo de trabajo.
    </td>
  </tr>
</table>

<div align="center">

![alt text](docs/assets/chapter4-designUX/wireflow-usergoal-6.png)
Wireflow Diagram - 6<br><br>
<img src="docs/assets/chapter4-designUX/diagram-usergoal-6.png" width="800px">
</div>


<table>
  <tr>
    <td class="header">User Persona</td>
    <td>Administrador - dueño del taller</td>
    <td class="header">Número</td>
    <td>7</td>
  </tr>
  <tr>
    <td class="header">User Goal</td>
    <td colspan="3" class="italic bold">
    Asignar una tarea a un mecánico disponible, seleccionar al personal adecuado según su especialidad, para asegurar una correcta distribución del trabajo y una atención eficiente de los servicios
    </td>
  </tr>
  <tr>
    <td class="header">Happy path</td>
    <td colspan="3">
    El flujo inicia en la pantalla de bienvenida (Start), donde el usuario accede a la aplicación mediante el botón “Get Started”. Seguidamente, se presenta la pantalla de inicio de sesión (Login), en la cual el usuario ingresa sus credenciales para autenticarse en el sistema.

Una vez dentro, el usuario es dirigido al panel de control (Dashboard), donde visualiza un resumen del estado del taller, incluyendo vehículos activos, servicios en proceso y métricas generales. Desde esta vista, el usuario puede navegar hacia la sección correspondiente para gestionar el personal o las órdenes de trabajo.

Posteriormente, el usuario accede a la pantalla de “Asignar mecánico”, donde se muestra la información del vehículo en espera junto con el tipo de servicio requerido. En esta misma pantalla, se presenta una lista de personal disponible, incluyendo datos relevantes como nombre del mecánico, especialidad y estado (disponible u ocupado).

El usuario selecciona al mecánico más adecuado en función de la tarea a realizar y su disponibilidad. Una vez hecha la selección, presiona el botón “Asignar tarea”, lo que ejecuta la acción dentro del sistema.

Como resultado, el sistema procesa la asignación y muestra una nueva pantalla con el estado actualizado, confirmando que la tarea ha sido registrada correctamente. Finalmente, el usuario puede aceptar la confirmación y continuar gestionando otras actividades dentro del sistema.
    </td>
  </tr>
</table>

<div align="center">

![alt text](docs/assets/chapter4-designUX/wireflow-usergoal-7.png)
Wireflow Diagram - 7<br><br>
<img src="docs/assets/chapter4-designUX/diagram-usergoal-7.png" width="800px">
</div>


<table>
  <tr>
    <td class="header">User Persona</td>
    <td>Administrador - dueño del taller</td>
    <td class="header">Número</td>
    <td>8</td>
  </tr>
  <tr>
    <td class="header">User Goal</td>
    <td colspan="3" class="italic bold">
    Registrar un nuevo mecánico en el sistema, ingresando sus datos personales, especialidad y estado inicial, para gestionar adecuadamente el equipo de trabajo y asignar tareas de manera eficiente.
    </td>
  </tr>
  <tr>
    <td class="header">Happy path</td>
    <td colspan="3">
    El flujo inicia en la pantalla de bienvenida (Start), donde el usuario accede a la aplicación mediante el botón “Get Started”. Luego, se presenta la pantalla de inicio de sesión (Login), en la cual el usuario ingresa sus credenciales para autenticarse.

Una vez dentro del sistema, el usuario es dirigido al panel de control (Panel), donde puede visualizar un resumen del estado del taller, incluyendo métricas generales como vehículos activos, servicios en proceso y resultados económicos. Desde esta pantalla, el usuario navega hacia el módulo de “Personal”.

En la sección de gestión de personal, el usuario visualiza la lista de mecánicos registrados, junto con información relevante como su especialidad y estado (disponible u ocupado). En esta pantalla, el usuario selecciona la opción “Añadir mecánico” para iniciar el proceso de registro.

A continuación, se muestra el formulario de “Agregar mecánico”, donde el usuario ingresa los datos requeridos, tales como nombre completo, especialidad, número de teléfono y estado inicial del trabajador. Una vez completada la información, el usuario presiona el botón “Guardar” para registrar al nuevo mecánico.

Como resultado de esta acción, el sistema procesa los datos y presenta una nueva pantalla con el estado actualizado, confirmando que el mecánico ha sido registrado correctamente. Finalmente, el usuario puede aceptar la confirmación y continuar gestionando otras funcionalidades del sistema.
    </td>
  </tr>
</table>

<div align="center">

![alt text](docs/assets/chapter4-designUX/wireflow-usergoal-8.png)
<p>Wireflow Diagram - 8</p><br><br>
<img src="docs/assets/chapter4-designUX/diagram-usergoal-8.png" width="800px">
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

<p align="justify">
  En esta sección se presenta el diseño orientado a objetos del sistema <strong>AutoService</strong>, 
  alineado con los principios de <strong>Domain-Driven Design (DDD)</strong> y 
  <strong>Clean Architecture</strong>.
</p>

<p align="justify">
  Los diagramas de clases modelan la estructura estática de cada 
  <strong>Bounded Context</strong> identificado en el <strong>Event Storming</strong>, 
  asegurando una clara separación de responsabilidades, alta cohesión y bajo acoplamiento.
</p>



<table>
  <thead>
    <tr>
      <th>Característica</th>
      <th>Descripción</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>Notación UML Estándar</td>
      <td align="justify">Se utiliza la sintaxis oficial de diagramas de clases.</td>
    </tr>
    <tr>
      <td>Visibilidad (Scope)</td>
      <td align="justify">- private, + public, # protected – encapsulamiento.</td>
    </tr>
    <tr>
      <td>Tipos de Datos C#</td>
      <td align="justify">Guid, string, DateTime, decimal, bool, int – tipado nativo .NET.</td>
    </tr>
    <tr>
      <td>Relaciones Explícitas</td>
      <td align="justify">Nombre de rol, dirección de navegación y multiplicidad (1, 0..1, *).</td>
    </tr>
    <tr>
      <td>Optimización para Persistencia</td>
      <td align="justify">Entidades consolidadas para mapeo directo al modelo relacional de 16 tablas.</td>
    </tr>
    <tr>
      <td>Patrones y Principios</td>
      <td align="justify">SOLID (SRP, DIP), Repository, Factory, Strategy.</td>
    </tr>
  </tbody>
</table>


#### 4.7.1. Class Diagrams

##### Diagrama de Clases General - AutoService

<div align="center">
<img src="docs/assets/chapter-4/class-diagrams/class-diagram-autoservice.png"width="1000">
</div>


##### Identity & Profile Context

###### Responsabilidades Principales
- Autenticación de usuarios mediante credenciales seguras (hash de contraseñas)
- Gestión de roles y asignación a usuarios
- Control de acceso multi-tenant mediante **WorkshopId**
- Auditoría de asignación de roles (fecha de asignación)

###### Reglas de Negocio Clave
- Cada usuario pertenece a un único taller (**WorkshopId**), asegurando aislamiento multi-tenant
- Los roles disponibles son: **Admin**, **Mechanic**, **Client**
- Un usuario puede tener múltiples roles simultáneamente
- La asignación de roles registra la fecha para trazabilidad
- Solo usuarios activos (**IsActive = true**) pueden autenticarse

<div align="center">
<img src="docs/assets/chapter-4/class-diagrams/class-diagram-identity-&-profile-context.png"width="400">
</div>


##### Workshop Operations Context (Core Domain)

###### Responsabilidades Principales
- Gestión del ciclo de vida completo de las órdenes de trabajo
- Registro y mantenimiento de información de clientes y vehículos
- Desglose operativo de servicios en tareas asignables a mecánicos
- Seguimiento del estado de servicios y auditoría de cambios
- Generación de códigos de seguimiento para transparencia al cliente

###### Reglas de Negocio Clave
- Cada orden de trabajo debe estar asociada a un vehículo y un taller
- Los vehículos deben tener un único propietario (cliente) registrado
- El estado de la orden sigue un flujo definido: **PENDING → IN_PROGRESS → COMPLETED → DELIVERED** (con soporte para **CANCELLED**)
- Cada cambio de estado se registra en **StatusHistory** para auditoría
- Cada orden genera un código de seguimiento único para consulta del cliente
- El monto total de la orden se calcula a partir de los costos de sus tareas

<div align="center">
<img src="docs/assets/chapter-4/class-diagrams/class-diagram-workshop-operations-context-core.png"width="800">
</div>


##### Staff Management Context (Supporting Domain)

###### Responsabilidades Principales
- Registro y gestión de información laboral de mecánicos
- Asignación y control de turnos de trabajo
- Validación de conflictos de horarios
- Cálculo de métricas laborales (ingresos semanales)
- Verificación de disponibilidad del personal técnico

###### Reglas de Negocio Clave
- Cada mecánico está asociado a un usuario del sistema (**UserId**) para autenticación
- Un mecánico pertenece a un único taller (**WorkshopId**)
- Los turnos de un mismo mecánico no pueden superponerse en el tiempo (**IsOverlapping()**)
- El estado **IsActive** determina si el mecánico está disponible para asignación
- Los tipos de turno son: **MORNING**, **AFTERNOON**, **NIGHT**, **OVERTIME**

<div align="center">
<img src="docs/assets/chapter-4/class-diagrams/class-diagram-staff-management-context.png"width="300">
</div>


##### Billing & Payment Context (Supporting Domain)

###### Responsabilidades Principales
- Generación de facturas y comprobantes fiscales
- Cálculo de subtotales, impuestos y totales
- Gestión de ítems detallados por factura
- Registro de pagos con múltiples métodos
- Procesamiento y seguimiento de transacciones
- Soporte para cancelación y reembolsos

###### Reglas de Negocio Clave
- Cada factura puede estar asociada a una orden de trabajo (relación opcional **0..1**)
- Los totales se calculan automáticamente a partir de los ítems y la tasa de impuesto
- Una factura puede recibir un solo pago (relación **0..1**), simplificando el modelo
- Se soportan múltiples métodos de pago: **efectivo**, **tarjeta crédito/débito**, **transferencia**
- Los pagos tienen un ciclo de vida: **PENDING → PROCESSING → COMPLETED / FAILED**
- Las facturas pueden estar en estado: **DRAFT**, **ISSUED**, **PAID**, **CANCELLED** o **OVERDUE**

<div align="center">
<img src="docs/assets/chapter-4/class-diagrams/class-diagram-billing-&-payment-context.png"width="500">
</div>


##### Customer Tracking & Notification Context (Supporting Domain)

###### Responsabilidades Principales
- Registro de notificaciones enviadas a clientes
- Envío de notificaciones a través de múltiples canales (Email, SMS, Push, WhatsApp)
- Seguimiento del estado de entrega de notificaciones
- Trazabilidad completa de la comunicación por cliente y orden de trabajo
- Soporte para notificaciones automáticas basadas en eventos del sistema

###### Reglas de Negocio Clave
- Cada notificación se registra antes de ser enviada, garantizando trazabilidad
- Las notificaciones se vinculan al cliente destinatario (**ClientId**)
- Opcionalmente, una notificación puede asociarse a una orden de trabajo (**WorkOrderId**)
- Los tipos de notificación incluyen: **actualización de estado**, **orden completada**, **pago recibido** y **recordatorios**
- El sistema soporta múltiples canales: **Email**, **SMS**, **Push Notification** y **WhatsApp**
- El ciclo de vida de una notificación es: **PENDING → SENT → DELIVERED / FAILED**

<div align="center">
<img src="docs/assets/chapter-4/class-diagrams/class-diagram-customer-tracking-&-notification-context.png"width="450">
</div>


##### Reporting & Analytics Context (Supporting Domain)

###### Responsabilidades Principales
- Generación de reportes bajo demanda o programada
- Almacenamiento de metadata de reportes generados (tipo, rango de fechas, URL del archivo)
- Exportación de reportes en múltiples formatos (PDF, Excel)
- Trazabilidad de quién generó cada reporte y cuándo

###### Regla de Negocio Clave
- Los reportes pueden generarse por rango de fechas personalizado
- Cada reporte está asociado a un taller específico (**WorkshopId**)
- Los tipos de reporte disponibles son: ingresos diarios, productividad semanal, resumen mensual y desempeño de mecánicos
- Los reportes generados se almacenan como archivos (PDF/Excel) con una URL de acceso
- La lógica de cálculo de métricas se ejecuta al momento de generar el reporte, consultando datos en vivo

<div align="center">
<img src="docs/assets/chapter-4/class-diagrams/class-diagram-reporting-&-analytics-context.png"width="300">
</div>


### 4.8. Database Design


<p align="justify">
En esta sección se presenta el diseño de la base de datos relacional para el <strong>AutoService</strong>, alineado con los <strong>Bounded Contexts</strong> identificados en el análisis de <strong>Domain-Driven Design (DDD)</strong> y optimizado para cumplir con el alcance del proyecto.
</p>


#### Características Principales del Diseño


<div style="overflow-x: auto;">
  <table>
    <thead>
      <tr>
        <th scope="col">Característica</th>
        <th scope="col">Descripción</th>
      </tr>
    </thead>
    <tbody>
      <tr>
        <td>Motor de Base de Datos</td>
        <td style="text-align: justify;">
          PostgreSQL 15+ / SQL Server 2019+ (según configuración del entorno).
        </td>
      </tr>
      <tr>
        <td>Normalización</td>
        <td style="text-align: justify;">
          Tercera Forma Normal (3NF) para eliminar redundancias y garantizar integridad referencial.
        </td>
      </tr>
      <tr>
        <td>Claves Primarias</td>
        <td style="text-align: justify;">
          Todas las tablas utilizan Guid/UUID como clave primaria para escalabilidad distribuida y evitar conflictos en entornos multi-tenant.
        </td>
      </tr>
      <tr>
        <td>Claves Foráneas</td>
        <td style="text-align: justify;">
          Relaciones explícitas con restricciones ON DELETE CASCADE o ON DELETE RESTRICT según la lógica de negocio y preservación de datos históricos.
        </td>
      </tr>
      <tr>
        <td>Índices</td>
        <td style="text-align: justify;">
          Índices en columnas de búsqueda frecuente (Plate, Email, OrderNumber, StatusEnum, WorkshopId) para optimizar consultas.
        </td>
      </tr>
      <tr>
        <td>Soft Delete</td>
        <td style="text-align: justify;">
          Columna IsActive o IsArchived en entidades críticas para preservación histórica sin eliminación física.
        </td>
      </tr>
      <tr>
        <td>Auditoría Básica</td>
        <td style="text-align: justify;">
          Columnas CreatedAt, UpdatedAt en tablas transaccionales para trazabilidad temporal.
        </td>
      </tr>
      <tr>
        <td>Enumeraciones</td>
        <td style="text-align: justify;">
          Campos INT con valores controlados para estados (WorkOrderStatus, PaymentStatus) garantizando consistencia de datos a nivel de aplicación.
        </td>
      </tr>
      <tr>
        <td>Multi-tenancy</td>
        <td style="text-align: justify;">
          Columna WorkshopId en tablas operativas para aislamiento lógico entre talleres (modelo SaaS), con políticas de Row-Level Security (RLS) opcionales.
        </td>
      </tr>
    </tbody>
  </table>
</div>


#### 4.8.1. Database Diagrams



##### Diagrama de Base de Datos General - AutoService

<div align="center">

![alt text](docs/assets/chapter-4/database-diagram/database-diagram-autoservice.png)
</div>


##### Identity & Profile Context
Este contexto gestiona la autenticación, autorización y configuración multi-tenant del sistema.

<div align="center">
<img src="docs/assets/chapter-4/database-diagram/database-diagram-identity-&-profile-context.png"width="600">
</div>


##### Workshop Operations Context (Core Domain)
El núcleo del negocio: gestión de órdenes de trabajo, tareas y seguimiento.

<div align="center">
<img src="docs/assets/chapter-4/database-diagram/database-diagram-workshop-operations-context-core.png"width="1000">
</div>


##### Staff Management Context (Supporting Domain)
Administra el personal técnico, sus turnos y disponibilidad operativa.

<div align="center">
<img src="docs/assets/chapter-4/database-diagram/database-diagram-staff-management-context.png"width="600">
</div>


##### Billing & Payment Context (Supporting Domain)
Gestiona la facturación, comprobantes y registro de transacciones económicas.

<div align="center">
<img src="docs/assets/chapter-4/database-diagram/database-diagram-billing-&-payment-context.png"width="800">
</div>


##### Customer Tracking & Notification Context (Supporting Domain)
Facilita la comunicación proactiva con el cliente final y el seguimiento externo.

<div align="center">
<img src="docs/assets/chapter-4/database-diagram/database-diagram-customer-tracking-&-notification-context.png"width="500">
</div>


##### Reporting & Analytics Context (Supporting Domain)
El contexto de Reporting se alimenta de las siguientes tablas operativas distribuidas en otros Bounded Contexts como Customer & Assets Context
Gestiona la información de clientes propietarios y sus vehículos registrados.

<div align="center">
<img src="docs/assets/chapter-4/database-diagram/database-diagram-customer-&-assets-context.png"width="350">
</div>
