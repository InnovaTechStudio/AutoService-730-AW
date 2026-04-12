## Capítulo V: Product Implementation, Validation & Deployment

### 5.1. Software Configuration Management

#### 5.1.1. Software Development Environment Configuration
<p align="justify">
  La siguiente tabla presenta las herramientas, plataformas y guías empleadas para la configuración del entorno de desarrollo del software, que detalla su       finalidad dentro del proyecto y el medio de acceso correspondiente.
</p>

<table>
  <thead>
    <tr>
      <th>Proceso</th>
      <th>Recurso o plataforma</th>
      <th>Finalidad</th>
      <th>Medio de acceso o Enlace</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>Especificación de requisitos</td>
      <td>Convenciones Gherkin</td>
      <td>Establecer condiciones y criterios funcionales precisos</td>
      <td><a href="https://cucumber.io/docs/gherkin/" target="_blank" aria-label="Ir a la página Guia Gherkin">Guía Gherkin</a></td>
    </tr>
    <tr>
      <td>Desarrollo Landing Page</td>
      <td>Visual Studio Code</td>
      <td>Programar, editar y optimizar el código fuente</td>
      <td><a href="https://code.visualstudio.com/" target="_blank" aria-label="Ir a la página de Visual Studio Code">Visual Studio Code</a></td>
    </tr>
    <tr>
      <td>Administración de versiones</td>
      <td>Git</td>
      <td>Registrar cambios y controlar las versiones del proyecto</td>
      <td><a href="https://git-scm.com/" target="_blank" aria-label="Ir a la página de Git">Git</a></td>
    </tr>
    <tr>
      <td>Diseño de experiencia e interfaz</td>
      <td>Figma</td>
      <td>Crear prototipos visuales y estructurar la interfaz del usuario</td>
      <td><a href="https://figma.com" target="_blank" aria-label="Ir a la página de Figma">Figma</a></td>
    </tr>
    <tr>
      <td>Publicación y despliegue</td>
      <td>Github Pages</td>
      <td>Implementar y alojar la página web en línea</td>
      <td><a href="https://pages.github.com/" target="_blank" aria-label="Ir a la página de Github Pages">Github Pages</a></td>
    </tr>
    <tr>
      <td>Planificación y gestión del proyecto</td>
      <td>Jira Software</td>
      <td>Gestionar el Product Backlog, Sprint Planning y seguimiento de tareas bajo metodología ágil</td>
      <td><a href="https://www.atlassian.com/es/software/jira" target="_blank" aria-label="Ir a la página de Jira Software">Jira Software</a></td>
    </tr>
    <tr>
      <td>Diagramas</td>
      <td>PlantUML</td>
      <td>Diseñar representaciones UML del sistema</td>
      <td><a href="https://plantuml.com/" target="_blank" aria-label="Ir a la página de UML">PlantUML</a></td>
    </tr>
    <tr>
      <td>Modelado de procesos</td>
      <td>UXPressia</td>
      <td>Elaborar herramientas de análisis UX centradas en el usuario</td>
      <td><a href="https://uxpressia.com/" target="_blank" aria-label="Ir a la página de UXPressia">UXPressia</a></td>
    </tr>
  </tbody>
</table>


#### 5.1.2. Source Code Management
<p align="justify">
  Para la gestión, control de versiones del proyecto y seguimiento del proyecto, el equipo utiliza GitHub como plataforma principal de almacenamiento del código fuente y colaboración. Esta herramienta permite mantener un historial detallado de los cambios realizados, facilitar el trabajo en equipo y asegurar la trazabilidad de cada modificación durante el ciclo de desarrollo.
  
  En la etapa actual del proyecto, se ha adoptado un flujo de trabajo basado en Git Flow, complementado con prácticas de Github Flow para la integración y revisión colaborativa de cambios. Esta estrategia permite una mejor organización del desarrollo, especialmente que considere el crecimiento progresivo del sistema y la necesidad de gestionar nuevas funcionalidades de manera estructurada.
  
  La estructura implementada considera las siguientes ramas principales: la rama main, que contiene la versión estable y desplegable del sistema; la rama develop, destinada a integrar los avances en desarrollo antes de su paso a producción; las ramas feature/, utilizadas para el desarrollo de nuevas funcionalidades o mejoras específicas; y las ramas hotfix/, orientadas a correcciones urgentes sobre la versión en producción.

  Cada nueva funcionalidad o corrección es desarrollada en una rama independiente creada a partir de develop, lo que permite mantener el aislamiento de cambios y reducir conflictos durante la integración. Una vez finalizado el desarrollo, los cambios son incorporados mediante Pull Requests, los cuales son revisados previamente por los integrantes del equipo antes de su fusión, siguiendo buenas prácticas de colaboración y control de calidad.

  Asimismo, con el propósito de mantener claridad y consistencia en el historial del repositorio, se ha adoptado la convención Conventional Commits, la cual estandariza la estructura de los mensajes de confirmación. Esta práctica facilita la identificación rápida del tipo de cambio realizado y mejora la legibilidad del historial de versiones.

  A continuación, se presentan algunos de los prefijos utilizados en los commits:
  
  - **feat** : para la incorporación de nuevas funcionalidades.
  - **fix**: para la corrección de errores.
  - **docs**: para modificaciones en la documentación.
  - **refactor**: para mejoras en la estructura interna del código sin alterar su funcionalidad.
  - **style**: ajustes de formato o estilo del código.
  - **test**: incorporación o actualización de pruebas.
  
  Por otra parte, el proyecto adopta el uso de versionado semántico (Semantic Versioning) bajo el esquema MAJOR.MINOR.PATCH, lo que permite clasificar de forma ordenada la evolución del sistema según la magnitud de los cambios implementados.

  De esta manera, el equipo garantiza una gestión eficiente del código fuente, que promueve la mantenibilidad, la colaboración y la escalabilidad del proyecto a lo largo de sus futuras iteraciones.
</p>

#### 5.1.3. Source Code Style Guide & Conventions
[Pendiente]

#### 5.1.4. Software Deployment Configuration
[Pendiente]

### 5.2. Landing Page, Services & Applications Implementation

#### 5.2.1. Sprint 1

##### 5.2.1.1. Sprint Planning 1
[Pendiente]

##### 5.2.1.2. Aspect Leaders and Collaborators
[Pendiente]

##### 5.2.1.3. Sprint Backlog 1
[Pendiente]

##### 5.2.1.4. Development Evidence for Sprint Review
[Pendiente]

##### 5.2.1.5. Execution Evidence for Sprint Review
[Pendiente]

##### 5.2.1.6. Services Documentation Evidence for Sprint Review
[Pendiente]

##### 5.2.1.7. Software Deployment Evidence for Sprint Review
[Pendiente]

##### 5.2.1.8. Team Collaboration Insights during Sprint
[Pendiente]

### 5.3. Validation Interviews

#### 5.3.1. Diseño de Entrevistas
[Pendiente]

#### 5.3.2. Registro de Entrevistas
[Pendiente]

#### 5.3.3. Evaluaciones según heurísticas
[Pendiente]

### 5.4. Video About-the-Product
[Pendiente]