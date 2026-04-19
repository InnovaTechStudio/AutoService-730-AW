## Capítulo IV: Product Design

### 4.1. Style Guidelines

#### 4.1.1. General Style Guidelines
[Pendiente]

#### 4.1.2. Web Style Guidelines
[Pendiente]

### 4.2. Information Architecture

#### 4.2.1. Organization Systems
[Pendiente]

#### 4.2.2. Labeling Systems
[Pendiente]

#### 4.2.3. SEO Tags and Meta Tags
[Pendiente]

#### 4.2.4. Searching Systems
[Pendiente]

#### 4.2.5. Navigation Systems
[Pendiente]

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

#### 4.6.1. Design-Level EventStorming
[Pendiente]

#### 4.6.2. Software Architecture Context Diagram
[Pendiente]

#### 4.6.3. Software Architecture Container Diagrams
[Pendiente]

#### 4.6.4. Software Architecture Components Diagrams
[Pendiente]

### 4.7. Software Object-Oriented Design

#### 4.7.1. Class Diagrams
[Pendiente]

### 4.8. Database Design

#### 4.8.1. Database Diagrams
[Pendiente]