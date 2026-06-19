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
<p align="justify">
  Con el objetivo de asegurar la calidad, mantenibilidad y escalabilidad de la solución propuesta, se ha definido un conjunto de lineamientos de estilo y convenciones de codificación aplicables a todos los lenguajes utilizados en el proyecto, específicamente HTML, CSS, JavaScript y C#.
  
  Como criterio general, todo el código fuente, que incluye nombres de variables, clases, archivos, comentarios técnicos y documentación interna, será redactado en idioma inglés, con el fin de mantener uniformidad y alinearse con estándares internacionales de desarrollo de software.
  
  Asimismo, se adoptan buenas prácticas basadas en guías reconocidad como Google Style Guides, MDN JavaScript, MDN JavaScript Guidelines, Microsoft C# Coding Conventions y lineamientos estándar de accesibilidad y legibilidad.

  **HTML Conventions**
  
  Para la estructura del frontend se empleará HTML5 semántico, que prioriza la correcta organización del contenido y la accesibilidad.

  Las principales convenciones adoptadas son:
  - Uso de etiquetas semánticas como &lt;header&gt;, &lt;nav&gt;, &lt;main&gt;, &lt;section&gt;, &lt;article&gt; y &lt;footer&gt; para mejorar la estructura lógica del documento.
  - Nombres de etiquetas y atributos escritos exclusivamente en minúsculas.
  - Cierre correcto de todas las etiquetas HTML.
  - Inclusión obligatoria del atributo alt en imágenes para mejorar la accesibilidad.
  - Uso de atributos width y height en imágenes cuando corresponde, para optimizar la carga visual.
  - Definición del atributo lang="en" en la etiqueta &lt;html&gt;.
  - Inclusión de metadatos esenciales como &lt;title&gt; y &lt;meta name="descripcion"&gt;.
  - Evitar el uso innecesario de estilos o scripts inline.

  Ejemplo:
  ``` HTML
  <section class="hero-banner">
      <img src="banner.jpg" alt="Main promotional banner" width="1200" height="600">
  </section>
  ```

**CSS Conventions**

  Para la hoja de estilos se seguirá una estructura modular y escalable, enfocada en la reutilización de componentes.
  Las convenciones establecidas son:
  - Uso de nomenclatura kebab-case para clases CSS.
  - Aplicación de la metodología BEM (Block Element Modifier) para mejorar la organización visual y funcional de estilos.
  - Uso de nombres descriptivos y significativos.
  - Declaraciones ordenadas de forma lógica: layout, box model, tipografía y visual.
  - Uso preferente de unidades relativas como rem, % y vh/vw.
  - Omisión de unidades en valores cero.
  - Implementación de diseño responsive con enfoque mobile-first.
  - Uso de variables CSS definidas en :root.

  ``` CSS
  :root{
      --primary-color: #2563eb;
      --secondary-color: #64748b;
  }

  .main-header{
      padding: 1rem;
      background-color: var(--primary-color);
  }
  ```

**JavaScript Conventions**

Para la lógica del lado del cliente se adoptarán lineamientos orientados a la claridad, reutilización y mantenimiento del código.
Se aplicarán las siguientes convenciones:
- Uso de camelCase para variable y funciones.
- Uso de PascalCase para clases y constructores.
- Declaraciones de variables con const y let, evitando el uso de var.
- Separación modular del código en archivos independientes según funcionalida.
- Uso de addEventListener() en lugar de eventos inline.
- Comentarios únicamente en lógica compleja o no evidente.
- Nombres de funciones descriptivos y orientados a acciones.

Ejemplo:
``` JavaScript
const submitButton = document.querySelector("#submit-button");
function validateForm(){
  return true;
}
```

**C# Conventions**

Para el desarrollo backend y lógica de negocio en C#, se seguirán las convenciones recomendadas por Microsoft.
Estas incluyen:
- Uso de PascalCase para clases, métodos y propiedades.
- Uso de camelCase para variables locales y parámetros.
- Métodos con nombres descriptivos orientados a verbos.
- Aplicación del principio de Single Responsibility Principle (SRP).
- Mantener longitud de línea razonable para facilitar lectura.
- Comentarios claros y breves en métodos críticos.
- Organización del código por capas: controllers, services, repositories y models.
  
Ejemplo:
``` C#
public class UserService
{
    public bool ValidateCredentials(string userEmail, string password)
    {
        return true;
    }
}
```

**Gherkin Conventions**

Para la definición de criterios de aceptación y pruebas funcionales se utilizará el lenguaje Gherkin, que sigue una estructura orientada al negocio.
Las convenciones definidas son:
- Uso obligatorio de la estructura Given-When-Then
- Redacción en lenguaje comprensible para stakeholders no técnicos.
- Escenarios con títulos claros y específicos.
- Uso de Scenario Outline cuando existan múltiples casos similares.
  
Ejemplo:
``` gherkin
Feature: User Login

Scenario: Sucessful login
    Given the user is on the login page
    When the user enters valid credential
    Then the system should redirect to the dashboard
```
**Coding Principles Adopted**

De manera transversal, el equipo aplicará los siguientes principios:
- Readbility First: código fácil de leer y entender.
- Consistency: mantener el mismo estilo en toda la solución.
- Modularity: separación clara de responsabilidades.
- Scalability: estructura preparada para crecimiento futuro.
- Maintainability: facilidad para futuras modificaciones.
</p>

#### 5.1.4. Software Deployment Configuration
**Landing Page Deployment - HTML, CSS and JavaScript**

**Source Repository Setup**
<p>
  Para la publicación de la Landing Page se utilizará un repositorio remoto alojado en GiHub, en el cual se almacenarán todos los archivos fuente correspondientes a la interfaz web estática.
  Dado que la solución ha sido con HTML, CSS y JavaScript, es indispensable que el archivo principal index.html permanezca en la raíz del repositorio, ya que este será tomado como archivo inicial durante el proceso de despliegue. Del mismo modo, los archivos complementarios como hojas de estilo, scripts e imágenes se organizarán en directorios específicos para facilitar el mantenimiento del proyecto.
  
  Ejemplo:
  ```
  /
  |---index.html
  |---css/
  |    |__ styles.css
  |---js/
  |    |__ main.js
  |---assets/
        |__ images/
  ```
</p>

**Deployment Process**
<p>
  La publicación del sitio se realizará mediante el servicio GitHub Pages, el cual permite desplegar sitios estáticos directamente desde el repositorio.
  Para habilitar el despliegue, se seguirán los siguientes pasos:
  - Ingresar al repositorio del proyecto en GitHub
  - Acceder al apartado Settings
  - Seleccionar la opción Pages
  - Elegir la opción Pages
  - Elegir la rama main como fuente de publicación
  - Establecer la carpeta raíz /root como directorio de despliegue
  - Guardar la configuración
  Una vez completado este proceso, GitHub iniciará automáticamente la generación del sitio web.
</p>

**Published Access**
<p>
  Finalizada la configuración, la plataforma proporcionará un enlace público mediante el cual se podrá acceder a la Landing Page desplegada.
  La URL seguirá una estructura similar a la siguiente:
  
  ```
  https://<usernanme>.github.io/<repository-name>/
  ```

  Este enlace corresponderá a la versión oficial publicada del producto.
</p>

**Version Updates**
<p>
  Cada vez que el equipo realice modificaciones en la Landing Page, estas deberán enviarse al repositorio mediante nuevos commits.
  Al actualizar la rama principal, el servicio GitHub Pages reflejará automáticamente los cambios en la versión publicada, que permitirán mantener el sitio sincronizado con la última versión estable del código fuente.
</p>

### 5.2. Landing Page, Services & Applications Implementation

#### 5.2.1. Sprint 1

##### 5.2.1.1. Sprint Planning 1

<div align="center">
  <table style="margin: auto; width: 100%; border-collapse: collapse; text-align: left;">
    <thead>
      <tr>
        <th colspan="2" style="text-align: center; background-color: #f2f2f2; font-size: 1.2em; padding: 10px; border: 1px solid #ddd;">Sprint #1</th>
      </tr>
    </thead>
    <tbody>
      <tr>
        <td colspan="2" style="background-color: #fafafa; font-weight: bold; text-align: center; padding: 10px; border: 1px solid #ddd;">Sprint Planning Background</td>
      </tr>
      <tr>
        <td style="width: 30%; font-weight: bold; padding: 10px; border: 1px solid #ddd;">Date</td>
        <td style="padding: 10px; border: 1px solid #ddd;">2026-04-08</td>
      </tr>
      <tr>
        <td style="font-weight: bold; padding: 10px; border: 1px solid #ddd;">Time</td>
        <td style="padding: 10px; border: 1px solid #ddd;">10:00 AM</td>
      </tr>
      <tr>
        <td style="font-weight: bold; padding: 10px; border: 1px solid #ddd;">Location</td>
        <td style="padding: 10px; border: 1px solid #ddd;">Reunión presencial en la UPC. (Pabellón L, piso 4, cubículo 11)</td>
      </tr>
      <tr>
        <td style="font-weight: bold; padding: 10px; border: 1px solid #ddd;">Prepared By</td>
        <td style="padding: 10px; border: 1px solid #ddd;">Sanchez Cuadrado, Juan Antonio</td>
      </tr>
      <tr>
        <td style="font-weight: bold; padding: 10px; border: 1px solid #ddd;">Attendees (to planning meeting)</td>
        <td style="padding: 10px; border: 1px solid #ddd;">López Monroy, Rodrigo Alfredo / Luis Miranda, Diego Andres / Mamani Vilca, Alan Jaivi / Pillaca Gonzales, Andy Saúl / Sanchez Cuadrado, Juan Antonio</td>
      </tr>
      <tr>
        <td style="font-weight: bold; padding: 10px; border: 1px solid #ddd;">Sprint 0 Review Summary</td>
        <td style="padding: 10px; border: 1px solid #ddd;">Al ser la iteración inicial del proyecto, no existe un Sprint previo para revisar. El equipo se enfocó en el setup inicial de herramientas, creación de la organización en GitHub y configuración del espacio de trabajo en Jira Software.</td>
      </tr>
      <tr>
        <td style="font-weight: bold; padding: 10px; border: 1px solid #ddd;">Sprint 0 Retrospective Summary</td>
        <td style="padding: 10px; border: 1px solid #ddd;">Al ser el primer ciclo, no hay retrospectiva previa. Sin embargo, el equipo acordó como norma de trabajo el uso estricto de Feature Branching para el control de versiones y la comunicación constante ante bloqueos técnicos.</td>
      </tr>
      <tr>
        <td colspan="2" style="background-color: #fafafa; font-weight: bold; text-align: center; padding: 10px; border: 1px solid #ddd;">Sprint Goal & User Stories</td>
      </tr>
      <tr>
        <td style="font-weight: bold; padding: 10px; border: 1px solid #ddd;">Sprint 1 Goal</td>
        <td style="padding: 10px; border: 1px solid #ddd;">
          <strong>Our focus is on</strong> deploying the official Landing Page and establishing the core software architecture and database design.<br><br>
          <strong>We believe it delivers</strong> a solid online presence for early user acquisition and a reliable technical foundation for the development team.<br><br>
          <strong>This will be confirmed when</strong> the Landing Page is publicly accessible via a web link with responsive design, and the C4 Model diagrams along with the Database Entity-Relationship diagram are fully documented and approved.
        </td>
      </tr>
      <tr>
        <td style="font-weight: bold; padding: 10px; border: 1px solid #ddd;">Sprint 1 Velocity</td>
        <td style="padding: 10px; border: 1px solid #ddd;">27 Story Points</td>
      </tr>
      <tr>
        <td style="font-weight: bold; padding: 10px; border: 1px solid #ddd;">Sum of Story Points</td>
        <td style="padding: 10px; border: 1px solid #ddd;">27 Story Points (US-01: 3, US-02: 2, US-03: 1, US-04: 3, TS-01: 5, TS-04: 3, TS-10: 5, TS-11: 5).</td>
      </tr>
    </tbody>
  </table>
</div>

##### 5.2.1.2. Aspect Leaders and Collaborators

En el presente Sprint 1, el alcance funcional y técnico se ha dividido en tres aspectos principales para garantizar una entrega eficiente:
1. Landing Page (Frontend): Desarrollo de la interfaz gráfica e identidad visual.
2. Architecture & Database: Diseño de diagramas C4 y modelado relacional de la base de datos.
3. DevOps & Deployment: Configuración de repositorios, CI/CD básico y hosting estático.

<div align="center">
  <table style="margin: auto; width: 100%; border-collapse: collapse; text-align: center;">
    <thead>
      <tr style="background-color: #f2f2f2;">
        <th style="padding: 10px; border: 1px solid #ddd; text-align: left;">Team Member (Last Name, First Name)</th>
        <th style="padding: 10px; border: 1px solid #ddd;">GitHub Username</th>
        <th style="padding: 10px; border: 1px solid #ddd;">Landing Page (Frontend)<br><small>Leader (L) / Collaborator (C)</small></th>
        <th style="padding: 10px; border: 1px solid #ddd;">Architecture & Database<br><small>Leader (L) / Collaborator (C)</small></th>
        <th style="padding: 10px; border: 1px solid #ddd;">DevOps & Deployment<br><small>Leader (L) / Collaborator (C)</small></th>
      </tr>
    </thead>
    <tbody>
      <tr>
        <td style="padding: 10px; border: 1px solid #ddd; text-align: left;">López Monroy, Rodrigo Alfredo</td>
        <td style="padding: 10px; border: 1px solid #ddd;">rodrigolopezu</td>
        <td style="padding: 10px; border: 1px solid #ddd; color: #1976d2;">C</td>
        <td style="padding: 10px; border: 1px solid #ddd; color: #1976d2;">C</td>
        <td style="padding: 10px; border: 1px solid #ddd; font-weight: bold; color: #2e7d32;">L</td>
      </tr>
      <tr>
        <td style="padding: 10px; border: 1px solid #ddd; text-align: left;">Luis Miranda, Diego Andres</td>
        <td style="padding: 10px; border: 1px solid #ddd;">andrewdmr</td>
        <td style="padding: 10px; border: 1px solid #ddd; font-weight: bold; color: #2e7d32;">L</td>
        <td style="padding: 10px; border: 1px solid #ddd; color: #1976d2;">C</td>
        <td style="padding: 10px; border: 1px solid #ddd; color: #1976d2;">C</td>
      </tr>
      <tr>
        <td style="padding: 10px; border: 1px solid #ddd; text-align: left;">Mamani Vilca, Alan Jaivi</td>
        <td style="padding: 10px; border: 1px solid #ddd;">alanmamaniv</td>
        <td style="padding: 10px; border: 1px solid #ddd; color: #1976d2;">C</td>
        <td style="padding: 10px; border: 1px solid #ddd; font-weight: bold; color: #2e7d32;">L</td>
        <td style="padding: 10px; border: 1px solid #ddd; color: #1976d2;">C</td>
      </tr>
      <tr>
        <td style="padding: 10px; border: 1px solid #ddd; text-align: left;">Pillaca Gonzales, Andy Saúl</td>
        <td style="padding: 10px; border: 1px solid #ddd;">apillacag</td>
        <td style="padding: 10px; border: 1px solid #ddd; color: #1976d2;">C</td>
        <td style="padding: 10px; border: 1px solid #ddd; color: #1976d2;">C</td>
        <td style="padding: 10px; border: 1px solid #ddd; color: #1976d2;">C</td>
      </tr>
      <tr>
        <td style="padding: 10px; border: 1px solid #ddd; text-align: left;">Sanchez Cuadrado, Juan Antonio</td>
        <td style="padding: 10px; border: 1px solid #ddd;">juanasc05</td>
        <td style="padding: 10px; border: 1px solid #ddd; color: #1976d2;">C</td>
        <td style="padding: 10px; border: 1px solid #ddd; font-weight: bold; color: #2e7d32;">L</td>
        <td style="padding: 10px; border: 1px solid #ddd; color: #1976d2;">C</td>
      </tr>
    </tbody>
  </table>
</div>

##### 5.2.1.3. Sprint Backlog 1

El presente Sprint Backlog detalla la descomposición técnica de las historias de usuario y técnicas seleccionadas para la primera iteración. El objetivo principal de este Sprint es establecer la presencia web inicial mediante la Landing Page y sentar las bases arquitectónicas del sistema. A continuación, se presenta la captura de nuestro tablero en Jira Software, seguida de la tabla de control de estado con la distribución de los Work-Items.

<div align="center">

![alt text](docs/assets/sprint1_jira.png)

</div>

URL del tablero completo en Jira: https://innovatechstudio.atlassian.net/jira/software/projects/ASS/boards/1/backlog

<div align="center">
  <table style="margin: auto; width: 100%; border-collapse: collapse; text-align: left; font-size: 13px; border: 1px solid #ddd;">
    <thead>
      <tr style="background-color: #e0e0e0; font-weight: bold;">
        <th style="padding: 10px; text-align: center; border: 1px solid #ddd;">Sprint #</th>
        <th colspan="7" style="padding: 10px; text-align: left; border: 1px solid #ddd;">1</th>
      </tr>
      <tr style="background-color: #f2f2f2;">
        <th colspan="2" style="text-align: center; border: 1px solid #ddd; padding: 10px;">User Story</th>
        <th colspan="6" style="text-align: center; border: 1px solid #ddd; padding: 10px;">Work-Item / Task</th>
      </tr>
      <tr style="background-color: #fafafa; text-align: center;">
        <th style="border: 1px solid #ddd; padding: 5px; width: 6%;">Id</th>
        <th style="border: 1px solid #ddd; padding: 5px; width: 15%;">Title</th>
        <th style="border: 1px solid #ddd; padding: 5px; width: 6%;">Id</th>
        <th style="border: 1px solid #ddd; padding: 5px; width: 15%;">Title</th>
        <th style="border: 1px solid #ddd; padding: 5px; width: 30%;">Description</th>
        <th style="border: 1px solid #ddd; padding: 5px; width: 8%;">Estimation (Hours)</th>
        <th style="border: 1px solid #ddd; padding: 5px; width: 12%;">Assigned To</th>
        <th style="border: 1px solid #ddd; padding: 5px; width: 8%;">Status</th>
      </tr>
    </thead>
    <tbody>
      <tr>
        <td rowspan="2" style="border: 1px solid #ddd; padding: 8px; vertical-align: middle; text-align: center; font-weight: bold;">US-01</td>
        <td rowspan="2" style="border: 1px solid #ddd; padding: 8px; vertical-align: middle;">Visualizar landing page</td>
        <td style="border: 1px solid #ddd; padding: 8px; text-align: center;">WI-01</td>
        <td style="border: 1px solid #ddd; padding: 8px;">Diseño inicial</td>
        <td style="border: 1px solid #ddd; padding: 8px;"><i>Diseñar wireframes y mockup inicial de la estructura web.</i></td>
        <td style="border: 1px solid #ddd; padding: 8px; text-align: center;">4</td>
        <td style="border: 1px solid #ddd; padding: 8px;">Luis, Diego</td>
        <td style="border: 1px solid #ddd; padding: 8px; text-align: center; font-weight: bold; color: #2aac2a;">Done</td>
      </tr>
      <tr>
        <td style="border: 1px solid #ddd; padding: 8px; text-align: center;">WI-02</td>
        <td style="border: 1px solid #ddd; padding: 8px;">Setup Frontend</td>
        <td style="border: 1px solid #ddd; padding: 8px;"><i>Configurar proyecto base utilizando React y Tailwind CSS.</i></td>
        <td style="border: 1px solid #ddd; padding: 8px; text-align: center;">3</td>
        <td style="border: 1px solid #ddd; padding: 8px;">López, Rodrigo</td>
        <td style="border: 1px solid #ddd; padding: 8px; text-align: center; font-weight: bold; color: #2aac2a;">Done</td>
      </tr>
      <tr>
        <td rowspan="2" style="border: 1px solid #ddd; padding: 8px; vertical-align: middle; text-align: center; font-weight: bold;">US-02</td>
        <td rowspan="2" style="border: 1px solid #ddd; padding: 8px; vertical-align: middle;">Visualizar beneficios del sistema</td>
        <td style="border: 1px solid #ddd; padding: 8px; text-align: center;">WI-03</td>
        <td style="border: 1px solid #ddd; padding: 8px;">Redacción Copy</td>
        <td style="border: 1px solid #ddd; padding: 8px;"><i>Redactar y estructurar el contenido (copy) explicativo.</i></td>
        <td style="border: 1px solid #ddd; padding: 8px; text-align: center;">2</td>
        <td style="border: 1px solid #ddd; padding: 8px;">Sanchez, Juan</td>
        <td style="border: 1px solid #ddd; padding: 8px; text-align: center; font-weight: bold; color: #2aac2a;">Done</td>
      </tr>
      <tr>
        <td style="border: 1px solid #ddd; padding: 8px; text-align: center;">WI-04</td>
        <td style="border: 1px solid #ddd; padding: 8px;">Componente Cards</td>
        <td style="border: 1px solid #ddd; padding: 8px;"><i>Desarrollar los componentes de tarjetas para beneficios.</i></td>
        <td style="border: 1px solid #ddd; padding: 8px; text-align: center;">4</td>
        <td style="border: 1px solid #ddd; padding: 8px;">Mamani, Alan</td>
        <td style="border: 1px solid #ddd; padding: 8px; text-align: center; font-weight: bold; color: #2aac2a;">Done</td>
      </tr>
      <tr>
        <td rowspan="2" style="border: 1px solid #ddd; padding: 8px; vertical-align: middle; text-align: center; font-weight: bold;">US-03</td>
        <td rowspan="2" style="border: 1px solid #ddd; padding: 8px; vertical-align: middle;">Acceder a la plataforma desde CTA</td>
        <td style="border: 1px solid #ddd; padding: 8px; text-align: center;">WI-05</td>
        <td style="border: 1px solid #ddd; padding: 8px;">Botones CTA</td>
        <td style="border: 1px solid #ddd; padding: 8px;"><i>Maquetar los botones de llamado a la acción.</i></td>
        <td style="border: 1px solid #ddd; padding: 8px; text-align: center;">2</td>
        <td style="border: 1px solid #ddd; padding: 8px;">Luis, Diego</td>
        <td style="border: 1px solid #ddd; padding: 8px; text-align: center; font-weight: bold; color: #2aac2a;">Done</td>
      </tr>
      <tr>
        <td style="border: 1px solid #ddd; padding: 8px; text-align: center;">WI-06</td>
        <td style="border: 1px solid #ddd; padding: 8px;">Enrutamiento React</td>
        <td style="border: 1px solid #ddd; padding: 8px;"><i>Configurar el enrutamiento base hacia vistas futuras.</i></td>
        <td style="border: 1px solid #ddd; padding: 8px; text-align: center;">3</td>
        <td style="border: 1px solid #ddd; padding: 8px;">Pillaca, Andy</td>
        <td style="border: 1px solid #ddd; padding: 8px; text-align: center; font-weight: bold; color: #2aac2a;">Done</td>
      </tr>
      <tr>
        <td rowspan="2" style="border: 1px solid #ddd; padding: 8px; vertical-align: middle; text-align: center; font-weight: bold;">US-04</td>
        <td rowspan="2" style="border: 1px solid #ddd; padding: 8px; vertical-align: middle;">Visualizar landing responsive</td>
        <td style="border: 1px solid #ddd; padding: 8px; text-align: center;">WI-07</td>
        <td style="border: 1px solid #ddd; padding: 8px;">Media Queries</td>
        <td style="border: 1px solid #ddd; padding: 8px;"><i>Aplicar clases utilitarias para ajuste a móviles y tablets.</i></td>
        <td style="border: 1px solid #ddd; padding: 8px; text-align: center;">4</td>
        <td style="border: 1px solid #ddd; padding: 8px;">Luis, Diego</td>
        <td style="border: 1px solid #ddd; padding: 8px; text-align: center; font-weight: bold; color: #2aac2a;">Done</td>
      </tr>
      <tr>
        <td style="border: 1px solid #ddd; padding: 8px; text-align: center;">WI-08</td>
        <td style="border: 1px solid #ddd; padding: 8px;">Testing UI</td>
        <td style="border: 1px solid #ddd; padding: 8px;"><i>Realizar validaciones de renderizado en pantallas.</i></td>
        <td style="border: 1px solid #ddd; padding: 8px; text-align: center;">2</td>
        <td style="border: 1px solid #ddd; padding: 8px;">Pillaca, Andy</td>
        <td style="border: 1px solid #ddd; padding: 8px; text-align: center; font-weight: bold; color: #2aac2a;">Done</td>
      </tr>
      <tr>
        <td rowspan="3" style="border: 1px solid #ddd; padding: 8px; vertical-align: middle; text-align: center; font-weight: bold;">TS-01</td>
        <td rowspan="3" style="border: 1px solid #ddd; padding: 8px; vertical-align: middle;">Definir arquitectura del sistema</td>
        <td style="border: 1px solid #ddd; padding: 8px; text-align: center;">WI-09</td>
        <td style="border: 1px solid #ddd; padding: 8px;">Context Diagram</td>
        <td style="border: 1px solid #ddd; padding: 8px;"><i>Diseñar Context Diagram bajo el modelo C4.</i></td>
        <td style="border: 1px solid #ddd; padding: 8px; text-align: center;">3</td>
        <td style="border: 1px solid #ddd; padding: 8px;">Mamani, Alan</td>
        <td style="border: 1px solid #ddd; padding: 8px; text-align: center; font-weight: bold; color: #2aac2a;">Done</td>
      </tr>
      <tr>
        <td style="border: 1px solid #ddd; padding: 8px; text-align: center;">WI-10</td>
        <td style="border: 1px solid #ddd; padding: 8px;">Container Diagram</td>
        <td style="border: 1px solid #ddd; padding: 8px;"><i>Diseñar Container Diagram bajo el modelo C4.</i></td>
        <td style="border: 1px solid #ddd; padding: 8px; text-align: center;">4</td>
        <td style="border: 1px solid #ddd; padding: 8px;">Sanchez, Juan</td>
        <td style="border: 1px solid #ddd; padding: 8px; text-align: center; font-weight: bold; color: #2aac2a;">Done</td>
      </tr>
      <tr>
        <td style="border: 1px solid #ddd; padding: 8px; text-align: center;">WI-11</td>
        <td style="border: 1px solid #ddd; padding: 8px;">Event Storming</td>
        <td style="border: 1px solid #ddd; padding: 8px;"><i>Elaborar el Design-Level Event Storming.</i></td>
        <td style="border: 1px solid #ddd; padding: 8px; text-align: center;">4</td>
        <td style="border: 1px solid #ddd; padding: 8px;">Mamani, Alan</td>
        <td style="border: 1px solid #ddd; padding: 8px; text-align: center; font-weight: bold; color: #2aac2a;">Done</td>
      </tr>
      <tr>
        <td rowspan="2" style="border: 1px solid #ddd; padding: 8px; vertical-align: middle; text-align: center; font-weight: bold;">TS-04</td>
        <td rowspan="2" style="border: 1px solid #ddd; padding: 8px; vertical-align: middle;">Diseñar modelo de base de datos</td>
        <td style="border: 1px solid #ddd; padding: 8px; text-align: center;">WI-12</td>
        <td style="border: 1px solid #ddd; padding: 8px;">Modelo Conceptual</td>
        <td style="border: 1px solid #ddd; padding: 8px;"><i>Identificar entidades y relaciones de negocio.</i></td>
        <td style="border: 1px solid #ddd; padding: 8px; text-align: center;">3</td>
        <td style="border: 1px solid #ddd; padding: 8px;">Sanchez, Juan</td>
        <td style="border: 1px solid #ddd; padding: 8px; text-align: center; font-weight: bold; color: #2aac2a;">Done</td>
      </tr>
      <tr>
        <td style="border: 1px solid #ddd; padding: 8px; text-align: center;">WI-13</td>
        <td style="border: 1px solid #ddd; padding: 8px;">Diagrama Lógico ER</td>
        <td style="border: 1px solid #ddd; padding: 8px;"><i>Elaborar el Diagrama Entidad-Relación de la BD.</i></td>
        <td style="border: 1px solid #ddd; padding: 8px; text-align: center;">5</td>
        <td style="border: 1px solid #ddd; padding: 8px;">Mamani, Alan</td>
        <td style="border: 1px solid #ddd; padding: 8px; text-align: center; font-weight: bold; color: #2aac2a;">Done</td>
      </tr>
      <tr>
        <td rowspan="2" style="border: 1px solid #ddd; padding: 8px; vertical-align: middle; text-align: center; font-weight: bold;">TS-10</td>
        <td rowspan="2" style="border: 1px solid #ddd; padding: 8px; vertical-align: middle;">Configurar entorno de desarrollo</td>
        <td style="border: 1px solid #ddd; padding: 8px; text-align: center;">WI-14</td>
        <td style="border: 1px solid #ddd; padding: 8px;">Configuración Git</td>
        <td style="border: 1px solid #ddd; padding: 8px;"><i>Definir estructura de repositorio y flujo de ramas.</i></td>
        <td style="border: 1px solid #ddd; padding: 8px; text-align: center;">3</td>
        <td style="border: 1px solid #ddd; padding: 8px;">López, Rodrigo</td>
        <td style="border: 1px solid #ddd; padding: 8px; text-align: center; font-weight: bold; color: #2aac2a;">Done</td>
      </tr>
      <tr>
        <td style="border: 1px solid #ddd; padding: 8px; text-align: center;">WI-15</td>
        <td style="border: 1px solid #ddd; padding: 8px;">Definir guía de estilos de código</td>
        <td style="border: 1px solid #ddd; padding: 8px;"><i>Code style guide and conventions.</i></td>
        <td style="border: 1px solid #ddd; padding: 8px; text-align: center;">5</td>
        <td style="border: 1px solid #ddd; padding: 8px;">Pillaca, Andy</td>
        <td style="border: 1px solid #ddd; padding: 8px; text-align: center; font-weight: bold; color: #2aac2a;">Done</td>
      </tr>
      <tr>
        <td rowspan="2" style="border: 1px solid #ddd; padding: 8px; vertical-align: middle; text-align: center; font-weight: bold;">TS-11</td>
        <td rowspan="2" style="border: 1px solid #ddd; padding: 8px; vertical-align: middle;">Desplegar aplicación</td>
        <td style="border: 1px solid #ddd; padding: 8px; text-align: center;">WI-16</td>
        <td style="border: 1px solid #ddd; padding: 8px;">Hosting de la landing page</td>
        <td style="border: 1px solid #ddd; padding: 8px;"><i>Configurar el servicio de hosting estático para la Landing Page.</i></td>
        <td style="border: 1px solid #ddd; padding: 8px; text-align: center;">4</td>
        <td style="border: 1px solid #ddd; padding: 8px;">López, Rodrigo</td>
        <td style="border: 1px solid #ddd; padding: 8px; text-align: center; font-weight: bold; color: #2aac2a;">Done</td>
      </tr>
      <tr>
        <td style="border: 1px solid #ddd; padding: 8px; text-align: center;">WI-17</td>
        <td style="border: 1px solid #ddd; padding: 8px;">Pruebas de acceso</td>
        <td style="border: 1px solid #ddd; padding: 8px;"><i>Verificar el acceso público al enlace.</i></td>
        <td style="border: 1px solid #ddd; padding: 8px; text-align: center;">2</td>
        <td style="border: 1px solid #ddd; padding: 8px;">Pillaca, Andy</td>
        <td style="border: 1px solid #ddd; padding: 8px; text-align: center; font-weight: bold; color: #2aac2a;">Done</td>
      </tr>
    </tbody>
  </table>
</div>

##### 5.2.1.4. Development Evidence for Sprint Review

<p align="justify">
Durante el Sprint 1, el equipo completó la base estratégica y técnica del proyecto, abarcando desde la definición del perfil de la startup hasta el diseño detallado del producto en los Capítulos I al IV. En cuanto a la implementación técnica, los esfuerzos se centraron en el diseño de mockups de alta fidelidad, el despliegue de la versión inicial de la Landing Page y la configuración de los entornos de desarrollo para la implementación de la Web Application y el RESTful API en los siguientes sprints.<br><br>
En la siguiente tabla se presentan commits que representan hitos clave del desarrollo de este sprint:
</p>

<table style="width: 100%; border-collapse: collapse; text-align: justify;">
  <thead>
    <tr style="background-color: #f2f2f2;">
      <th style="border: 1px solid #ddd; padding: 8px;">Repository</th>
      <th style="border: 1px solid #ddd; padding: 8px;">Branch</th>
      <th style="border: 1px solid #ddd; padding: 8px;">Commit Id</th>
      <th style="border: 1px solid #ddd; padding: 8px;">Commit Message</th>
      <th style="border: 1px solid #ddd; padding: 8px;">Commit Message Body</th>
      <th style="border: 1px solid #ddd; padding: 8px;">Commited on (Date)</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td style="border: 1px solid #ddd; padding: 8px;"><code>InnovaTechStudio/AutoService-730-AW</code></td>
      <td style="border: 1px solid #ddd; padding: 8px;"><code>main</code></td>
      <td style="border: 1px solid #ddd; padding: 8px;"><code>3648f26</code></td>
      <td style="border: 1px solid #ddd; padding: 8px;">chore:</td>
      <td style="border: 1px solid #ddd; padding: 8px;">initial project setup</td>
      <td style="border: 1px solid #ddd; padding: 8px;">12/04/2026</td>
    </tr>
    <tr>
      <td style="border: 1px solid #ddd; padding: 8px;"><code>InnovaTechStudio/AutoService-730-AW</code></td>
      <td style="border: 1px solid #ddd; padding: 8px;"><code>feature/chapter-1</code></td>
      <td style="border: 1px solid #ddd; padding: 8px;"><code>73c3ef0</code></td>
      <td style="border: 1px solid #ddd; padding: 8px;">docs:</td>
      <td style="border: 1px solid #ddd; padding: 8px;">add lean ux canvas section</td>
      <td style="border: 1px solid #ddd; padding: 8px;">12/04/2026</td>
    </tr>
    <tr>
      <td style="border: 1px solid #ddd; padding: 8px;"><code>InnovaTechStudio/AutoService-730-AW</code></td>
      <td style="border: 1px solid #ddd; padding: 8px;"><code>feature/chapter-2-needfinding</code></td>
      <td style="border: 1px solid #ddd; padding: 8px;"><code>0fde76b</code></td>
      <td style="border: 1px solid #ddd; padding: 8px;">docs:</td>
      <td style="border: 1px solid #ddd; padding: 8px;">reorganize interview sections into design and record structure</td>
      <td style="border: 1px solid #ddd; padding: 8px;">13/04/2026</td>
    </tr>
    <tr>
      <td style="border: 1px solid #ddd; padding: 8px;"><code>InnovaTechStudio/AutoService-730-AW</code></td>
      <td style="border: 1px solid #ddd; padding: 8px;"><code>feature/chapter5.1-software-configuration-management</code></td>
      <td style="border: 1px solid #ddd; padding: 8px;"><code>cf04690</code></td>
      <td style="border: 1px solid #ddd; padding: 8px;">docs:</td>
      <td style="border: 1px solid #ddd; padding: 8px;">add software deployment configuration to software configuration management</td>
      <td style="border: 1px solid #ddd; padding: 8px;">13/04/2026</td>
    </tr>
    <tr>
      <td style="border: 1px solid #ddd; padding: 8px;"><code>InnovaTechStudio/AutoService-730-AW</code></td>
      <td style="border: 1px solid #ddd; padding: 8px;"><code>feature/chapter-2-interview-structure</code></td>
      <td style="border: 1px solid #ddd; padding: 8px;"><code>c8b28d0</code></td>
      <td style="border: 1px solid #ddd; padding: 8px;">docs:</td>
      <td style="border: 1px solid #ddd; padding: 8px;">add interview record-1</td>
      <td style="border: 1px solid #ddd; padding: 8px;">14/04/2026</td>
    </tr>
    <tr>
      <td style="border: 1px solid #ddd; padding: 8px;"><code>InnovaTechStudio/AutoService-730-AW</code></td>
      <td style="border: 1px solid #ddd; padding: 8px;"><code>feature/information-architecture-and-ddd</code></td>
      <td style="border: 1px solid #ddd; padding: 8px;"><code>b1cad74</code></td>
      <td style="border: 1px solid #ddd; padding: 8px;">docs:</td>
      <td style="border: 1px solid #ddd; padding: 8px;">add c4 diagrams to the ddd section</td>
      <td style="border: 1px solid #ddd; padding: 8px;">16/04/2026</td>
    </tr>
    <tr>
      <td style="border: 1px solid #ddd; padding: 8px;"><code>InnovaTechStudio/AutoService-730-AW</code></td>
      <td style="border: 1px solid #ddd; padding: 8px;"><code>feature/chapter-4/design-UX/UI</code></td>
      <td style="border: 1px solid #ddd; padding: 8px;"><code>4adbeb7</code></td>
      <td style="border: 1px solid #ddd; padding: 8px;">docs:</td>
      <td style="border: 1px solid #ddd; padding: 8px;">add wireflow diagram</td>
      <td style="border: 1px solid #ddd; padding: 8px;">19/04/2026</td>
    </tr>
    <tr>
      <td style="border: 1px solid #ddd; padding: 8px;"><code>InnovaTechStudio/AutoService-730-AW</code></td>
      <td style="border: 1px solid #ddd; padding: 8px;"><code>feature/chapter-4-design-diagrams</code></td>
      <td style="border: 1px solid #ddd; padding: 8px;"><code>47ecbf9</code></td>
      <td style="border: 1px solid #ddd; padding: 8px;">docs:</td>
      <td style="border: 1px solid #ddd; padding: 8px;">add database design diagrams for Chapter 4</td>
      <td style="border: 1px solid #ddd; padding: 8px;">19/04/2026</td>
    </tr>
    <tr>
      <td style="border: 1px solid #ddd; padding: 8px;"><code>InnovaTechStudio/AutoService-730-AW</code></td>
      <td style="border: 1px solid #ddd; padding: 8px;"><code>feature/landing-page-wireframe</code></td>
      <td style="border: 1px solid #ddd; padding: 8px;"><code>2d08360</code></td>
      <td style="border: 1px solid #ddd; padding: 8px;">docs:</td>
      <td style="border: 1px solid #ddd; padding: 8px;">add pricing section to landing page wireframe</td>
      <td style="border: 1px solid #ddd; padding: 8px;">20/04/2026</td>
    </tr>
    <tr>
      <td style="border: 1px solid #ddd; padding: 8px;"><code>InnovaTechStudio/AutoService-landing</code></td>
      <td style="border: 1px solid #ddd; padding: 8px;"><code>feature/landing-base</code></td>
      <td style="border: 1px solid #ddd; padding: 8px;"><code>5c2cdfa</code></td>
      <td style="border: 1px solid #ddd; padding: 8px;">feat:</td>
      <td style="border: 1px solid #ddd; padding: 8px;">redesign landing page visual system</td>
      <td style="border: 1px solid #ddd; padding: 8px;">19/04/2026</td>
    </tr>
  </tbody>
</table>

##### 5.2.1.5. Execution Evidence for Sprint Review

<p align="justify">
En esta sección se presenta la evidencia de la ejecución del producto lograda durante el Sprint 1. El resultado principal de esta iteración es la primera versión funcional de la Landing Page de AutoService, desarrollada con HTML5, CSS3 y JavaScript. Esta interfaz presenta de forma clara el modelo de negocio, las herramientas principales de la plataforma y los planes de suscripción disponibles. Se ha verificado que la navegación interactiva (scroll suave y menú hamburguesa) sea fluida y que el diseño sea completamente adaptable (responsive web design) para garantizar una correcta experiencia de usuario tanto en navegadores de escritorio como en dispositivos móviles.
</p>

<div align="center">
  <h5>Vista Principal de la Landing Page (Hero Section y Navegación)</h5>
  <img src="docs/assets/chapter-5/landing_ss_1.png" alt="Landing Page Hero Section" width="80%">
  
  <h5>Sección de Características y Planes de Suscripción</h5>
  <img src="docs/assets/chapter-5/landing_ss_2.png" alt="Landing Page Pricing y Features" width="80%">

  <h5>Video de presentación y ejecución de la Landing Page</h5>
  <img src="docs/assets/chapter-5/landing_execution.png" alt="Landing Page Pricing y Features" width="80%">
  
</div>

<p align="justify">
Para ilustrar la visualización y las interacciones logradas en este Sprint, se adjunta el enlace a un video demostrativo. En este registro se evidencia el funcionamiento de los componentes clave, la adaptabilidad del diseño en distintas resoluciones y la coherencia visual con los lineamientos de UI establecidos en el Capítulo IV del proyecto. 
</p>

URL video de ejecución de la Landing Page: <code>https://upcedupe-my.sharepoint.com/personal/u202421866_upc_edu_pe/_layouts/15/stream.aspx?id=%2Fpersonal%2Fu202421866%5Fupc%5Fedu%5Fpe%2FDocuments%2Flanding%2Devidence%2Emp4&nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJPbmVEcml2ZUZvckJ1c2luZXNzIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXciLCJyZWZlcnJhbFZpZXciOiJNeUZpbGVzTGlua0NvcHkifX0&ga=1&referrer=StreamWebApp%2EWeb&referrerScenario=AddressBarCopied%2Eview%2E1a416f63%2D5442%2D4400%2Db740%2D7fb6621fa42f</code>.

---

##### 5.2.1.6. Services Documentation Evidence for Sprint Review

<p align="justify">
Durante el Sprint 1, la implementación del contenedor central <b>API RESTful</b> (Backend) de AutoService fue programada estratégicamente para el siguiente sprint. Sin embargo, como parte del alcance funcional y técnico de este primer entregable, se integró y documentó el uso de un Web Service de terceros para habilitar la interactividad de la Landing Page.
</p>

<p align="justify">
Se implementó <b>EmailJS</b>, un servicio basado en la nube que permite el envío de correos electrónicos transaccionales mediante peticiones HTTP directamente desde el cliente (Client-side). Esto permite conectar el formulario de contacto de la Landing Page con la bandeja de entrada del equipo, asegurando la comunicación inmediata sin necesidad de desplegar un servidor intermedio.
</p>

<table style="width: 100%; border-collapse: collapse; text-align: justify; margin-bottom: 1.5em;">
  <thead>
    <tr style="background-color: #f2f2f2;">
      <th style="border: 1px solid #ddd; padding: 8px; text-align: center;">Servicio (Endpoint)</th>
      <th style="border: 1px solid #ddd; padding: 8px; text-align: center;">Método</th>
      <th style="border: 1px solid #ddd; padding: 8px; text-align: center;">Descripción</th>
      <th style="border: 1px solid #ddd; padding: 8px; text-align: center;">Payload / Parámetros</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td style="border: 1px solid #ddd; padding: 8px; text-align: center;"><code>https://api.emailjs.com/api/v1.0/email/send</code></td>
      <td style="border: 1px solid #ddd; padding: 8px; text-align: center;"><strong>POST</strong></td>
      <td style="border: 1px solid #ddd; padding: 8px;">Procesa y envía los datos del formulario de contacto hacia el correo electrónico configurado por el equipo.</td>
      <td style="border: 1px solid #ddd; padding: 8px;"><code>service_id</code>, <code>template_id</code>, <code>user_id</code> (Public Key), <code>template_params</code> (nombre, email, mensaje)</td>
    </tr>
  </tbody>
</table>

<p align="justify">
A continuación, se adjunta la evidencia visual de la configuración de este servicio y la interacción exitosa utilizando datos de muestra enviados desde el formulario en producción:
</p>

<div align="center">
  <h5 style="margin-bottom: 0.5em;">Evidencia 1: Configuración del Servicio y Template en EmailJS</h5>
  <img src="docs/assets/chapter-5/emailjs_config.png" alt="EmailJS Dashboard Configuration" width="80%" style="margin-bottom: 1.5em;">
  
  <h5 style="margin-bottom: 0.5em;">Evidencia 2: Interacción exitosa (Correo de prueba recibido)</h5>
  <img src="docs/assets/chapter-5/emailjs_example.png" alt="EmailJS Received Email" width="80%">
</div>

---

##### 5.2.1.7. Software Deployment Evidence for Sprint Review

<p align="justify">
En esta sección se detallan los procesos realizados para el despliegue de la solución durante el Sprint 1. El objetivo principal fue poner en producción la versión inicial de la Landing Page, permitiendo que el modelo de negocio de AutoService sea accesible para los interesados y potenciales clientes desde cualquier navegador.
</p>

<p align="justify">
Para el despliegue, se utilizó <b>GitHub Pages</b>, aprovechando su integración nativa con el repositorio de código fuente. El proceso consistió en los siguientes pasos estratégicos:
</p>

<ol style="text-align: justify;">
  <li><strong>Configuración del Entorno:</strong> Se configuró el repositorio específico para la Landing Page, asegurando que el archivo <code>index.html</code> se encuentre en la raíz para su correcto reconocimiento.</li>
  <li><strong>Activación del Servicio:</strong> Se habilitó GitHub Pages desde los ajustes del repositorio, seleccionando la rama <code>main</code> como fuente de despliegue.</li>
  <li><strong>Automatización (CI/CD):</strong> Se validó el flujo de trabajo automático mediante GitHub Actions, el cual dispara un nuevo despliegue cada vez que se realiza un merge a la rama principal.</li>
</ol>

<div align="center">

  <h5>Evidencia 1: Configuración de GitHub Pages en el Repositorio</h5>
    <img src="docs/assets/chapter-5/pages_settings.png" alt="GitHub Pages Settings" width="80%">
  <h5>Evidencia 2: Workflow para la Landing Page</h5>
    <img src="docs/assets/chapter-5/landing_pulse.png" alt="GitHub Actions Workflow" width="80%">
  <h5>Evidencia 3: Visualización de la Landing Page en Producción</h5>
    <img src="docs/assets/chapter-5/landing_ss_1.png" alt="Live Landing Page" width="80%">

</div><p align="justify">

La Landing Page se encuentra actualmente operativa en la siguiente URL: <code>https://innovatechstudio.github.io/Autoservice-landing-page/</code>.
</p>

---

##### 5.2.1.8. Team Collaboration Insights during Sprint

<p align="justify">
Durante el Sprint 1, el equipo mantuvo un flujo de trabajo altamente colaborativo y organizado, aplicando estrictamente la estrategia de control de versiones GitFlow. Para asegurar la calidad y revisión por pares, todo el desarrollo de la arquitectura, investigación de UX/UI y codificación de la Landing Page se trabajó en ramas independientes (<i>feature branches</i>). La integración del trabajo se realizó exclusivamente mediante <b>Pull Requests</b> hacia la rama <code>develop</code>, lo que fomentó la comunicación y revisión conjunta antes de consolidar los avances.
</p>

<p align="justify">
A continuación, se presentan los analíticos extraídos de GitHub (Insights) que evidencian la participación equitativa y constante de todos los miembros del equipo (<i>Aspect Leaders</i> y <i>Collaborators</i>) tanto en el repositorio principal de documentación como en el de la Landing Page.
</p>

<div align="center">
  <h5>Evidencia 1: Gráfico de Contribuciones por Miembro del Equipo</h5>
  <img src="docs/assets/chapter-5/contributors.png" alt="GitHub Contributors Graph" width="80%">
  
  <h5>Evidencia 2: Resumen de Actividad del Sprint (GitHub Pulse)</h5>
  <img src="docs/assets/chapter-5/pulse.png" alt="GitHub Pulse Activity" width="80%">

  <h5>Evidencia 3: Gestión Colaborativa mediante Pull Requests</h5>
  <img src="docs/assets/chapter-5/closed_pr.png" alt="GitHub Closed Pull Requests" width="80%">
</div>

<p align="justify">
Como demuestran las gráficas y el resumen de actividad, la carga de trabajo se distribuyó de manera eficiente, logrando que el 100% de los integrantes registre commits significativos (alineados a <i>Conventional Commits</i>), gestione integraciones (Merges) y participe activamente en las fases de análisis, diseño e implementación temprana del producto.
</p>

#### 5.2.2. Sprint 2

##### 5.2.2.1. Sprint Planning 2

<div align="center">
  <table style="margin: auto; width: 100%; border-collapse: collapse; text-align: left;">
    <thead>
      <tr>
        <th colspan="2" style="text-align: center; background-color: #f2f2f2; font-size: 1.2em; padding: 10px; border: 1px solid #ddd;">Sprint #2</th>
      </tr>
    </thead>
    <tbody>
      <tr>
        <td colspan="2" style="background-color: #fafafa; font-weight: bold; text-align: center; padding: 10px; border: 1px solid #ddd;">Sprint Planning Background</td>
      </tr>
      <tr>
        <td style="width: 30%; font-weight: bold; padding: 10px; border: 1px solid #ddd;">Date</td>
        <td style="padding: 10px; border: 1px solid #ddd;">2026-04-29</td>
      </tr>
      <tr>
        <td style="font-weight: bold; padding: 10px; border: 1px solid #ddd;">Time</td>
        <td style="padding: 10px; border: 1px solid #ddd;">10:00 AM</td>
      </tr>
      <tr>
        <td style="font-weight: bold; padding: 10px; border: 1px solid #ddd;">Location</td>
        <td style="padding: 10px; border: 1px solid #ddd;">Reunión presencial en la UPC. (Pabellón I, piso 5, cubículo 4)</td>
      </tr>
      <tr>
        <td style="font-weight: bold; padding: 10px; border: 1px solid #ddd;">Prepared By</td>
        <td style="padding: 10px; border: 1px solid #ddd;">Mamani Vilca, Alan Jaivi</td>
      </tr>
      <tr>
        <td style="font-weight: bold; padding: 10px; border: 1px solid #ddd;">Attendees (to planning meeting)</td>
        <td style="padding: 10px; border: 1px solid #ddd;">
          Pillaca Gonzales, Andy Saúl / López Monroy, Rodrigo Alfredo / Luis Miranda, Diego Andres / Mamani Vilca, Alan Jaivi / Sanchez Cuadrado, Juan Antonio
        </td>
      </tr>
      <tr>
        <td style="font-weight: bold; padding: 10px; border: 1px solid #ddd;">Sprint 1 Review Summary</td>
        <td style="padding: 10px; border: 1px solid #ddd;">
          Durante el Sprint 1, el equipo logró desplegar exitosamente la Landing Page oficial de AutoService, además de completar la documentación técnica relacionada con la arquitectura del sistema, diagramas C4 y diseño de base de datos. También se configuró el flujo de trabajo colaborativo utilizando GitHub, GitFlow y GitHub Pages para el despliegue continuo del producto.
        </td>
      </tr>
      <tr>
        <td style="font-weight: bold; padding: 10px; border: 1px solid #ddd;">Sprint 1 Retrospective Summary</td>
        <td style="padding: 10px; border: 1px solid #ddd;">
          El equipo identificó como principal fortaleza la correcta distribución de tareas y la integración continua mediante Pull Requests. Asimismo, se acordó mejorar la coordinación entre frontend y backend para las siguientes iteraciones, priorizando la definición temprana de contratos de datos y estructuras de consumo de APIs para reducir retrabajos e inconsistencias.
        </td>
      </tr>
      <tr>
        <td colspan="2" style="background-color: #fafafa; font-weight: bold; text-align: center; padding: 10px; border: 1px solid #ddd;">Sprint Goal & User Stories</td>
      </tr>
      <tr>
        <td style="font-weight: bold; padding: 10px; border: 1px solid #ddd;">Sprint 2 Goal</td>
        <td style="padding: 10px; border: 1px solid #ddd;">
          <strong>Our focus is on</strong> developing the first functional version of the AutoService frontend application connected to a Fake API environment.<br><br>
          <strong>We believe it delivers</strong> an interactive and testable prototype that allows administrators and customers to interact with vehicle tracking, work orders and authentication functionalities before integrating the final backend services.<br><br>
          <strong>This will be confirmed when</strong> the frontend application successfully consumes mock API endpoints, displays dynamic information correctly, and allows navigation between the main modules of the system with responsive behavior.
        </td>
      </tr>
      <tr>
        <td style="font-weight: bold; padding: 10px; border: 1px solid #ddd;">Sprint 2 Velocity</td>
        <td style="padding: 10px; border: 1px solid #ddd;">36 Story Points</td>
      </tr>
      <tr>
        <td style="font-weight: bold; padding: 10px; border: 1px solid #ddd;">Sum of Story Points</td>
        <td style="padding: 10px; border: 1px solid #ddd;">
          36 Story Points (US-05: 5, US-06: 5, US-07: 1, US-08: 3, US-09: 5, US-10: 2, US-23: 3, US-24: 3, TS-02: 5, TS-03: 3, TS-08: 3, TS-09: 3).
        </td>
      </tr>
    </tbody>
  </table>
</div>

##### 5.2.2.2. Aspect Leaders and Collaborators

En el presente Sprint 2, el alcance funcional y técnico se ha dividido en tres aspectos principales para garantizar una entrega eficiente:
1. Frontend Development: Desarrollo de las principales interfaces y componentes del sistema.
2. Fake API Development: Implementación y configuración de la Fake API para pruebas e integración.
3. Frontend Deployment: Configuración y despliegue del frontend en un entorno accesible públicamente.

<div align="center">
  <table style="margin: auto; width: 100%; border-collapse: collapse; text-align: center;">
    <thead>
      <tr style="background-color: #f2f2f2;">
        <th style="padding: 10px; border: 1px solid #ddd; text-align: left;">Team Member (Last Name, First Name)</th>
        <th style="padding: 10px; border: 1px solid #ddd;">GitHub Username</th>
        <th style="padding: 10px; border: 1px solid #ddd;">Frontend Development<br><small>Leader (L) / Collaborator (C)</small></th>
        <th style="padding: 10px; border: 1px solid #ddd;">Fake API Development<br><small>Leader (L) / Collaborator (C)</small></th>
        <th style="padding: 10px; border: 1px solid #ddd;">Frontend Deployment<br><small>Leader (L) / Collaborator (C)</small></th>
      </tr>
    </thead>
    <tbody>
      <tr>
        <td style="padding: 10px; border: 1px solid #ddd; text-align: left;">Aguilar Aguayo, Pillaca Gonzales, Andy Saúl</td>
        <td style="padding: 10px; border: 1px solid #ddd;">apillacag</td>
        <td style="padding: 10px; border: 1px solid #ddd; color: #1976d2;">C</td>
        <td style="padding: 10px; border: 1px solid #ddd; font-weight: bold; color: #1976d2;">C</td>
        <td style="padding: 10px; border: 1px solid #ddd; color: #1976d2;">C</td>
      </tr>
      <tr>
        <td style="padding: 10px; border: 1px solid #ddd; text-align: left;">López Monroy, Rodrigo Alfredo</td>
        <td style="padding: 10px; border: 1px solid #ddd;">rodrigolopezu</td>
        <td style="padding: 10px; border: 1px solid #ddd; font-weight: bold; color: #2e7d32;">L</td>
        <td style="padding: 10px; border: 1px solid #ddd; color: #1976d2;">C</td>
        <td style="padding: 10px; border: 1px solid #ddd; font-weight: bold; color: #2e7d32;">L</td>
      </tr>
      <tr>
        <td style="padding: 10px; border: 1px solid #ddd; text-align: left;">Luis Miranda, Diego Andres</td>
        <td style="padding: 10px; border: 1px solid #ddd;">andrewdmr</td>
        <td style="padding: 10px; border: 1px solid #ddd; font-weight: bold; color: #2e7d32;">L</td>
        <td style="padding: 10px; border: 1px solid #ddd; color: #1976d2;">C</td>
        <td style="padding: 10px; border: 1px solid #ddd; color: #1976d2;">C</td>
      </tr>
      <tr>
        <td style="padding: 10px; border: 1px solid #ddd; text-align: left;">Mamani Vilca, Alan Jaivi</td>
        <td style="padding: 10px; border: 1px solid #ddd;">alanmamaniv</td>
        <td style="padding: 10px; border: 1px solid #ddd; color: #1976d2;">C</td>
        <td style="padding: 10px; border: 1px solid #ddd; font-weight: bold; color: #2e7d32;">L</td>
        <td style="padding: 10px; border: 1px solid #ddd; color: #1976d2;">C</td>
      </tr>
      <tr>
        <td style="padding: 10px; border: 1px solid #ddd; text-align: left;">Sanchez Cuadrado, Juan Antonio</td>
        <td style="padding: 10px; border: 1px solid #ddd;">juanasc05</td>
        <td style="padding: 10px; border: 1px solid #ddd; color: #1976d2;">C</td>
        <td style="padding: 10px; border: 1px solid #ddd; color: #2e7d32;">L</td>
        <td style="padding: 10px; border: 1px solid #ddd; color: #1976d2;">C</td>
      </tr>
    </tbody>
  </table>
</div>

##### 5.2.2.3. Sprint Backlog 2

El presente Sprint Backlog detalla la descomposición técnica de las historias de usuario seleccionadas para la segunda iteración del proyecto. El objetivo principal de este Sprint es desarrollar la primera versión funcional del Frontend, integrarlo con una Fake API y desplegar la aplicación para pruebas funcionales y validación temprana. A continuación, se presenta la captura de nuestro tablero en Jira Software, seguida de la tabla de control de estado con la distribución de los Work-Items.

<div align="center">
  <table style="margin: auto; width: 100%; border-collapse: collapse; text-align: left; font-size: 13px; border: 1px solid #ddd;">
    <thead>
      <tr style="background-color: #e0e0e0; font-weight: bold;">
        <th style="padding: 10px; text-align: center; border: 1px solid #ddd;">Sprint #</th>
        <th colspan="7" style="padding: 10px; text-align: left; border: 1px solid #ddd;">2</th>
      </tr>
      <tr style="background-color: #f2f2f2;">
        <th colspan="2" style="text-align: center; border: 1px solid #ddd; padding: 10px;">User Story</th>
        <th colspan="6" style="text-align: center; border: 1px solid #ddd; padding: 10px;">Work-Item / Task</th>
      </tr>
      <tr style="background-color: #fafafa; text-align: center;">
        <th style="border: 1px solid #ddd; padding: 5px; width: 6%;">Id</th>
        <th style="border: 1px solid #ddd; padding: 5px; width: 15%;">Title</th>
        <th style="border: 1px solid #ddd; padding: 5px; width: 6%;">Id</th>
        <th style="border: 1px solid #ddd; padding: 5px; width: 15%;">Title</th>
        <th style="border: 1px solid #ddd; padding: 5px; width: 30%;">Description</th>
        <th style="border: 1px solid #ddd; padding: 5px; width: 8%;">Estimation (Hours)</th>
        <th style="border: 1px solid #ddd; padding: 5px; width: 12%;">Assigned To</th>
        <th style="border: 1px solid #ddd; padding: 5px; width: 8%;">Status</th>
      </tr>
    </thead>
    <tbody>
      <tr>
        <td rowspan="2" style="border: 1px solid #ddd; padding: 8px; text-align: center; font-weight: bold;">US-08</td>
        <td rowspan="2" style="border: 1px solid #ddd; padding: 8px;">Registrar vehículo</td>
        <td style="border: 1px solid #ddd; padding: 8px; text-align: center;">WI-18</td>
        <td style="border: 1px solid #ddd; padding: 8px;">Formulario de registro</td>
        <td style="border: 1px solid #ddd; padding: 8px;"><i>Implementar formulario para registrar vehículos en el sistema.</i></td>
        <td style="border: 1px solid #ddd; padding: 8px; text-align: center;">5</td>
        <td style="border: 1px solid #ddd; padding: 8px;">Luis, Diego</td>
        <td style="border: 1px solid #ddd; padding: 8px; text-align: center; color: #2aac2a; font-weight: bold;">Done</td>
      </tr>
      <tr>
        <td style="border: 1px solid #ddd; padding: 8px; text-align: center;">WI-19</td>
        <td style="border: 1px solid #ddd; padding: 8px;">Persistencia Fake API</td>
        <td style="border: 1px solid #ddd; padding: 8px;"><i>Conectar formulario de registro con endpoints simulados.</i></td>
        <td style="border: 1px solid #ddd; padding: 8px; text-align: center;">4</td>
        <td style="border: 1px solid #ddd; padding: 8px;">Mamani, Alan</td>
        <td style="border: 1px solid #ddd; padding: 8px; text-align: center; color: #2aac2a; font-weight: bold;">Done</td>
      </tr>
      <tr>
        <td rowspan="2" style="border: 1px solid #ddd; padding: 8px; text-align: center; font-weight: bold;">US-09</td>
        <td rowspan="2" style="border: 1px solid #ddd; padding: 8px;">Crear orden de trabajo</td>
        <td style="border: 1px solid #ddd; padding: 8px; text-align: center;">WI-20</td>
        <td style="border: 1px solid #ddd; padding: 8px;">Vista de órdenes</td>
        <td style="border: 1px solid #ddd; padding: 8px;"><i>Desarrollar interfaz para creación de órdenes de trabajo.</i></td>
        <td style="border: 1px solid #ddd; padding: 8px;">6</td>
        <td style="border: 1px solid #ddd; padding: 8px;">Aguilar, Andy Saúl</td>
        <td style="border: 1px solid #ddd; padding: 8px; text-align: center; color: #2aac2a; font-weight: bold;">Done</td>
      </tr>
      <tr>
        <td style="border: 1px solid #ddd; padding: 8px; text-align: center;">WI-21</td>
        <td style="border: 1px solid #ddd; padding: 8px;">Servicio de órdenes</td>
        <td style="border: 1px solid #ddd; padding: 8px;"><i>Implementar lógica de comunicación con Fake API.</i></td>
        <td style="border: 1px solid #ddd; padding: 8px;">5</td>
        <td style="border: 1px solid #ddd; padding: 8px;">López, Rodrigo</td>
        <td style="border: 1px solid #ddd; padding: 8px; text-align: center; color: #2aac2a; font-weight: bold;">Done</td>
      </tr>
      <tr>
        <td rowspan="2" style="border: 1px solid #ddd; padding: 8px; text-align: center; font-weight: bold;">US-10</td>
        <td rowspan="2" style="border: 1px solid #ddd; padding: 8px;">Visualizar vehículos en el taller</td>
        <td style="border: 1px solid #ddd; padding: 8px; text-align: center;">WI-22</td>
        <td style="border: 1px solid #ddd; padding: 8px;">Tabla de vehículos</td>
        <td style="border: 1px solid #ddd; padding: 8px;"><i>Mostrar listado dinámico de vehículos activos.</i></td>
        <td style="border: 1px solid #ddd; padding: 8px;">4</td>
        <td style="border: 1px solid #ddd; padding: 8px;">Luis, Diego</td>
        <td style="border: 1px solid #ddd; padding: 8px; text-align: center; color: #2aac2a; font-weight: bold;">Done</td>
      </tr>
      <tr>
        <td style="border: 1px solid #ddd; padding: 8px; text-align: center;">WI-23</td>
        <td style="border: 1px solid #ddd; padding: 8px;">Consumo de datos</td>
        <td style="border: 1px solid #ddd; padding: 8px;"><i>Consumir información desde JSON Server.</i></td>
        <td style="border: 1px solid #ddd; padding: 8px;">3</td>
        <td style="border: 1px solid #ddd; padding: 8px;">Sanchez, Juan</td>
        <td style="border: 1px solid #ddd; padding: 8px; text-align: center; color: #2aac2a; font-weight: bold;">Done</td>
      </tr>
      <tr>
        <td rowspan="2" style="border: 1px solid #ddd; padding: 8px; text-align: center; font-weight: bold;">US-23</td>
        <td rowspan="2" style="border: 1px solid #ddd; padding: 8px;">Ingresar código de seguimiento</td>
        <td style="border: 1px solid #ddd; padding: 8px; text-align: center;">WI-24</td>
        <td style="border: 1px solid #ddd; padding: 8px;">Pantalla de tracking</td>
        <td style="border: 1px solid #ddd; padding: 8px;"><i>Crear vista para ingreso de código de seguimiento.</i></td>
        <td style="border: 1px solid #ddd; padding: 8px;">4</td>
        <td style="border: 1px solid #ddd; padding: 8px;">Aguilar, Andy Saúl</td>
        <td style="border: 1px solid #ddd; padding: 8px; text-align: center; color: #2aac2a; font-weight: bold;">Done</td>
      </tr>
      <tr>
        <td style="border: 1px solid #ddd; padding: 8px; text-align: center;">WI-25</td>
        <td style="border: 1px solid #ddd; padding: 8px;">Validación de código</td>
        <td style="border: 1px solid #ddd; padding: 8px;"><i>Implementar validación básica de búsqueda de órdenes.</i></td>
        <td style="border: 1px solid #ddd; padding: 8px;">2</td>
        <td style="border: 1px solid #ddd; padding: 8px;">Mamani, Alan</td>
        <td style="border: 1px solid #ddd; padding: 8px; text-align: center; color: #2aac2a; font-weight: bold;">Done</td>
      </tr>
      <tr>
        <td rowspan="2" style="border: 1px solid #ddd; padding: 8px; text-align: center; font-weight: bold;">US-24</td>
        <td rowspan="2" style="border: 1px solid #ddd; padding: 8px;">Visualizar estado del vehículo</td>
        <td style="border: 1px solid #ddd; padding: 8px; text-align: center;">WI-26</td>
        <td style="border: 1px solid #ddd; padding: 8px;">Vista estado del vehículo</td>
        <td style="border: 1px solid #ddd; padding: 8px;"><i>Mostrar estado actual y progreso del servicio.</i></td>
        <td style="border: 1px solid #ddd; padding: 8px;">5</td>
        <td style="border: 1px solid #ddd; padding: 8px;">Luis, Diego</td>
        <td style="border: 1px solid #ddd; padding: 8px; text-align: center; color: #2aac2a; font-weight: bold;">Done</td>
      </tr>
      <tr>
        <td style="border: 1px solid #ddd; padding: 8px; text-align: center;">WI-27</td>
        <td style="border: 1px solid #ddd; padding: 8px;">Integración tracking API</td>
        <td style="border: 1px solid #ddd; padding: 8px;"><i>Conectar datos de seguimiento con Fake API.</i></td>
        <td style="border: 1px solid #ddd; padding: 8px;">4</td>
        <td style="border: 1px solid #ddd; padding: 8px;">López, Rodrigo</td>
        <td style="border: 1px solid #ddd; padding: 8px; text-align: center; color: #2aac2a; font-weight: bold;">Done</td>
      </tr>
      <tr>
        <td rowspan="2" style="border: 1px solid #ddd; padding: 8px; text-align: center; font-weight: bold;">TS-02</td>
        <td rowspan="2" style="border: 1px solid #ddd; padding: 8px;">Implementar API REST</td>
        <td style="border: 1px solid #ddd; padding: 8px; text-align: center;">WI-28</td>
        <td style="border: 1px solid #ddd; padding: 8px;">Configuración JSON Server</td>
        <td style="border: 1px solid #ddd; padding: 8px;"><i>Levantar servidor Fake API para pruebas del frontend.</i></td>
        <td style="border: 1px solid #ddd; padding: 8px;">3</td>
        <td style="border: 1px solid #ddd; padding: 8px;">Mamani, Alan</td>
        <td style="border: 1px solid #ddd; padding: 8px; text-align: center; color: #2aac2a; font-weight: bold;">Done</td>
      </tr>
      <tr>
        <td style="border: 1px solid #ddd; padding: 8px; text-align: center;">WI-29</td>
        <td style="border: 1px solid #ddd; padding: 8px;">Definición de endpoints</td>
        <td style="border: 1px solid #ddd; padding: 8px;"><i>Definir rutas y recursos necesarios para el sistema.</i></td>
        <td style="border: 1px solid #ddd; padding: 8px;">4</td>
        <td style="border: 1px solid #ddd; padding: 8px;">Sanchez, Juan</td>
        <td style="border: 1px solid #ddd; padding: 8px; text-align: center; color: #2aac2a; font-weight: bold;">Done</td>
      </tr>
      <tr>
        <td rowspan="2" style="border: 1px solid #ddd; padding: 8px; text-align: center; font-weight: bold;">TS-11</td>
        <td rowspan="2" style="border: 1px solid #ddd; padding: 8px;">Desplegar aplicación</td>
        <td style="border: 1px solid #ddd; padding: 8px; text-align: center;">WI-30</td>
        <td style="border: 1px solid #ddd; padding: 8px;">Deploy frontend</td>
        <td style="border: 1px solid #ddd; padding: 8px;"><i>Publicar el frontend en entorno cloud para pruebas.</i></td>
        <td style="border: 1px solid #ddd; padding: 8px;">4</td>
        <td style="border: 1px solid #ddd; padding: 8px;">López, Rodrigo</td>
        <td style="border: 1px solid #ddd; padding: 8px; text-align: center; color: #2aac2a; font-weight: bold;">Done</td>
      </tr>
      <tr>
        <td style="border: 1px solid #ddd; padding: 8px; text-align: center;">WI-31</td>
        <td style="border: 1px solid #ddd; padding: 8px;">Validación de despliegue</td>
        <td style="border: 1px solid #ddd; padding: 8px;"><i>Realizar pruebas funcionales sobre el entorno desplegado.</i></td>
        <td style="border: 1px solid #ddd; padding: 8px;">2</td>
        <td style="border: 1px solid #ddd; padding: 8px;">Aguilar, Andy Saúl</td>
        <td style="border: 1px solid #ddd; padding: 8px; text-align: center; color: #2aac2a; font-weight: bold;">Done</td>
      </tr>
    </tbody>
  </table>
</div>

##### 5.2.2.4. Development Evidence for Sprint Review

<p align="justify">
Durante el Sprint 2, el equipo se enfocó en la implementación funcional de la Web Application utilizando Angular y TypeScript, integrando nuevas vistas, componentes y funcionalidades relacionadas con la gestión operativa del taller automotriz. Asimismo, se consolidó la arquitectura frontend mediante la implementación de internacionalización (i18n), mejoras de UI/UX, refactorización de módulos y la integración de flujos completos como vehículos, órdenes de trabajo, mecánicos y tracking de clientes.<br><br>

Entre los principales avances del sprint se encuentran la implementación de i18n en múltiples módulos, el rediseño del dashboard administrativo, mejoras en la gestión de vehículos y órdenes de trabajo, así como la integración de flujos de seguimiento de clientes y pagos. Además, se realizaron tareas de mejora de experiencia de usuario, optimización de componentes y soporte para vistas responsivas.<br><br>

En la siguiente tabla se presentan commits que representan hitos clave del desarrollo de este sprint:
</p>

<table style="width: 100%; border-collapse: collapse; text-align: justify;">
  <thead>
    <tr style="background-color: #f2f2f2;">
      <th style="border: 1px solid #ddd; padding: 8px;">Repository</th>
      <th style="border: 1px solid #ddd; padding: 8px;">Branch</th>
      <th style="border: 1px solid #ddd; padding: 8px;">Commit Id</th>
      <th style="border: 1px solid #ddd; padding: 8px;">Commit Message</th>
      <th style="border: 1px solid #ddd; padding: 8px;">Commit Message Body</th>
      <th style="border: 1px solid #ddd; padding: 8px;">Committed on (Date)</th>
    </tr>
  </thead>

  <tbody>
    <tr>
      <td style="border: 1px solid #ddd; padding: 8px;">
        <code>InnovaTechStudio/AutoService-730-AW-Frontend</code>
      </td>
      <td style="border: 1px solid #ddd; padding: 8px;">
        <code>develop</code>
      </td>
      <td style="border: 1px solid #ddd; padding: 8px;">
        <code>c118649</code>
      </td>
      <td style="border: 1px solid #ddd; padding: 8px;">feat:</td>
      <td style="border: 1px solid #ddd; padding: 8px;">import i18n in main.js</td>
      <td style="border: 1px solid #ddd; padding: 8px;">11/05/2026</td>
    </tr>
    <tr>
      <td style="border: 1px solid #ddd; padding: 8px;"><code>InnovaTechStudio/AutoService-730-AW-Frontend</code></td>
      <td style="border: 1px solid #ddd; padding: 8px;"><code>develop</code></td>
      <td style="border: 1px solid #ddd; padding: 8px;"><code>0dbf840</code></td>
      <td style="border: 1px solid #ddd; padding: 8px;">feat:</td>
      <td style="border: 1px solid #ddd; padding: 8px;">add internationalization to login view</td>
      <td style="border: 1px solid #ddd; padding: 8px;">11/05/2026</td>
    </tr>
    <tr>
      <td style="border: 1px solid #ddd; padding: 8px;"><code>InnovaTechStudio/AutoService-730-AW-Frontend</code></td>
      <td style="border: 1px solid #ddd; padding: 8px;"><code>develop</code></td>
      <td style="border: 1px solid #ddd; padding: 8px;"><code>de49f9e</code></td>
      <td style="border: 1px solid #ddd; padding: 8px;">feat:</td>
      <td style="border: 1px solid #ddd; padding: 8px;">add internationalization to mechanics view</td>
      <td style="border: 1px solid #ddd; padding: 8px;">11/05/2026</td>
    </tr>
    <tr>
      <td style="border: 1px solid #ddd; padding: 8px;"><code>InnovaTechStudio/AutoService-730-AW-Frontend</code></td>
      <td style="border: 1px solid #ddd; padding: 8px;"><code>develop</code></td>
      <td style="border: 1px solid #ddd; padding: 8px;"><code>d1b0d5c</code></td>
      <td style="border: 1px solid #ddd; padding: 8px;">feat:</td>
      <td style="border: 1px solid #ddd; padding: 8px;">add internationalization to vehicles module</td>
      <td style="border: 1px solid #ddd; padding: 8px;">11/05/2026</td>
    </tr>
    <tr>
      <td style="border: 1px solid #ddd; padding: 8px;"><code>InnovaTechStudio/AutoService-730-AW-Frontend</code></td>
      <td style="border: 1px solid #ddd; padding: 8px;"><code>develop</code></td>
      <td style="border: 1px solid #ddd; padding: 8px;"><code>95c24cb</code></td>
      <td style="border: 1px solid #ddd; padding: 8px;">feat:</td>
      <td style="border: 1px solid #ddd; padding: 8px;">add internationalization to customers module</td>
      <td style="border: 1px solid #ddd; padding: 8px;">11/05/2026</td>
    </tr>
    <tr>
      <td style="border: 1px solid #ddd; padding: 8px;"><code>InnovaTechStudio/AutoService-730-AW-Frontend</code></td>
      <td style="border: 1px solid #ddd; padding: 8px;"><code>develop</code></td>
      <td style="border: 1px solid #ddd; padding: 8px;"><code>d684096</code></td>
      <td style="border: 1px solid #ddd; padding: 8px;">feat:</td>
      <td style="border: 1px solid #ddd; padding: 8px;">add internationalization to work orders</td>
      <td style="border: 1px solid #ddd; padding: 8px;">11/05/2026</td>
    </tr>
    <tr>
      <td style="border: 1px solid #ddd; padding: 8px;"><code>InnovaTechStudio/AutoService-730-AW-Frontend</code></td>
      <td style="border: 1px solid #ddd; padding: 8px;"><code>feature/admin-dashboard-ui</code></td>
      <td style="border: 1px solid #ddd; padding: 8px;"><code>1669c64</code></td>
      <td style="border: 1px solid #ddd; padding: 8px;">style:</td>
      <td style="border: 1px solid #ddd; padding: 8px;">improve admin dashboard interface</td>
      <td style="border: 1px solid #ddd; padding: 8px;">10/05/2026</td>
    </tr>
    <tr>
      <td style="border: 1px solid #ddd; padding: 8px;"><code>InnovaTechStudio/AutoService-730-AW-Frontend</code></td>
      <td style="border: 1px solid #ddd; padding: 8px;"><code>feature/admin-dashboard-ui</code></td>
      <td style="border: 1px solid #ddd; padding: 8px;"><code>4007e78</code></td>
      <td style="border: 1px solid #ddd; padding: 8px;">refactor:</td>
      <td style="border: 1px solid #ddd; padding: 8px;">split admin dashboard into components</td>
      <td style="border: 1px solid #ddd; padding: 8px;">10/05/2026</td>
    </tr>
    <tr>
      <td style="border: 1px solid #ddd; padding: 8px;"><code>InnovaTechStudio/AutoService-730-AW-Frontend</code></td>
      <td style="border: 1px solid #ddd; padding: 8px;"><code>feature/customer-trust</code></td>
      <td style="border: 1px solid #ddd; padding: 8px;"><code>b0f743b</code></td>
      <td style="border: 1px solid #ddd; padding: 8px;">feat:</td>
      <td style="border: 1px solid #ddd; padding: 8px;">implement vehicle tracking flow for customers</td>
      <td style="border: 1px solid #ddd; padding: 8px;">10/05/2026</td>
    </tr>
    <tr>
      <td style="border: 1px solid #ddd; padding: 8px;"><code>InnovaTechStudio/AutoService-730-AW-Frontend</code></td>
      <td style="border: 1px solid #ddd; padding: 8px;"><code>feature/customer-payment</code></td>
      <td style="border: 1px solid #ddd; padding: 8px;"><code>3ca1fa6</code></td>
      <td style="border: 1px solid #ddd; padding: 8px;">feat:</td>
      <td style="border: 1px solid #ddd; padding: 8px;">integrate online payment modal</td>
      <td style="border: 1px solid #ddd; padding: 8px;">10/05/2026</td>
    </tr>

  </tbody>
</table>

##### 5.2.2.5. Execution Evidence for Sprint Review

<p align="justify">
En esta sección se presenta la evidencia de ejecución correspondiente al Sprint 2. Durante esta iteración, el equipo logró implementar la primera versión funcional del Frontend Web Application de AutoService utilizando Vue.js y JavaScript. El sistema desarrollado incorpora módulos orientados a la gestión operativa de talleres automotrices, incluyendo dashboards administrativos, gestión de órdenes de trabajo, seguimiento de vehículos, coordinación de tareas mecánicas y visualización responsive para distintos dispositivos.<br><br>

Asimismo, se integraron componentes reutilizables, mejoras visuales de interfaz de usuario, configuraciones de entorno para consumo de APIs desplegadas en la nube y funcionalidades relacionadas con la experiencia del cliente, como seguimiento del servicio y pagos en línea. Se verificó el correcto funcionamiento de las vistas implementadas, la navegación entre módulos y la adaptabilidad responsive del sistema tanto en navegadores de escritorio como en dispositivos móviles.
</p>

<div align="center">

  <h5>Dashboard Administrativo y Gestión Operacional</h5>
  <img src="docs/assets/chapter-5/frontend_dashboard.png" 
       alt="Frontend Dashboard" width="80%">

  <h5>Vista de Órdenes de Trabajo y Gestión de Tareas</h5>
  <img src="docs/assets/chapter-5/frontend_workorders.png" 
       alt="Frontend Work Orders" width="80%">

</div>

<p align="justify">
Para evidenciar las funcionalidades implementadas durante este Sprint, se adjunta un video demostrativo donde se muestra la ejecución de los principales módulos del frontend. En el registro se aprecia la navegación entre vistas, la interacción con componentes dinámicos, el diseño responsive y la integración visual siguiendo los lineamientos de arquitectura y diseño establecidos en los capítulos previos del proyecto.
</p>

URL video de ejecución del Frontend Web Application: 
<code>https://your-demo-video-link.com</code>.

##### 5.2.2.6. Services Documentation Evidence for Sprint Review

<p align="justify">
Durante el Sprint 2, el equipo implementó y desplegó la primera versión funcional del contenedor RESTful API de AutoService utilizando JSON Server como Fake API. La solución fue desplegada en una máquina virtual con Ubuntu Linux alojada en Google Cloud Platform (GCP), permitiendo centralizar los datos del sistema y habilitar la integración en línea con la aplicación frontend desarrollada en Vue.js.
</p>

<p align="justify">
La API fue diseñada para simular el comportamiento de un backend real mediante operaciones CRUD completas utilizando los verbos HTTP principales (GET, POST, PATCH y DELETE). Durante este Sprint, se desarrollaron y consumieron múltiples endpoints relacionados con la gestión operativa del taller automotriz, incluyendo talleres, clientes, vehículos, mecánicos, órdenes de trabajo y tareas.
</p>

<p align="justify">
El despliegue de esta Fake API permitió desacoplar completamente el frontend de datos locales mockeados y facilitó las pruebas colaborativas entre los integrantes del equipo mediante una infraestructura accesible públicamente.
</p>

<p align="justify">
URL base desplegada del servicio:
</p>

<div align="center">
<code>https://autoservice-api.ddns.net/</code>
</div>

<br>

<p align="justify">
Para validar el correcto funcionamiento de los servicios implementados, el equipo realizó pruebas de interacción desde el frontend Vue.js desplegado. Asimismo, se verificó la conectividad remota mediante variables de entorno centralizadas para la URL base del API.
</p>

<p align="justify">
A continuación, se presentan evidencias visuales relacionadas con la infraestructura desplegada, el funcionamiento del JSON Server y el consumo de datos desde el frontend:
</p>

<div align="center">

  <h5>Evidencia 1: Máquina virtual Ubuntu desplegada en Google Cloud Platform</h5>
  <img src="docs/assets/chapter-5/gcp_ubuntu_vm.png" alt="GCP Ubuntu VM" width="80%">

  <h5>Evidencia 2: JSON Server ejecutándose con recursos REST disponibles</h5>
  <img src="docs/assets/chapter-5/json_server_running.png" alt="JSON Server Running" width="80%">

  <h5>Evidencia 3: Respuesta JSON de endpoint /work-orders</h5>
  <img src="docs/assets/chapter-5/workorders_response.png" alt="Work Orders Response" width="80%">

</div>

<p align="justify">
Repositorio relacionado con la implementación y consumo de Web Services:
</p>

<ul>
  <li>
    <code>https://github.com/InnovaTechStudio/AutoService-730-AW-Frontend</code>
  </li>
</ul>

<p align="justify">
Commits relevantes relacionados con integración y consumo de servicios durante el Sprint 2:
</p>

<ul>
  <li><code>c118649</code> — feat: import i18n in main.js</li>
  <li><code>0dbf840</code> — feat: add internationalization to login view</li>
  <li><code>d1b0d5c</code> — feat: add internationalization to vehicles</li>
  <li><code>d684096</code> — feat: add internationalization to work orders</li>
  <li><code>e22ee6a</code> — feat: add more updates to internationalization (tracking and payment)</li>
  <li><code>136cef0</code> — feat: implement base logic and components for customer management</li>
  <li><code>b0f743b</code> — feat: implementar flujo de seguimiento de vehículos de clientes</li>
  <li><code>84bf274</code> — feat: implement dynamic vehicle image syncing and dashboard improvements</li>
  <li><code>1669c64</code> — style: improve admin dashboard interface</li>
  <li><code>92512fa</code> — feat: integrate vehicle images into work orders</li>
  <li><code>f9d6273</code> — feat: UI design improvement and backend support</li>
</ul>

##### 5.2.2.7. Software Deployment Evidence for Sprint Review

<p align="justify">
Durante el Sprint 2, el equipo realizó el despliegue funcional de la Web Application y de la Fake API utilizada para el consumo de datos dinámicos del sistema AutoService. A diferencia del Sprint 1, donde únicamente se desplegó la Landing Page institucional, en esta iteración se consolidó una arquitectura distribuida compuesta por un Frontend desplegado en la nube mediante Azure Static Web Apps y un servidor de datos RESTful desplegado sobre una máquina virtual Ubuntu en Google Cloud Platform (GCP).
</p>

<p align="justify">
El despliegue permitió validar exitosamente la comunicación entre el cliente desarrollado en Vue.js y la Fake API basada en JSON Server, habilitando operaciones HTTP reales para las entidades principales del sistema como talleres, clientes, vehículos, órdenes de trabajo, mecánicos y tareas. Asimismo, se verificó el correcto funcionamiento del flujo CI/CD automatizado mediante GitHub Actions para el despliegue continuo del frontend.
</p>

<p align="justify">
La arquitectura de despliegue implementada durante este Sprint se compone de los siguientes elementos:
</p>

<ol style="text-align: justify;">
  <li>
    <strong>Frontend Web Application:</strong> Aplicación desarrollada con Vue.js y desplegada mediante Azure Static Web Apps.
  </li>
  <li>
    <strong>Fake REST API:</strong> Servicio RESTful basado en JSON Server desplegado en una máquina virtual Ubuntu sobre Google Cloud Platform.
  </li>
  <li>
    <strong>Process Manager:</strong> Uso de PM2 para mantener la disponibilidad continua del servicio backend.
  </li>
  <li>
    <strong>CI/CD:</strong> Integración continua y despliegue automático mediante GitHub Actions conectado al repositorio oficial del proyecto.
  </li>
</ol>

<p align="justify">
Para el despliegue del frontend, se utilizó Azure Static Web Apps aprovechando su integración nativa con GitHub Actions. El proceso automatizado realiza la compilación de la aplicación Vue y publica automáticamente una nueva versión cada vez que se ejecuta un merge hacia la rama principal del repositorio.
</p>

<p align="justify">
En paralelo, la Fake API fue desplegada sobre una instancia Ubuntu en GCP utilizando Node.js y JSON Server. El servicio fue configurado para ejecutarse persistentemente mediante PM2, permitiendo que los endpoints REST permanezcan disponibles incluso tras reinicios del servidor. Además, se configuró un dominio dinámico DDNS para facilitar el acceso remoto al servicio desde el frontend desplegado en Azure.
</p>

<div align="center">

  <h5>Evidencia 1: Azure Static Web App desplegada en producción (Vue.js)</h5>
  <img src="docs/assets/chapter-5/azure_static_webapp_overview.png" 
       alt="Azure Static Web App Overview" 
       width="80%">

  <h5>Evidencia 2: Pipeline CI/CD ejecutado correctamente mediante GitHub Actions</h5>
  <img src="docs/assets/chapter-5/github_actions_frontend_deploy.png" 
       alt="GitHub Actions Deploy" 
       width="80%">

  <h5>Evidencia 3: Servicio JSON Server ejecutándose persistentemente con PM2</h5>
  <img src="docs/assets/chapter-5/pm2_json_server_running.png" 
       alt="PM2 JSON Server Running" 
       width="80%">

</div>

<p align="justify">
La aplicación frontend desplegada se encuentra disponible públicamente en la siguiente URL:
</p>

<p align="center">
  <code>https://witty-meadow-063b9d310.7.azurestaticapps.net/</code>
</p>

<p align="justify">
Asimismo, la Fake API RESTful desplegada mediante JSON Server se encuentra disponible en:
</p>

<p align="center">
  <code>https://autoservice-api.ddns.net/</code>
</p>

<p align="justify">
El repositorio oficial del frontend utilizado para el despliegue continuo es:
</p>

<p align="center">
  <code>https://github.com/InnovaTechStudio/AutoService-730-AW-Frontend</code>
</p>

<p align="justify">
Entre los commits más relevantes relacionados con despliegue, integración y configuración de producción para este Sprint destacan:
</p>

<table style="width: 100%; border-collapse: collapse; text-align: justify;">
  <thead>
    <tr style="background-color: #f2f2f2;">
      <th style="border: 1px solid #ddd; padding: 8px;">Commit Id</th>
      <th style="border: 1px solid #ddd; padding: 8px;">Commit Message</th>
      <th style="border: 1px solid #ddd; padding: 8px;">Descripción Técnica</th>
    </tr>
  </thead>
  <tbody>
    <tr><td><code>c118649</code></td><td>feat: import i18n in main.js</td><td>Configuración base de internacionalización en la aplicación Vue.js.</td></tr>
    <tr><td><code>0dbf840</code></td><td>feat: add i18n to login view</td><td>Implementación de traducciones en vista de login.</td></tr>
    <tr><td><code>d1b0d5c</code></td><td>feat: add i18n to vehicles</td><td>Internacionalización del módulo de vehículos.</td></tr>
    <tr><td><code>d684096</code></td><td>feat: add i18n to work orders</td><td>Internacionalización del módulo de órdenes de trabajo.</td></tr>
    <tr><td><code>e22ee6a</code></td><td>feat: add tracking and payment updates</td><td>Mejoras en módulos de tracking y pagos.</td></tr>
    <tr><td><code>136cef0</code></td><td>feat: customer logic and components</td><td>Implementación base de lógica de clientes.</td></tr>
    <tr><td><code>b0f743b</code></td><td>feat: vehicle tracking flow</td><td>Flujo de seguimiento de vehículos de clientes.</td></tr>
    <tr><td><code>84bf274</code></td><td>feat: vehicle image syncing</td><td>Sincronización dinámica de imágenes de vehículos.</td></tr>
    <tr><td><code>1669c64</code></td><td>style: improve admin dashboard</td><td>Mejoras visuales del dashboard administrativo.</td></tr>
    <tr><td><code>92512fa</code></td><td>feat: integrate vehicle images</td><td>Integración de imágenes en órdenes de trabajo.</td></tr>
    <tr><td><code>f9d6273</code></td><td>feat: UI improvements and backend support</td><td>Mejoras generales de UI y soporte de integración.</td></tr>
  </tbody>
</table>

##### 5.2.1.8. Team Collaboration Insights during Sprint

<p align="justify">
Durante el Sprint 2, el equipo mantuvo un flujo de trabajo colaborativo enfocado en la implementación funcional de la Web Application de AutoService utilizando Angular y una arquitectura basada en dominios. Para garantizar la organización del desarrollo y la estabilidad del proyecto, se aplicó estrictamente la estrategia GitFlow, utilizando ramas independientes para cada funcionalidad, corrección o mejora implementada durante el Sprint.
</p>

<p align="justify">
Cada integrante trabajó sobre ramas <i>feature/*</i> y <i>hotfix/*</i>, integrando posteriormente sus avances mediante Pull Requests hacia la rama <code>develop</code>. Posteriormente, luego de las validaciones funcionales y revisiones correspondientes, los cambios fueron consolidados hacia la rama <code>main</code> para su despliegue automático en Azure Static Web Apps mediante GitHub Actions.
</p>

<p align="justify">
La colaboración del equipo se evidenció principalmente en el desarrollo conjunto de vistas administrativas, gestión de órdenes de trabajo, integración de componentes responsivos, conexión con la Fake API RESTful y configuración de entornos de producción. Asimismo, se aplicaron convenciones de versionamiento utilizando <i>Conventional Commits</i>, permitiendo mantener trazabilidad clara de cada cambio realizado durante el Sprint.
</p>

<p align="justify">
A continuación, se presentan los analíticos y evidencias extraídas directamente del repositorio frontend del proyecto, las cuales reflejan la actividad constante, integración colaborativa y organización del equipo durante el Sprint 2.
</p>

<div align="center">

  <h5>Evidencia 1: Gráfico de contribuciones por integrante del equipo</h5>
  <img src="docs/assets/chapter-5/frontend_contributors_graph.png" alt="Frontend Contributors Graph" width="80%">

  <h5>Evidencia 2: Resumen de actividad del Sprint mediante GitHub Pulse</h5>
  <img src="docs/assets/chapter-5/frontend_pulse_activity.png"  alt="Frontend Pulse Activity" width="80%">

  <h5>Evidencia 3: Gestión colaborativa mediante Pull Requests y merges</h5>
  <img src="docs/assets/chapter-5/frontend_closed_pull_requests.png" alt="Frontend Closed Pull Requests" width="80%">

  <h5>Evidencia 4: Organización de ramas bajo estrategia GitFlow</h5>
  <img src="docs/assets/chapter-5/frontend_gitflow_branches.png" alt="Frontend GitFlow Branches" width="80%">

</div>

<p align="justify">
Las evidencias presentadas demuestran que el equipo mantuvo una participación activa y distribuida durante todo el Sprint, registrando commits significativos, integraciones frecuentes y despliegues continuos hacia producción. Asimismo, el uso de Pull Requests permitió centralizar la revisión de cambios y asegurar la estabilidad del proyecto antes de cada integración hacia las ramas principales del repositorio.
</p>

<p align="justify">
Entre las actividades colaborativas más relevantes realizadas durante este Sprint destacan:
</p>

<ul style="text-align: justify;">
  <li>Implementación de vistas administrativas y dashboards.</li>
  <li>Desarrollo de módulos de órdenes de trabajo y gestión de tareas.</li>
  <li>Integración de componentes responsivos para dispositivos móviles.</li>
  <li>Conexión del frontend Angular con la Fake API RESTful desplegada en GCP.</li>
  <li>Configuración de variables de entorno y despliegue productivo en Azure Static Web Apps.</li>
  <li>Corrección de errores de compilación e integración entre módulos.</li>
</ul>

<p align="justify">
El repositorio principal utilizado para el trabajo colaborativo durante este Sprint fue:
</p>

<p align="center">
  <code>
    https://github.com/InnovaTechStudio/AutoService-729-OS-Frontend
  </code>
</p>

#### 5.2.3. Sprint 3

##### 5.2.3.1. Sprint Planning 3

<div align="center">
  <table style="margin: auto; width: 100%; border-collapse: collapse; text-align: left;">
    <thead>
      <tr>
        <th colspan="2" style="text-align: center; background-color: #f2f2f2; font-size: 1.2em; padding: 10px; border: 1px solid #ddd;">Sprint #3</th>
      </tr>
    </thead>
    <tbody>
      <tr>
        <td colspan="2" style="background-color: #fafafa; font-weight: bold; text-align: center; padding: 10px; border: 1px solid #ddd;">Sprint Planning Background</td>
      </tr>
      <tr>
        <td style="width: 30%; font-weight: bold; padding: 10px; border: 1px solid #ddd;">Date</td>
        <td style="padding: 10px; border: 1px solid #ddd;">2026-06-03</td>
      </tr>
      <tr>
        <td style="font-weight: bold; padding: 10px; border: 1px solid #ddd;">Time</td>
        <td style="padding: 10px; border: 1px solid #ddd;">10:00 AM</td>
      </tr>
      <tr>
        <td style="font-weight: bold; padding: 10px; border: 1px solid #ddd;">Location</td>
        <td style="padding: 10px; border: 1px solid #ddd;">Reunión presencial en la UPC. (Pabellón I, piso 6, cubículo 5)</td>
      </tr>
      <tr>
        <td style="font-weight: bold; padding: 10px; border: 1px solid #ddd;">Prepared By</td>
        <td style="padding: 10px; border: 1px solid #ddd;">López Monroy, Rodrigo Alfredo</td>
      </tr>
      <tr>
        <td style="font-weight: bold; padding: 10px; border: 1px solid #ddd;">Attendees (to planning meeting)</td>
        <td style="padding: 10px; border: 1px solid #ddd;">
          Pillaca Gonzales, Andy Saúl / López Monroy, Rodrigo Alfredo / Luis Miranda, Diego Andres / Mamani Vilca, Alan Jaivi / Sanchez Cuadrado, Juan Antonio
        </td>
      </tr>
      <tr>
        <td style="font-weight: bold; padding: 10px; border: 1px solid #ddd;">Sprint 2 Review Summary</td>
        <td style="padding: 10px; border: 1px solid #ddd;">
          Durante el Sprint 2, el equipo logró desarrollar la aplicación web en el lado del cliente (Frontend), integrando exitosamente el consumo de datos a través de un entorno simulado (Fake REST API). Además, se configuró el flujo de integración y despliegue continuo hacia entornos de producción, logrando una versión interactiva para la gestión operativa del sistema.
        </td>
      </tr>
      <tr>
        <td style="font-weight: bold; padding: 10px; border: 1px solid #ddd;">Sprint 2 Retrospective Summary</td>
        <td style="padding: 10px; border: 1px solid #ddd;">
          El equipo destacó la eficiencia en el flujo de trabajo mediante ramas de características y Pull Requests. Como punto de mejora, se identificó la necesidad de definir los contratos de datos y la documentación OpenAPI (Swagger) antes de programar la lógica de negocio, garantizando así una conexión fluida y sin reprocesos entre el nuevo backend en C# y el frontend existente.
        </td>
      </tr>
      <tr>
        <td colspan="2" style="background-color: #fafafa; font-weight: bold; text-align: center; padding: 10px; border: 1px solid #ddd;">Sprint Goal & User Stories</td>
      </tr>
      <tr>
        <td style="font-weight: bold; padding: 10px; border: 1px solid #ddd;">Sprint 3 Goal</td>
        <td style="padding: 10px; border: 1px solid #ddd;">
          <strong>Our focus is on</strong> developing the backend Web Services, deploying them to a cloud platform, and establishing a successful connection with the updated frontend application.<br><br>
          <strong>We believe it delivers</strong> a fully integrated and robust software solution that manages real business logic and persistent data, effectively replacing the temporary mock API environment.<br><br>
          <strong>This will be confirmed when</strong> the frontend successfully communicates with the deployed backend endpoints, all services are documented via Swagger, and the end-to-end functionality is verified through usability evaluation interviews.
        </td>
      </tr>
      <tr>
        <td style="font-weight: bold; padding: 10px; border: 1px solid #ddd;">Sprint 3 Velocity</td>
        <td style="padding: 10px; border: 1px solid #ddd;">37 Story Points</td>
      </tr>
      <tr>
        <td style="font-weight: bold; padding: 10px; border: 1px solid #ddd;">Sum of Story Points</td>
        <td style="padding: 10px; border: 1px solid #ddd;">
          37 Story Points (US-11: 2, US-12: 3, US-25: 3, US-26: 2, US-27: 2, TS-03: 3, TS-05: 5, TS-06: 3, TS-07: 5, TS-08: 3, TS-09: 3, TS-12: 2).
        </td>
      </tr>
    </tbody>
  </table>
</div>

##### 5.2.3.2. Aspect Leaders and Collaborators

En el presente Sprint 3, el alcance funcional y técnico se ha dividido en cuatro aspectos principales para garantizar una entrega eficiente y alineada con los requerimientos arquitectónicos y de validación:
1. **Backend Development:** Desarrollo de los Web Services y lógica de negocio mediante ASP.NET Core y C#.
2. **Backend Deployment:** Configuración de servicios en la nube y despliegue continuo de los Web Services.
3. **Frontend Adaptations:** Ajustes en la aplicación cliente para el consumo de los nuevos endpoints reales.
4. **Validation Interviews:** Diseño, ejecución y análisis de las entrevistas de validación y heurísticas con usuarios finales.

<div align="center">
  <table style="margin: auto; width: 100%; border-collapse: collapse; text-align: center;">
    <thead>
      <tr style="background-color: #f2f2f2;">
        <th style="padding: 10px; border: 1px solid #ddd; text-align: left;">Team Member (Last Name, First Name)</th>
        <th style="padding: 10px; border: 1px solid #ddd;">GitHub Username</th>
        <th style="padding: 10px; border: 1px solid #ddd;">Backend Development<br><small>Leader (L) / Collaborator (C)</small></th>
        <th style="padding: 10px; border: 1px solid #ddd;">Backend Deployment<br><small>Leader (L) / Collaborator (C)</small></th>
        <th style="padding: 10px; border: 1px solid #ddd;">Frontend Adaptations<br><small>Leader (L) / Collaborator (C)</small></th>
        <th style="padding: 10px; border: 1px solid #ddd;">Validation Interviews<br><small>Leader (L) / Collaborator (C)</small></th>
      </tr>
    </thead>
    <tbody>
      <tr>
        <td style="padding: 10px; border: 1px solid #ddd; text-align: left;">López Monroy, Rodrigo Alfredo</td>
        <td style="padding: 10px; border: 1px solid #ddd;">rodrigolopezu</td>
        <td style="padding: 10px; border: 1px solid #ddd; font-weight: bold; color: #2e7d32;">L</td>
        <td style="padding: 10px; border: 1px solid #ddd; color: #1976d2;">C</td>
        <td style="padding: 10px; border: 1px solid #ddd; color: #1976d2;">C</td>
        <td style="padding: 10px; border: 1px solid #ddd; color: #1976d2;">C</td>
      </tr>
      <tr>
        <td style="padding: 10px; border: 1px solid #ddd; text-align: left;">Luis Miranda, Diego Andres</td>
        <td style="padding: 10px; border: 1px solid #ddd;">andrewdmr</td>
        <td style="padding: 10px; border: 1px solid #ddd; color: #1976d2;">C</td>
        <td style="padding: 10px; border: 1px solid #ddd; font-weight: bold; color: #2e7d32;">L</td>
        <td style="padding: 10px; border: 1px solid #ddd; color: #1976d2;">C</td>
        <td style="padding: 10px; border: 1px solid #ddd; color: #1976d2;">C</td>
      </tr>
      <tr>
        <td style="padding: 10px; border: 1px solid #ddd; text-align: left;">Mamani Vilca, Alan Jaivi</td>
        <td style="padding: 10px; border: 1px solid #ddd;">alanmamaniv</td>
        <td style="padding: 10px; border: 1px solid #ddd; color: #1976d2;">C</td>
        <td style="padding: 10px; border: 1px solid #ddd; color: #1976d2;">C</td>
        <td style="padding: 10px; border: 1px solid #ddd; color: #1976d2;">C</td>
        <td style="padding: 10px; border: 1px solid #ddd; font-weight: bold; color: #2e7d32;">L</td>
      </tr>
      <tr>
        <td style="padding: 10px; border: 1px solid #ddd; text-align: left;">Pillaca Gonzales, Andy Saúl</td>
        <td style="padding: 10px; border: 1px solid #ddd;">apillacag</td>
        <td style="padding: 10px; border: 1px solid #ddd; color: #1976d2;">C</td>
        <td style="padding: 10px; border: 1px solid #ddd; color: #1976d2;">C</td>
        <td style="padding: 10px; border: 1px solid #ddd; color: #1976d2;">C</td>
        <td style="padding: 10px; border: 1px solid #ddd; color: #1976d2;">C</td>
      </tr>
      <tr>
        <td style="padding: 10px; border: 1px solid #ddd; text-align: left;">Sanchez Cuadrado, Juan Antonio</td>
        <td style="padding: 10px; border: 1px solid #ddd;">juanasc05</td>
        <td style="padding: 10px; border: 1px solid #ddd; color: #1976d2;">C</td>
        <td style="padding: 10px; border: 1px solid #ddd; color: #1976d2;">C</td>
        <td style="padding: 10px; border: 1px solid #ddd; font-weight: bold; color: #2e7d32;">L</td>
        <td style="padding: 10px; border: 1px solid #ddd; color: #1976d2;">C</td>
      </tr>
    </tbody>
  </table>
</div>

##### 5.2.3.3. Sprint Backlog 3

El presente Sprint Backlog detalla la descomposición técnica de las historias de usuario y técnicas seleccionadas para la tercera iteración del proyecto. El objetivo principal de este Sprint es desarrollar el Backend mediante servicios RESTful en C# con ASP.NET Core, establecer la persistencia de datos reales, conectar el Frontend actualizado con los nuevos endpoints y desplegar la solución en la nube para pruebas de integración. A continuación, se presenta la captura de nuestro tablero en Jira Software, seguida de la tabla de control de estado con la distribución de los Work-Items.

<div align="center">
  <img src="docs/assets/sprint3_jira.png" alt="Sprint 3 Jira Board" width="80%">
</div>

<br>

<div align="center">
  <table style="margin: auto; width: 100%; border-collapse: collapse; text-align: left; font-size: 13px; border: 1px solid #ddd;">
    <thead>
      <tr style="background-color: #e0e0e0; font-weight: bold;">
        <th style="padding: 10px; text-align: center; border: 1px solid #ddd;">Sprint #</th>
        <th colspan="7" style="padding: 10px; text-align: left; border: 1px solid #ddd;">3</th>
      </tr>
      <tr style="background-color: #f2f2f2;">
        <th colspan="2" style="text-align: center; border: 1px solid #ddd; padding: 10px;">User Story</th>
        <th colspan="6" style="text-align: center; border: 1px solid #ddd; padding: 10px;">Work-Item / Task</th>
      </tr>
      <tr style="background-color: #fafafa; text-align: center;">
        <th style="border: 1px solid #ddd; padding: 5px; width: 6%;">Id</th>
        <th style="border: 1px solid #ddd; padding: 5px; width: 15%;">Title</th>
        <th style="border: 1px solid #ddd; padding: 5px; width: 6%;">Id</th>
        <th style="border: 1px solid #ddd; padding: 5px; width: 15%;">Title</th>
        <th style="border: 1px solid #ddd; padding: 5px; width: 30%;">Description</th>
        <th style="border: 1px solid #ddd; padding: 5px; width: 8%;">Estimation (Hours)</th>
        <th style="border: 1px solid #ddd; padding: 5px; width: 12%;">Assigned To</th>
        <th style="border: 1px solid #ddd; padding: 5px; width: 8%;">Status</th>
      </tr>
    </thead>
    <tbody>
      <tr>
        <td rowspan="2" style="border: 1px solid #ddd; padding: 8px; text-align: center; font-weight: bold;">US-11</td>
        <td rowspan="2" style="border: 1px solid #ddd; padding: 8px;">Actualizar estado del vehículo</td>
        <td style="border: 1px solid #ddd; padding: 8px; text-align: center;">WI-32</td>
        <td style="border: 1px solid #ddd; padding: 8px;">Adaptación UI de estado</td>
        <td style="border: 1px solid #ddd; padding: 8px;"><i>Actualizar componentes frontend para enviar cambios de estado al nuevo API.</i></td>
        <td style="border: 1px solid #ddd; padding: 8px; text-align: center;">2</td>
        <td style="border: 1px solid #ddd; padding: 8px;">Luis, Diego</td>
        <td style="border: 1px solid #ddd; padding: 8px; text-align: center; color: #2aac2a; font-weight: bold;">Done</td>
      </tr>
      <tr>
        <td style="border: 1px solid #ddd; padding: 8px; text-align: center;">WI-33</td>
        <td style="border: 1px solid #ddd; padding: 8px;">Endpoint PATCH estado</td>
        <td style="border: 1px solid #ddd; padding: 8px;"><i>Crear controlador en C# para actualizar la etapa del vehículo.</i></td>
        <td style="border: 1px solid #ddd; padding: 8px; text-align: center;">2</td>
        <td style="border: 1px solid #ddd; padding: 8px;">López, Rodrigo</td>
        <td style="border: 1px solid #ddd; padding: 8px; text-align: center; color: #2aac2a; font-weight: bold;">Done</td>
      </tr>
      <tr>
        <td rowspan="2" style="border: 1px solid #ddd; padding: 8px; text-align: center; font-weight: bold;">US-12</td>
        <td rowspan="2" style="border: 1px solid #ddd; padding: 8px;">Visualizar detalle del vehículo</td>
        <td style="border: 1px solid #ddd; padding: 8px; text-align: center;">WI-34</td>
        <td style="border: 1px solid #ddd; padding: 8px;">Integración GET detalle</td>
        <td style="border: 1px solid #ddd; padding: 8px;"><i>Consumir el endpoint real para poblar la vista de detalles del vehículo.</i></td>
        <td style="border: 1px solid #ddd; padding: 8px; text-align: center;">3</td>
        <td style="border: 1px solid #ddd; padding: 8px;">Pillaca, Andy</td>
        <td style="border: 1px solid #ddd; padding: 8px; text-align: center; color: #2aac2a; font-weight: bold;">Done</td>
      </tr>
      <tr>
        <td style="border: 1px solid #ddd; padding: 8px; text-align: center;">WI-35</td>
        <td style="border: 1px solid #ddd; padding: 8px;">Lógica de negocio detalle</td>
        <td style="border: 1px solid #ddd; padding: 8px;"><i>Implementar servicio en backend que consolide datos de cliente y vehículo.</i></td>
        <td style="border: 1px solid #ddd; padding: 8px; text-align: center;">3</td>
        <td style="border: 1px solid #ddd; padding: 8px;">Sanchez, Juan</td>
        <td style="border: 1px solid #ddd; padding: 8px; text-align: center; color: #2aac2a; font-weight: bold;">Done</td>
      </tr>
      <tr>
        <td rowspan="2" style="border: 1px solid #ddd; padding: 8px; text-align: center; font-weight: bold;">US-25</td>
        <td rowspan="2" style="border: 1px solid #ddd; padding: 8px;">Visualizar tareas del vehículo</td>
        <td style="border: 1px solid #ddd; padding: 8px; text-align: center;">WI-36</td>
        <td style="border: 1px solid #ddd; padding: 8px;">Endpoint tareas por orden</td>
        <td style="border: 1px solid #ddd; padding: 8px;"><i>Exponer lista de tareas asociadas a una orden de trabajo específica.</i></td>
        <td style="border: 1px solid #ddd; padding: 8px; text-align: center;">3</td>
        <td style="border: 1px solid #ddd; padding: 8px;">Mamani, Alan</td>
        <td style="border: 1px solid #ddd; padding: 8px; text-align: center; color: #2aac2a; font-weight: bold;">Done</td>
      </tr>
      <tr>
        <td style="border: 1px solid #ddd; padding: 8px; text-align: center;">WI-37</td>
        <td style="border: 1px solid #ddd; padding: 8px;">Componente tareas cliente</td>
        <td style="border: 1px solid #ddd; padding: 8px;"><i>Desarrollar componente de solo lectura para el panel de cliente.</i></td>
        <td style="border: 1px solid #ddd; padding: 8px; text-align: center;">3</td>
        <td style="border: 1px solid #ddd; padding: 8px;">Luis, Diego</td>
        <td style="border: 1px solid #ddd; padding: 8px; text-align: center; color: #2aac2a; font-weight: bold;">Done</td>
      </tr>
      <tr>
        <td rowspan="2" style="border: 1px solid #ddd; padding: 8px; text-align: center; font-weight: bold;">US-26</td>
        <td rowspan="2" style="border: 1px solid #ddd; padding: 8px;">Visualizar fechas estimadas</td>
        <td style="border: 1px solid #ddd; padding: 8px; text-align: center;">WI-38</td>
        <td style="border: 1px solid #ddd; padding: 8px;">Cálculo de fechas API</td>
        <td style="border: 1px solid #ddd; padding: 8px;"><i>Lógica en backend para proyectar y retornar fechas de entrega.</i></td>
        <td style="border: 1px solid #ddd; padding: 8px; text-align: center;">2</td>
        <td style="border: 1px solid #ddd; padding: 8px;">López, Rodrigo</td>
        <td style="border: 1px solid #ddd; padding: 8px; text-align: center; color: #2aac2a; font-weight: bold;">Done</td>
      </tr>
      <tr>
        <td style="border: 1px solid #ddd; padding: 8px; text-align: center;">WI-39</td>
        <td style="border: 1px solid #ddd; padding: 8px;">Renderizado de fechas</td>
        <td style="border: 1px solid #ddd; padding: 8px;"><i>Formatear y mostrar fechas proyectadas en la vista de seguimiento.</i></td>
        <td style="border: 1px solid #ddd; padding: 8px; text-align: center;">2</td>
        <td style="border: 1px solid #ddd; padding: 8px;">Pillaca, Andy</td>
        <td style="border: 1px solid #ddd; padding: 8px; text-align: center; color: #2aac2a; font-weight: bold;">Done</td>
      </tr>
      <tr>
        <td rowspan="2" style="border: 1px solid #ddd; padding: 8px; text-align: center; font-weight: bold;">US-27</td>
        <td rowspan="2" style="border: 1px solid #ddd; padding: 8px;">Visualizar costos del servicio</td>
        <td style="border: 1px solid #ddd; padding: 8px; text-align: center;">WI-40</td>
        <td style="border: 1px solid #ddd; padding: 8px;">Agregación de costos</td>
        <td style="border: 1px solid #ddd; padding: 8px;"><i>Servicio para sumar costos de tareas planificadas en la orden.</i></td>
        <td style="border: 1px solid #ddd; padding: 8px; text-align: center;">2</td>
        <td style="border: 1px solid #ddd; padding: 8px;">Mamani, Alan</td>
        <td style="border: 1px solid #ddd; padding: 8px; text-align: center; color: #2aac2a; font-weight: bold;">Done</td>
      </tr>
      <tr>
        <td style="border: 1px solid #ddd; padding: 8px; text-align: center;">WI-41</td>
        <td style="border: 1px solid #ddd; padding: 8px;">UI desglose de costos</td>
        <td style="border: 1px solid #ddd; padding: 8px;"><i>Mostrar tabla de presupuesto y total estimado en el panel de cliente.</i></td>
        <td style="border: 1px solid #ddd; padding: 8px; text-align: center;">2</td>
        <td style="border: 1px solid #ddd; padding: 8px;">Sanchez, Juan</td>
        <td style="border: 1px solid #ddd; padding: 8px; text-align: center; color: #2aac2a; font-weight: bold;">Done</td>
      </tr>
      <tr>
        <td rowspan="2" style="border: 1px solid #ddd; padding: 8px; text-align: center; font-weight: bold;">TS-03</td>
        <td rowspan="2" style="border: 1px solid #ddd; padding: 8px;">Estructurar backend modular</td>
        <td style="border: 1px solid #ddd; padding: 8px; text-align: center;">WI-42</td>
        <td style="border: 1px solid #ddd; padding: 8px;">Configuración de capas</td>
        <td style="border: 1px solid #ddd; padding: 8px;"><i>Separar el proyecto C# en Controllers, Services y Data.</i></td>
        <td style="border: 1px solid #ddd; padding: 8px; text-align: center;">3</td>
        <td style="border: 1px solid #ddd; padding: 8px;">López, Rodrigo</td>
        <td style="border: 1px solid #ddd; padding: 8px; text-align: center; color: #2aac2a; font-weight: bold;">Done</td>
      </tr>
      <tr>
        <td style="border: 1px solid #ddd; padding: 8px; text-align: center;">WI-43</td>
        <td style="border: 1px solid #ddd; padding: 8px;">Inyección de Dependencias</td>
        <td style="border: 1px solid #ddd; padding: 8px;"><i>Registrar servicios y repositorios en el contenedor IoC de ASP.NET Core.</i></td>
        <td style="border: 1px solid #ddd; padding: 8px; text-align: center;">3</td>
        <td style="border: 1px solid #ddd; padding: 8px;">Sanchez, Juan</td>
        <td style="border: 1px solid #ddd; padding: 8px; text-align: center; color: #2aac2a; font-weight: bold;">Done</td>
      </tr>
      <tr>
        <td rowspan="2" style="border: 1px solid #ddd; padding: 8px; text-align: center; font-weight: bold;">TS-05</td>
        <td rowspan="2" style="border: 1px solid #ddd; padding: 8px;">Implementar persistencia de datos</td>
        <td style="border: 1px solid #ddd; padding: 8px; text-align: center;">WI-44</td>
        <td style="border: 1px solid #ddd; padding: 8px;">Configuración EF Core</td>
        <td style="border: 1px solid #ddd; padding: 8px;"><i>Instalar Entity Framework Core y configurar la cadena de conexión.</i></td>
        <td style="border: 1px solid #ddd; padding: 8px; text-align: center;">4</td>
        <td style="border: 1px solid #ddd; padding: 8px;">Mamani, Alan</td>
        <td style="border: 1px solid #ddd; padding: 8px; text-align: center; color: #2aac2a; font-weight: bold;">Done</td>
      </tr>
      <tr>
        <td style="border: 1px solid #ddd; padding: 8px; text-align: center;">WI-45</td>
        <td style="border: 1px solid #ddd; padding: 8px;">Migraciones y Seed Data</td>
        <td style="border: 1px solid #ddd; padding: 8px;"><i>Generar la migración inicial de la base de datos y poblar datos base.</i></td>
        <td style="border: 1px solid #ddd; padding: 8px; text-align: center;">4</td>
        <td style="border: 1px solid #ddd; padding: 8px;">López, Rodrigo</td>
        <td style="border: 1px solid #ddd; padding: 8px; text-align: center; color: #2aac2a; font-weight: bold;">Done</td>
      </tr>
      <tr>
        <td rowspan="2" style="border: 1px solid #ddd; padding: 8px; text-align: center; font-weight: bold;">TS-06</td>
        <td rowspan="2" style="border: 1px solid #ddd; padding: 8px;">Gestionar relaciones entre entidades</td>
        <td style="border: 1px solid #ddd; padding: 8px; text-align: center;">WI-46</td>
        <td style="border: 1px solid #ddd; padding: 8px;">Mapeo Fluent API</td>
        <td style="border: 1px solid #ddd; padding: 8px;"><i>Definir llaves primarias, foráneas y restricciones en el DbContext.</i></td>
        <td style="border: 1px solid #ddd; padding: 8px; text-align: center;">3</td>
        <td style="border: 1px solid #ddd; padding: 8px;">Mamani, Alan</td>
        <td style="border: 1px solid #ddd; padding: 8px; text-align: center; color: #2aac2a; font-weight: bold;">Done</td>
      </tr>
      <tr>
        <td style="border: 1px solid #ddd; padding: 8px; text-align: center;">WI-47</td>
        <td style="border: 1px solid #ddd; padding: 8px;">Repositorios de datos</td>
        <td style="border: 1px solid #ddd; padding: 8px;"><i>Crear clases para abstraer el acceso a datos y manejo de transacciones.</i></td>
        <td style="border: 1px solid #ddd; padding: 8px; text-align: center;">3</td>
        <td style="border: 1px solid #ddd; padding: 8px;">Sanchez, Juan</td>
        <td style="border: 1px solid #ddd; padding: 8px; text-align: center; color: #2aac2a; font-weight: bold;">Done</td>
      </tr>
      <tr>
        <td rowspan="2" style="border: 1px solid #ddd; padding: 8px; text-align: center; font-weight: bold;">TS-07</td>
        <td rowspan="2" style="border: 1px solid #ddd; padding: 8px;">Consumir APIs externas</td>
        <td style="border: 1px solid #ddd; padding: 8px; text-align: center;">WI-48</td>
        <td style="border: 1px solid #ddd; padding: 8px;">Configurar HttpClient</td>
        <td style="border: 1px solid #ddd; padding: 8px;"><i>Preparar HttpClient Factory para la comunicación con servicios externos.</i></td>
        <td style="border: 1px solid #ddd; padding: 8px; text-align: center;">3</td>
        <td style="border: 1px solid #ddd; padding: 8px;">López, Rodrigo</td>
        <td style="border: 1px solid #ddd; padding: 8px; text-align: center; color: #2aac2a; font-weight: bold;">Done</td>
      </tr>
      <tr>
        <td style="border: 1px solid #ddd; padding: 8px; text-align: center;">WI-49</td>
        <td style="border: 1px solid #ddd; padding: 8px;">Implementación Swagger</td>
        <td style="border: 1px solid #ddd; padding: 8px;"><i>Configurar OpenAPI Specification para exponer la documentación de la API.</i></td>
        <td style="border: 1px solid #ddd; padding: 8px; text-align: center;">4</td>
        <td style="border: 1px solid #ddd; padding: 8px;">Pillaca, Andy</td>
        <td style="border: 1px solid #ddd; padding: 8px; text-align: center; color: #2aac2a; font-weight: bold;">Done</td>
      </tr>
      <tr>
        <td rowspan="2" style="border: 1px solid #ddd; padding: 8px; text-align: center; font-weight: bold;">TS-08</td>
        <td rowspan="2" style="border: 1px solid #ddd; padding: 8px;">Manejar respuestas de API</td>
        <td style="border: 1px solid #ddd; padding: 8px; text-align: center;">WI-50</td>
        <td style="border: 1px solid #ddd; padding: 8px;">Data Transfer Objects (DTOs)</td>
        <td style="border: 1px solid #ddd; padding: 8px;"><i>Crear estructuras para recibir y enviar datos de forma segura.</i></td>
        <td style="border: 1px solid #ddd; padding: 8px; text-align: center;">3</td>
        <td style="border: 1px solid #ddd; padding: 8px;">Luis, Diego</td>
        <td style="border: 1px solid #ddd; padding: 8px; text-align: center; color: #2aac2a; font-weight: bold;">Done</td>
      </tr>
      <tr>
        <td style="border: 1px solid #ddd; padding: 8px; text-align: center;">WI-51</td>
        <td style="border: 1px solid #ddd; padding: 8px;">Serialización JSON</td>
        <td style="border: 1px solid #ddd; padding: 8px;"><i>Asegurar correcto parseo y validación de los datos entrantes.</i></td>
        <td style="border: 1px solid #ddd; padding: 8px; text-align: center;">3</td>
        <td style="border: 1px solid #ddd; padding: 8px;">Mamani, Alan</td>
        <td style="border: 1px solid #ddd; padding: 8px; text-align: center; color: #2aac2a; font-weight: bold;">Done</td>
      </tr>
      <tr>
        <td rowspan="2" style="border: 1px solid #ddd; padding: 8px; text-align: center; font-weight: bold;">TS-09</td>
        <td rowspan="2" style="border: 1px solid #ddd; padding: 8px;">Implementar manejo de errores</td>
        <td style="border: 1px solid #ddd; padding: 8px; text-align: center;">WI-52</td>
        <td style="border: 1px solid #ddd; padding: 8px;">Middleware Excepciones</td>
        <td style="border: 1px solid #ddd; padding: 8px;"><i>Capturar errores no controlados a nivel global en la API.</i></td>
        <td style="border: 1px solid #ddd; padding: 8px; text-align: center;">3</td>
        <td style="border: 1px solid #ddd; padding: 8px;">López, Rodrigo</td>
        <td style="border: 1px solid #ddd; padding: 8px; text-align: center; color: #2aac2a; font-weight: bold;">Done</td>
      </tr>
      <tr>
        <td style="border: 1px solid #ddd; padding: 8px; text-align: center;">WI-53</td>
        <td style="border: 1px solid #ddd; padding: 8px;">Formatos de error HTTP</td>
        <td style="border: 1px solid #ddd; padding: 8px;"><i>Estandarizar las respuestas 400 y 500 para el cliente web.</i></td>
        <td style="border: 1px solid #ddd; padding: 8px; text-align: center;">2</td>
        <td style="border: 1px solid #ddd; padding: 8px;">Sanchez, Juan</td>
        <td style="border: 1px solid #ddd; padding: 8px; text-align: center; color: #2aac2a; font-weight: bold;">Done</td>
      </tr>
      <tr>
        <td rowspan="2" style="border: 1px solid #ddd; padding: 8px; text-align: center; font-weight: bold;">TS-12</td>
        <td rowspan="2" style="border: 1px solid #ddd; padding: 8px;">Configurar hosting y dominio</td>
        <td style="border: 1px solid #ddd; padding: 8px; text-align: center;">WI-54</td>
        <td style="border: 1px solid #ddd; padding: 8px;">Despliegue del Web Service</td>
        <td style="border: 1px solid #ddd; padding: 8px;"><i>Publicar el backend C# en un entorno Cloud para consumo externo.</i></td>
        <td style="border: 1px solid #ddd; padding: 8px; text-align: center;">3</td>
        <td style="border: 1px solid #ddd; padding: 8px;">Luis, Diego</td>
        <td style="border: 1px solid #ddd; padding: 8px; text-align: center; color: #2aac2a; font-weight: bold;">Done</td>
      </tr>
      <tr>
        <td style="border: 1px solid #ddd; padding: 8px; text-align: center;">WI-55</td>
        <td style="border: 1px solid #ddd; padding: 8px;">Configuración de CORS</td>
        <td style="border: 1px solid #ddd; padding: 8px;"><i>Permitir las peticiones desde el origen del frontend desplegado.</i></td>
        <td style="border: 1px solid #ddd; padding: 8px; text-align: center;">2</td>
        <td style="border: 1px solid #ddd; padding: 8px;">Pillaca, Andy</td>
        <td style="border: 1px solid #ddd; padding: 8px; text-align: center; color: #2aac2a; font-weight: bold;">Done</td>
      </tr>
    </tbody>
  </table>
</div>

##### 5.2.3.4. Development Evidence for Sprint Review

<p align="justify">
Durante el Sprint 3, el equipo se enfocó en la implementación funcional de los Web Services (Backend) utilizando C# y el marco de trabajo ASP.NET Core, logrando reemplazar exitosamente el entorno simulado (Fake API) empleado en la iteración anterior. Asimismo, se consolidó la arquitectura del software basada en Domain-Driven Design (DDD), estableciendo contextos delimitados (Bounded Contexts) claros y desacoplados para la gestión operativa del taller automotriz.<br>

Entre los principales avances de este sprint se destacan la implementación de la persistencia de datos relacional mediante Entity Framework Core, la configuración de migraciones automáticas de la base de datos y la exposición de endpoints RESTful mediante controladores especializados para la gestión de inventario, órdenes de trabajo (Work Orders), vehículos (Fleet Management) y clientes. Además, se desarrollaron tareas de contenerización mediante Docker para asegurar el despliegue en la nube y se ejecutó la sincronización final con la interfaz de usuario (Frontend).<br>

En la siguiente tabla se presentan commits que representan hitos clave del desarrollo de este sprint en el repositorio del backend:
</p>

<table style="width: 100%; border-collapse: collapse; text-align: justify;">
  <thead>
    <tr style="background-color: #f2f2f2;">
      <th style="border: 1px solid #ddd; padding: 8px;">Repository</th>
      <th style="border: 1px solid #ddd; padding: 8px;">Branch</th>
      <th style="border: 1px solid #ddd; padding: 8px;">Commit Id</th>
      <th style="border: 1px solid #ddd; padding: 8px;">Commit Message</th>
      <th style="border: 1px solid #ddd; padding: 8px;">Commit Message Body</th>
      <th style="border: 1px solid #ddd; padding: 8px;">Committed on (Date)</th>
    </tr>
  </thead>

  <tbody>
    <tr>
      <td style="border: 1px solid #ddd; padding: 8px;"><code>InnovaTechStudio/AutoService-730-AW-Backend</code></td>
      <td style="border: 1px solid #ddd; padding: 8px;"><code>feature/shared-persistence</code></td>
      <td style="border: 1px solid #ddd; padding: 8px;"><code>5052eea</code></td>
      <td style="border: 1px solid #ddd; padding: 8px;">feat:</td>
      <td style="border: 1px solid #ddd; padding: 8px;">add base structure for selected bounded contexts</td>
      <td style="border: 1px solid #ddd; padding: 8px;">05/06/2026</td>
    </tr>
    <tr>
      <td style="border: 1px solid #ddd; padding: 8px;"><code>InnovaTechStudio/AutoService-730-AW-Backend</code></td>
      <td style="border: 1px solid #ddd; padding: 8px;"><code>feature/inventory-management</code></td>
      <td style="border: 1px solid #ddd; padding: 8px;"><code>8bd82ab</code></td>
      <td style="border: 1px solid #ddd; padding: 8px;">feat:</td>
      <td style="border: 1px solid #ddd; padding: 8px;">implement InventoryItemsController for inventory management API</td>
      <td style="border: 1px solid #ddd; padding: 8px;">07/06/2026</td>
    </tr>
    <tr>
      <td style="border: 1px solid #ddd; padding: 8px;"><code>InnovaTechStudio/AutoService-730-AW-Backend</code></td>
      <td style="border: 1px solid #ddd; padding: 8px;"><code>feature/workshop-operations-context</code></td>
      <td style="border: 1px solid #ddd; padding: 8px;"><code>0217886</code></td>
      <td style="border: 1px solid #ddd; padding: 8px;">feat:</td>
      <td style="border: 1px solid #ddd; padding: 8px;">add WorkOrder entity and methods</td>
      <td style="border: 1px solid #ddd; padding: 8px;">08/06/2026</td>
    </tr>
    <tr>
      <td style="border: 1px solid #ddd; padding: 8px;"><code>InnovaTechStudio/AutoService-730-AW-Backend</code></td>
      <td style="border: 1px solid #ddd; padding: 8px;"><code>feature/workshop-operations-context</code></td>
      <td style="border: 1px solid #ddd; padding: 8px;"><code>3635a20</code></td>
      <td style="border: 1px solid #ddd; padding: 8px;">feat:</td>
      <td style="border: 1px solid #ddd; padding: 8px;">add logical Task controller create, update, delete, patch</td>
      <td style="border: 1px solid #ddd; padding: 8px;">09/06/2026</td>
    </tr>
    <tr>
      <td style="border: 1px solid #ddd; padding: 8px;"><code>InnovaTechStudio/AutoService-730-AW-Backend</code></td>
      <td style="border: 1px solid #ddd; padding: 8px;"><code>feature/workshop-operations-context</code></td>
      <td style="border: 1px solid #ddd; padding: 8px;"><code>4642489</code></td>
      <td style="border: 1px solid #ddd; padding: 8px;">feat:</td>
      <td style="border: 1px solid #ddd; padding: 8px;">task-workorder management AppDbContext and repositories implementation</td>
      <td style="border: 1px solid #ddd; padding: 8px;">09/06/2026</td>
    </tr>
    <tr>
      <td style="border: 1px solid #ddd; padding: 8px;"><code>InnovaTechStudio/AutoService-730-AW-Backend</code></td>
      <td style="border: 1px solid #ddd; padding: 8px;"><code>feature/fleet-management-bounded-context</code></td>
      <td style="border: 1px solid #ddd; padding: 8px;"><code>12ff2ae</code></td>
      <td style="border: 1px solid #ddd; padding: 8px;">feat(fleet-management):</td>
      <td style="border: 1px solid #ddd; padding: 8px;">add VehiclesController REST endpoint</td>
      <td style="border: 1px solid #ddd; padding: 8px;">10/06/2026</td>
    </tr>
    <tr>
      <td style="border: 1px solid #ddd; padding: 8px;"><code>InnovaTechStudio/AutoService-730-AW-Backend</code></td>
      <td style="border: 1px solid #ddd; padding: 8px;"><code>feature/customer-management-bounded-context</code></td>
      <td style="border: 1px solid #ddd; padding: 8px;"><code>9d20ad1</code></td>
      <td style="border: 1px solid #ddd; padding: 8px;">feat(customer-management):</td>
      <td style="border: 1px solid #ddd; padding: 8px;">add CustomerController REST endpoint</td>
      <td style="border: 1px solid #ddd; padding: 8px;">11/06/2026</td>
    </tr>
    <tr>
      <td style="border: 1px solid #ddd; padding: 8px;"><code>InnovaTechStudio/AutoService-730-AW-Backend</code></td>
      <td style="border: 1px solid #ddd; padding: 8px;"><code>feature/IAM</code></td>
      <td style="border: 1px solid #ddd; padding: 8px;"><code>fd8de5f</code></td>
      <td style="border: 1px solid #ddd; padding: 8px;">feat:</td>
      <td style="border: 1px solid #ddd; padding: 8px;">add IAM v.1.0</td>
      <td style="border: 1px solid #ddd; padding: 8px;">12/06/2026</td>
    </tr>
    <tr>
      <td style="border: 1px solid #ddd; padding: 8px;"><code>InnovaTechStudio/AutoService-730-AW-Backend</code></td>
      <td style="border: 1px solid #ddd; padding: 8px;"><code>develop</code></td>
      <td style="border: 1px solid #ddd; padding: 8px;"><code>476e366</code></td>
      <td style="border: 1px solid #ddd; padding: 8px;">feat:</td>
      <td style="border: 1px solid #ddd; padding: 8px;">add Dockerfile start of deployment</td>
      <td style="border: 1px solid #ddd; padding: 8px;">13/06/2026</td>
    </tr>
    <tr>
      <td style="border: 1px solid #ddd; padding: 8px;"><code>InnovaTechStudio/AutoService-730-AW-Backend</code></td>
      <td style="border: 1px solid #ddd; padding: 8px;"><code>develop</code></td>
      <td style="border: 1px solid #ddd; padding: 8px;"><code>2702651</code></td>
      <td style="border: 1px solid #ddd; padding: 8px;">fix:</td>
      <td style="border: 1px solid #ddd; padding: 8px;">add execution automatic migrations in Program.cs</td>
      <td style="border: 1px solid #ddd; padding: 8px;">13/06/2026</td>
    </tr>
    <tr>
      <td style="border: 1px solid #ddd; padding: 8px;"><code>InnovaTechStudio/AutoService-730-AW-Backend</code></td>
      <td style="border: 1px solid #ddd; padding: 8px;"><code>feature/final-backend-sync</code></td>
      <td style="border: 1px solid #ddd; padding: 8px;"><code>b0378cc</code></td>
      <td style="border: 1px solid #ddd; padding: 8px;">feat:</td>
      <td style="border: 1px solid #ddd; padding: 8px;">Final backend sync</td>
      <td style="border: 1px solid #ddd; padding: 8px;">13/06/2026</td>
    </tr>
  </tbody>
</table>

##### 5.2.3.5. Execution Evidence for Sprint Review

<p align="justify">
Durante el Sprint 3, el equipo logró exitosamente la integración completa entre el Frontend actualizado y los nuevos Web Services desarrollados en C# con ASP.NET Core. Se reemplazó por completo la dependencia del entorno simulado (Fake API), permitiendo que la aplicación web consuma, registre y actualice datos reales alojados en una base de datos relacional. 
<br><br>
Los principales logros de ejecución incluyen la correcta visualización del detalle de los vehículos, el cálculo dinámico de costos y fechas estimadas de entrega, y la capacidad de actualizar el estado operativo de los vehículos en el taller, reflejando estos cambios en tiempo real en el panel del cliente.
</p>

<div align="center">
  <h5>Captura de Integración: Vista de Detalle y Costos de Orden de Trabajo</h5>
  <img src="docs/assets/execution_frontend_integration.png" alt="Frontend Integration with C# Backend" width="80%">
</div>

<br>

<p align="justify">
Para ilustrar la navegación y el correcto funcionamiento de estos flujos integrados, se ha preparado un video demostrativo. En el siguiente enlace se evidencia la interacción del usuario final con las nuevas funcionalidades y el consumo exitoso de los servicios desplegados:
</p>

<ul>
  <li><b>Video de Ejecución (Sprint 3):</b> <a href="enlace_pendiente" target="_blank">Ver demostración de integración Front-Back</a></li>
</ul>

##### 5.2.3.6. Services Documentation Evidence for Sprint Review

<p align="justify">
Para garantizar la correcta adopción, mantenimiento y consumo de los Web Services desarrollados en el presente hito, se implementó la documentación interactiva de la API utilizando la especificación OpenAPI a través de la herramienta Swagger. Esta interfaz permite a los desarrolladores de las aplicaciones cliente visualizar de manera transparente la estructura de las rutas, los esquemas de los recursos y los parámetros requeridos para las solicitudes HTTP.
<br><br>
A continuación, se presenta el registro detallado y completo de las acciones implementadas en la arquitectura orientada a servicios del sistema AutoService:
</p>

<ul>
  <li><b>Repositorio de Web Services:</b> <a href="https://github.com/InnovaTechStudio/AutoService-730-AW-Backend" target="_blank">AutoService-730-AW-Backend</a></li>
  <li><b>Documentación Interactiva (Swagger UI):</b> <a href="https://autoservice-aw-backend.onrender.com/swagger/index.html" target="_blank">AutoService API v1 Documentation</a></li>
</ul>

<div align="center">
  <table style="margin: auto; width: 100%; border-collapse: collapse; text-align: left; font-size: 12px; border: 1px solid #ddd;">
    <thead>
      <tr style="background-color: #f2f2f2;">
        <th style="padding: 8px; border: 1px solid #ddd; text-align: center; width: 25%;">Endpoint / Verbo HTTP</th>
        <th style="padding: 8px; border: 1px solid #ddd; width: 30%;">Descripción de la Acción</th>
        <th style="padding: 8px; border: 1px solid #ddd; width: 25%;">Parámetros Requeridos</th>
        <th style="padding: 8px; border: 1px solid #ddd; width: 20%;">Respuesta Esperada (JSON)</th>
      </tr>
    </thead>
    <tbody>
      <tr style="background-color: #fafafa; font-weight: bold;"><td colspan="4" style="padding: 6px; border: 1px solid #ddd;">Módulo de Autenticación y Acceso (Auth)</td></tr>
      <tr>
        <td style="padding: 6px; border: 1px solid #ddd; text-align: center;"><strong>POST</strong><br><code>/api/v1/auth/sign-in</code></td>
        <td style="padding: 6px; border: 1px solid #ddd;">Permite el inicio de sesión de usuarios registrados.</td>
        <td style="padding: 6px; border: 1px solid #ddd;"><b>Body:</b> <code>SignInResource</code> (email, password).</td>
        <td style="padding: 6px; border: 1px solid #ddd;"><b>200 OK</b><br>Token de acceso.</td>
      </tr>
      <tr>
        <td style="padding: 6px; border: 1px solid #ddd; text-align: center;"><strong>POST</strong><br><code>/api/v1/auth/sign-up</code></td>
        <td style="padding: 6px; border: 1px solid #ddd;">Registra una credencial de usuario con un rol y taller específico.</td>
        <td style="padding: 6px; border: 1px solid #ddd;"><b>Body:</b> <code>SignUpResource</code> (email, password, role, workshopId).</td>
        <td style="padding: 6px; border: 1px solid #ddd;"><b>200 OK</b><br>Usuario creado.</td>
      </tr>
      <tr>
        <td style="padding: 6px; border: 1px solid #ddd; text-align: center;"><strong>POST</strong><br><code>/api/v1/auth/register-workshop</code></td>
        <td style="padding: 6px; border: 1px solid #ddd;">Registra un nuevo taller automotriz junto con su administrador base.</td>
        <td style="padding: 6px; border: 1px solid #ddd;"><b>Body:</b> <code>SignUpWorkshopResource</code> (workshopName, email, password).</td>
        <td style="padding: 6px; border: 1px solid #ddd;"><b>200 OK</b><br>Taller registrado.</td>
      </tr>
      <tr style="background-color: #fafafa; font-weight: bold;"><td colspan="4" style="padding: 6px; border: 1px solid #ddd;">Módulo de Gestión de Clientes (Customers)</td></tr>
      <tr>
        <td style="padding: 6px; border: 1px solid #ddd; text-align: center;"><strong>POST</strong><br><code>/api/v1/customers</code></td>
        <td style="padding: 6px; border: 1px solid #ddd;">Crea un nuevo perfil de cliente en el taller.</td>
        <td style="padding: 6px; border: 1px solid #ddd;"><b>Body:</b> <code>CreateCustomerResource</code> (fullName, dni, email, phone).</td>
        <td style="padding: 6px; border: 1px solid #ddd;"><b>200 OK</b><br>Cliente guardado.</td>
      </tr>
      <tr>
        <td style="padding: 6px; border: 1px solid #ddd; text-align: center;"><strong>GET</strong><br><code>/api/v1/customers</code></td>
        <td style="padding: 6px; border: 1px solid #ddd;">Recupera el listado completo de clientes registrados en el sistema.</td>
        <td style="padding: 6px; border: 1px solid #ddd;">Ninguno.</td>
        <td style="padding: 6px; border: 1px solid #ddd;"><b>200 OK</b><br>Colección de clientes.</td>
      </tr>
      <tr>
        <td style="padding: 6px; border: 1px solid #ddd; text-align: center;"><strong>GET</strong><br><code>/api/v1/customers/{id}</code></td>
        <td style="padding: 6px; border: 1px solid #ddd;">Obtiene la información detallada de un cliente según su identificador único.</td>
        <td style="padding: 6px; border: 1px solid #ddd;"><b>Path:</b> <code>id</code> (integer).</td>
        <td style="padding: 6px; border: 1px solid #ddd;"><b>200 OK</b><br>Datos de cliente.</td>
      </tr>
      <tr>
        <td style="padding: 6px; border: 1px solid #ddd; text-align: center;"><strong>PUT</strong><br><code>/api/v1/customers/{id}</code></td>
        <td style="padding: 6px; border: 1px solid #ddd;">Actualiza los datos personales y de contacto de un cliente existente.</td>
        <td style="padding: 6px; border: 1px solid #ddd;"><b>Path:</b> <code>id</code> (integer)<br><b>Body:</b> <code>UpdateCustomerResource</code>.</td>
        <td style="padding: 6px; border: 1px solid #ddd;"><b>200 OK</b><br>Cliente modificado.</td>
      </tr>
      <tr>
        <td style="padding: 6px; border: 1px solid #ddd; text-align: center;"><strong>DELETE</strong><br><code>/api/v1/customers/{id}</code></td>
        <td style="padding: 6px; border: 1px solid #ddd;">Elimina de forma lógica o física un cliente del sistema.</td>
        <td style="padding: 6px; border: 1px solid #ddd;"><b>Path:</b> <code>id</code> (integer).</td>
        <td style="padding: 6px; border: 1px solid #ddd;"><b>200 OK</b><br>Confirmación de remoción.</td>
      </tr>
      <tr style="background-color: #fafafa; font-weight: bold;"><td colspan="4" style="padding: 6px; border: 1px solid #ddd;">Módulo de Inventario de Repuestos (InventoryItems)</td></tr>
      <tr>
        <td style="padding: 6px; border: 1px solid #ddd; text-align: center;"><strong>POST</strong><br><code>/api/v1/inventoryitems</code></td>
        <td style="padding: 6px; border: 1px solid #ddd;">Registra un nuevo artículo o repuesto en el almacén del taller.</td>
        <td style="padding: 6px; border: 1px solid #ddd;"><b>Body:</b> <code>CreateInventoryItemResource</code> (name, category, brand, unitPrice, stock, minStock, image).</td>
        <td style="padding: 6px; border: 1px solid #ddd;"><b>200 OK</b><br>Artículo registrado.</td>
      </tr>
      <tr>
        <td style="padding: 6px; border: 1px solid #ddd; text-align: center;"><strong>GET</strong><br><code>/api/v1/inventoryitems</code></td>
        <td style="padding: 6px; border: 1px solid #ddd;">Obtiene todos los repuestos y materiales disponibles en el inventario.</td>
        <td style="padding: 6px; border: 1px solid #ddd;">Ninguno.</td>
        <td style="padding: 6px; border: 1px solid #ddd;"><b>200 OK</b><br>Lista de inventario.</td>
      </tr>
      <tr>
        <td style="padding: 6px; border: 1px solid #ddd; text-align: center;"><strong>GET</strong><br><code>/api/v1/inventoryitems/{id}</code></td>
        <td style="padding: 6px; border: 1px solid #ddd;">Recupera los datos técnicos y stock actual de un repuesto específico.</td>
        <td style="padding: 6px; border: 1px solid #ddd;"><b>Path:</b> <code>id</code> (integer).</td>
        <td style="padding: 6px; border: 1px solid #ddd;"><b>200 OK</b><br>Detalle del artículo.</td>
      </tr>
      <tr>
        <td style="padding: 6px; border: 1px solid #ddd; text-align: center;"><strong>PUT</strong><br><code>/api/v1/inventoryitems/{id}</code></td>
        <td style="padding: 6px; border: 1px solid #ddd;">Actualiza el stock, precio unitario o propiedades de un ítem de inventario.</td>
        <td style="padding: 6px; border: 1px solid #ddd;"><b>Path:</b> <code>id</code> (integer)<br><b>Body:</b> <code>CreateInventoryItemResource</code>.</td>
        <td style="padding: 6px; border: 1px solid #ddd;"><b>200 OK</b><br>Artículo actualizado.</td>
      </tr>
      <tr>
        <td style="padding: 6px; border: 1px solid #ddd; text-align: center;"><strong>DELETE</strong><br><code>/api/v1/inventoryitems/{id}</code></td>
        <td style="padding: 6px; border: 1px solid #ddd;">Remueve un artículo del catálogo de repuestos.</td>
        <td style="padding: 6px; border: 1px solid #ddd;"><b>Path:</b> <code>id</code> (integer).</td>
        <td style="padding: 6px; border: 1px solid #ddd;"><b>200 OK</b><br>Artículo eliminado.</td>
      </tr>
      <tr style="background-color: #fafafa; font-weight: bold;"><td colspan="4" style="padding: 6px; border: 1px solid #ddd;">Módulo de Gestión de Mecánicos (Mechanics)</td></tr>
      <tr>
        <td style="padding: 6px; border: 1px solid #ddd; text-align: center;"><strong>POST</strong><br><code>/api/v1/mechanics</code></td>
        <td style="padding: 6px; border: 1px solid #ddd;">Registra un nuevo miembro del equipo técnico o mecánico.</td>
        <td style="padding: 6px; border: 1px solid #ddd;"><b>Body:</b> <code>CreateMechanicResource</code> (fullName, specialty, maxCapacity, email, password).</td>
        <td style="padding: 6px; border: 1px solid #ddd;"><b>200 OK</b><br>Mecánico creado.</td>
      </tr>
      <tr>
        <td style="padding: 6px; border: 1px solid #ddd; text-align: center;"><strong>GET</strong><br><code>/api/v1/mechanics</code></td>
        <td style="padding: 6px; border: 1px solid #ddd;">Obtiene la nómina de mecánicos registrados y sus respectivas especialidades.</td>
        <td style="padding: 6px; border: 1px solid #ddd;">Ninguno.</td>
        <td style="padding: 6px; border: 1px solid #ddd;"><b>200 OK</b><br>Lista de mecánicos.</td>
      </tr>
      <tr>
        <td style="padding: 6px; border: 1px solid #ddd; text-align: center;"><strong>GET</strong><br><code>/api/v1/mechanics/{id}</code></td>
        <td style="padding: 6px; border: 1px solid #ddd;">Recupera el perfil de un mecánico específico y su capacidad operativa.</td>
        <td style="padding: 6px; border: 1px solid #ddd;"><b>Path:</b> <code>id</code> (integer).</td>
        <td style="padding: 6px; border: 1px solid #ddd;"><b>200 OK</b><br>Datos de mecánico.</td>
      </tr>
      <tr>
        <td style="padding: 6px; border: 1px solid #ddd; text-align: center;"><strong>PUT</strong><br><code>/api/v1/mechanics/{id}</code></td>
        <td style="padding: 6px; border: 1px solid #ddd;">Modifica la especialidad, capacidad máxima o datos de contacto de un mecánico.</td>
        <td style="padding: 6px; border: 1px solid #ddd;"><b>Path:</b> <code>id</code> (integer)<br><b>Body:</b> <code>UpdateMechanicResource</code> (fullName, specialty, maxCapacity, email).</td>
        <td style="padding: 6px; border: 1px solid #ddd;"><b>200 OK</b><br>Mecánico actualizado.</td>
      </tr>
      <tr>
        <td style="padding: 6px; border: 1px solid #ddd; text-align: center;"><strong>DELETE</strong><br><code>/api/v1/mechanics/{id}</code></td>
        <td style="padding: 6px; border: 1px solid #ddd;">Elimina el registro de un mecánico del personal activo.</td>
        <td style="padding: 6px; border: 1px solid #ddd;"><b>Path:</b> <code>id</code> (integer).</td>
        <td style="padding: 6px; border: 1px solid #ddd;"><b>200 OK</b><br>Mecánico eliminado.</td>
      </tr>
      <tr style="background-color: #fafafa; font-weight: bold;"><td colspan="4" style="padding: 6px; border: 1px solid #ddd;">Módulo de Tareas Operativas (Tasks)</td></tr>
      <tr>
        <td style="padding: 6px; border: 1px solid #ddd; text-align: center;"><strong>POST</strong><br><code>/api/v1/tasks</code></td>
        <td style="padding: 6px; border: 1px solid #ddd;">Asigna una nueva actividad técnica específica a una orden de trabajo.</td>
        <td style="padding: 6px; border: 1px solid #ddd;"><b>Body:</b> <code>CreateTaskResource</code> (workOrderId, mechanicId, description, priority, estimatedTime, laborPrice).</td>
        <td style="padding: 6px; border: 1px solid #ddd;"><b>200 OK</b><br>Tarea creada.</td>
      </tr>
      <tr>
        <td style="padding: 6px; border: 1px solid #ddd; text-align: center;"><strong>GET</strong><br><code>/api/v1/tasks</code></td>
        <td style="padding: 6px; border: 1px solid #ddd;">Filtra y lista las tareas operativas asociadas a una orden o a un mecánico.</td>
        <td style="padding: 6px; border: 1px solid #ddd;"><b>Query:</b> <code>workOrderId</code> (integer), <code>mechanicId</code> (integer).</td>
        <td style="padding: 6px; border: 1px solid #ddd;"><b>200 OK</b><br>Colección de tareas.</td>
      </tr>
      <tr>
        <td style="padding: 6px; border: 1px solid #ddd; text-align: center;"><strong>PUT</strong><br><code>/api/v1/tasks/{id}</code></td>
        <td style="padding: 6px; border: 1px solid #ddd;">Reemplaza integralmente las propiedades y la asignación técnica de una tarea.</td>
        <td style="padding: 6px; border: 1px solid #ddd;"><b>Path:</b> <code>id</code> (integer)<br><b>Body:</b> <code>UpdateTaskResource</code>.</td>
        <td style="padding: 6px; border: 1px solid #ddd;"><b>200 OK</b><br>Tarea modificada.</td>
      </tr>
      <tr>
        <td style="padding: 6px; border: 1px solid #ddd; text-align: center;"><strong>PATCH</strong><br><code>/api/v1/tasks/{id}</code></td>
        <td style="padding: 6px; border: 1px solid #ddd;">Efectúa cambios parciales en el estado, diagnóstico técnico o aprobaciones de una tarea.</td>
        <td style="padding: 6px; border: 1px solid #ddd;"><b>Path:</b> <code>id</code> (integer)<br><b>Body:</b> <code>PatchTaskResource</code> (status, technicalDiagnosis, customerExplanation, internalObservation, evidenceRegistered, adminReviewStatus).</td>
        <td style="padding: 6px; border: 1px solid #ddd;"><b>200 OK</b><br>Campos actualizados.</td>
      </tr>
      <tr>
        <td style="padding: 6px; border: 1px solid #ddd; text-align: center;"><strong>DELETE</strong><br><code>/api/v1/tasks/{id}</code></td>
        <td style="padding: 6px; border: 1px solid #ddd;">Cancela y remueve una tarea operativa de la orden de trabajo.</td>
        <td style="padding: 6px; border: 1px solid #ddd;"><b>Path:</b> <code>id</code> (integer).</td>
        <td style="padding: 6px; border: 1px solid #ddd;"><b>200 OK</b><br>Tarea eliminada.</td>
      </tr>
      <tr style="background-color: #fafafa; font-weight: bold;"><td colspan="4" style="padding: 6px; border: 1px solid #ddd;">Módulo de Seguimiento Público (Tracking)</td></tr>
      <tr>
        <td style="padding: 6px; border: 1px solid #ddd; text-align: center;"><strong>GET</strong><br><code>/api/v1/tracking/workorders</code></td>
        <td style="padding: 6px; border: 1px solid #ddd;">Permite a un cliente consultar el estado general de su orden mediante el código de seguimiento único.</td>
        <td style="padding: 6px; border: 1px solid #ddd;"><b>Query:</b> <code>trackingCode</code> (string).</td>
        <td style="padding: 6px; border: 1px solid #ddd;"><b>200 OK</b><br>Estado de orden.</td>
      </tr>
      <tr>
        <td style="padding: 6px; border: 1px solid #ddd; text-align: center;"><strong>GET</strong><br><code>/api/v1/tracking/vehicles/{id}</code></td>
        <td style="padding: 6px; border: 1px solid #ddd;">Monitorea la ubicación interna o etapa de reparación actual de un vehículo.</td>
        <td style="padding: 6px; border: 1px solid #ddd;"><b>Path:</b> <code>id</code> (integer).</td>
        <td style="padding: 6px; border: 1px solid #ddd;"><b>200 OK</b><br>Seguimiento de vehículo.</td>
      </tr>
      <tr>
        <td style="padding: 6px; border: 1px solid #ddd; text-align: center;"><strong>GET</strong><br><code>/api/v1/tracking/tasks</code></td>
        <td style="padding: 6px; border: 1px solid #ddd;">Recupera el progreso en tiempo real de las tareas de una determinada orden para el cliente.</td>
        <td style="padding: 6px; border: 1px solid #ddd;"><b>Query:</b> <code>workOrderId</code> (integer).</td>
        <td style="padding: 6px; border: 1px solid #ddd;"><b>200 OK</b><br>Tareas en curso.</td>
      </tr>
      <tr>
        <td style="padding: 6px; border: 1px solid #ddd; text-align: center;"><strong>GET</strong><br><code>/api/v1/tracking/customers/{id}</code></td>
        <td style="padding: 6px; border: 1px solid #ddd;">Expone de forma segura las actualizaciones dirigidas al perfil de un cliente en particular.</td>
        <td style="padding: 6px; border: 1px solid #ddd;"><b>Path:</b> <code>id</code> (integer).</td>
        <td style="padding: 6px; border: 1px solid #ddd;"><b>200 OK</b><br>Estado del cliente.</td>
      </tr>
      <tr>
        <td style="padding: 6px; border: 1px solid #ddd; text-align: center;"><strong>GET</strong><br><code>/api/v1/tracking/workshops/{id}</code></td>
        <td style="padding: 6px; border: 1px solid #ddd;">Muestra la información de disponibilidad y datos del taller de forma externa.</td>
        <td style="padding: 6px; border: 1px solid #ddd;"><b>Path:</b> <code>id</code> (string).</td>
        <td style="padding: 6px; border: 1px solid #ddd;"><b>200 OK</b><br>Detalle de taller.</td>
      </tr>
      <tr style="background-color: #fafafa; font-weight: bold;"><td colspan="4" style="padding: 6px; border: 1px solid #ddd;">Módulo de Control de Flotas y Vehículos (Vehicles)</td></tr>
      <tr>
        <td style="padding: 6px; border: 1px solid #ddd; text-align: center;"><strong>POST</strong><br><code>/api/v1/vehicles</code></td>
        <td style="padding: 6px; border: 1px solid #ddd;">Asocia y registra un nuevo vehículo a la cuenta de un cliente específico.</td>
        <td style="padding: 6px; border: 1px solid #ddd;"><b>Body:</b> <code>CreateVehicleResource</code> (plate, brand, model, year, color, status, image, customerId).</td>
        <td style="padding: 6px; border: 1px solid #ddd;"><b>200 OK</b><br>Vehículo guardado.</td>
      </tr>
      <tr>
        <td style="padding: 6px; border: 1px solid #ddd; text-align: center;"><strong>GET</strong><br><code>/api/v1/vehicles</code></td>
        <td style="padding: 6px; border: 1px solid #ddd;">Devuelve la lista general de todos los vehículos registrados en el taller.</td>
        <td style="padding: 6px; border: 1px solid #ddd;">Ninguno.</td>
        <td style="padding: 6px; border: 1px solid #ddd;"><b>200 OK</b><br>Lista de vehículos.</td>
      </tr>
      <tr>
        <td style="padding: 6px; border: 1px solid #ddd; text-align: center;"><strong>GET</strong><br><code>/api/v1/vehicles/{id}</code></td>
        <td style="padding: 6px; border: 1px solid #ddd;">Obtiene las características técnicas detalladas de un vehículo en particular.</td>
        <td style="padding: 6px; border: 1px solid #ddd;"><b>Path:</b> <code>id</code> (integer).</td>
        <td style="padding: 6px; border: 1px solid #ddd;"><b>200 OK</b><br>Detalle de vehículo.</td>
      </tr>
      <tr>
        <td style="padding: 6px; border: 1px solid #ddd; text-align: center;"><strong>PUT</strong><br><code>/api/v1/vehicles/{id}</code></td>
        <td style="padding: 6px; border: 1px solid #ddd;">Modifica de forma integral las características o el estado asignado de un vehículo.</td>
        <td style="padding: 6px; border: 1px solid #ddd;"><b>Path:</b> <code>id</code> (integer)<br><b>Body:</b> <code>CreateVehicleResource</code>.</td>
        <td style="padding: 6px; border: 1px solid #ddd;"><b>200 OK</b><br>Vehículo modificado.</td>
      </tr>
      <tr>
        <td style="padding: 6px; border: 1px solid #ddd; text-align: center;"><strong>DELETE</strong><br><code>/api/v1/vehicles/{id}</code></td>
        <td style="padding: 6px; border: 1px solid #ddd;">Remueve la unidad automotriz del listado activo del sistema.</td>
        <td style="padding: 6px; border: 1px solid #ddd;"><b>Path:</b> <code>id</code> (integer).</td>
        <td style="padding: 6px; border: 1px solid #ddd;"><b>200 OK</b><br>Vehículo eliminado.</td>
      </tr>
      <tr style="background-color: #fafafa; font-weight: bold;"><td colspan="4" style="padding: 6px; border: 1px solid #ddd;">Módulo de Órdenes de Trabajo (WorkOrders)</td></tr>
      <tr>
        <td style="padding: 6px; border: 1px solid #ddd; text-align: center;"><strong>POST</strong><br><code>/api/v1/workorders</code></td>
        <td style="padding: 6px; border: 1px solid #ddd;">Abre un nuevo expediente u orden de servicio ligada a un vehículo y cliente.</td>
        <td style="padding: 6px; border: 1px solid #ddd;"><b>Body:</b> <code>CreateWorkOrderResource</code> (vehicleId, customerId, mechanicId, description, estimatedDate).</td>
        <td style="padding: 6px; border: 1px solid #ddd;"><b>200 OK</b><br>Orden creada.</td>
      </tr>
      <tr>
        <td style="padding: 6px; border: 1px solid #ddd; text-align: center;"><strong>GET</strong><br><code>/api/v1/workorders</code></td>
        <td style="padding: 6px; border: 1px solid #ddd;">Lista la totalidad de órdenes de servicio registradas en la base de datos.</td>
        <td style="padding: 6px; border: 1px solid #ddd;">Ninguno.</td>
        <td style="padding: 6px; border: 1px solid #ddd;"><b>200 OK</b><br>Lista de órdenes.</td>
      </tr>
      <tr>
        <td style="padding: 6px; border: 1px solid #ddd; text-align: center;"><strong>GET</strong><br><code>/api/v1/workorders/{id}</code></td>
        <td style="padding: 6px; border: 1px solid #ddd;">Obtiene el desglose, diagnóstico, plazos y mecánicos encargados de una orden específica.</td>
        <td style="padding: 6px; border: 1px solid #ddd;"><b>Path:</b> <code>id</code> (integer).</td>
        <td style="padding: 6px; border: 1px solid #ddd;"><b>200 OK</b><br>Detalle de la orden.</td>
      </tr>
      <tr>
        <td style="padding: 6px; border: 1px solid #ddd; text-align: center;"><strong>PUT</strong><br><code>/api/v1/workorders/{id}</code></td>
        <td style="padding: 6px; border: 1px solid #ddd;">Actualiza las verificaciones de control de calidad (limpieza, piezas, pruebas) y estado final de la orden.</td>
        <td style="padding: 6px; border: 1px solid #ddd;"><b>Path:</b> <code>id</code> (integer)<br><b>Body:</b> <code>UpdateWorkOrderResource</code> (description, estimatedDate, price, status, tasksCompleted, sparePartsChecked, diagnosisValidated, cleaningDone, finalTestDone).</td>
        <td style="padding: 6px; border: 1px solid #ddd;"><b>200 OK</b><br>Orden actualizada.</td>
      </tr>
    </tbody>
  </table>
</div>

<br>

<p align="justify">
A continuación, se presentan las capturas correspondientes que evidencian la disponibilidad de la interfaz interactiva sobre el entorno real en la nube, demostrando la consistencia de los contratos de datos mapeados.
</p>

<div align="center">
  <h5>Vista General de los Endpoints Documentados</h5>
  <img src="docs/assets/swagger_general.png" alt="Swagger UI General View" width="80%">
</div>

<br>

<div align="center">
  <h5>Detalle de Parámetros y Esquemas en Endpoint POST</h5>
  <img src="docs/assets/swagger_endpoint_detail.png" alt="Swagger UI Endpoint Detail" width="80%">
</div>

<br>

<div align="center">
  <h5>Prueba de Ejecución (Try it out) e Interacción con el API</h5>
  <img src="docs/assets/swagger_tryitout.png" alt="Swagger UI Endpoint Try it out" width="80%">
</div>

##### 5.2.3.7. Software Deployment Evidence for Sprint Review

<p align="justify">
En el presente apartado se detallan los procesos técnicos y las configuraciones ejecutadas para el despliegue de los distintos componentes de la solución de software durante el Sprint 3. Las actividades abarcaron desde la configuración de recursos en proveedores en la nube hasta la automatización de los flujos de integración y despliegue continuo (CI/CD), asegurando la disponibilidad productiva de la Landing Page, la Aplicación Web (Frontend) y los Servicios Web (Backend).
</p>

---

###### A. Componentes Desplegados y Entornos Cloud

<p align="justify">
Para garantizar el correcto funcionamiento distribuido de la arquitectura, se gestionó la publicación de tres artefactos principales en diferentes proveedores en la nube:
</p>

<ul>
  <li>
    <b>Landing Page (Sitio Web Estático):</b> Alojada y distribuida mediante GitHub Pages, garantizando una entrega rápida de la página promocional del producto.
    <br><b>URL:</b> <a href="https://innovatechstudio.github.io/Autoservice-landing-page-aw/" target="_blank">https://innovatechstudio.github.io/Autoservice-landing-page-aw/</a>
  </li>
  <li>
    <b>Web Application (Frontend):</b> Desplegada en la plataforma Microsoft Azure utilizando el servicio Azure Static Web Apps, integrado con flujos automatizados de compilación.
    <br><b>URL:</b> <a href="https://witty-meadow-063b9d310.7.azurestaticapps.net/login" target="_blank">https://witty-meadow-063b9d310.7.azurestaticapps.net/login</a>
  </li>
  <li>
    <b>Web Services (Backend API):</b> Hospedados en la plataforma Cloud de Render mediante la construcción y ejecución de un contenedor Docker, exponiendo la lógica de negocio y la conexión a la base de datos.
    <br><b>URL:</b> <a href="https://autoservice-aw-backend.onrender.com/swagger/index.html" target="_blank">https://autoservice-aw-backend.onrender.com/swagger/index.html</a>
  </li>
</ul>

---

###### B. Configuración Paso a Paso del Proceso de Despliegue

<p align="justify">
A continuación, se describen de manera secuencial los pasos realizados por el equipo de ingeniería para materializar el entorno productivo de la solución integral:
</p>

**Paso 1: Despliegue de la Landing Page (GitHub Pages)**
<p align="justify">
Se configuró el repositorio de la Landing Page para utilizar GitHub Pages. Desde la configuración del repositorio, se seleccionó la rama de producción y el directorio raíz para la publicación automática del HTML, CSS y JavaScript cada vez que se realiza una integración de cambios (Pull Request aprobado) en dicha rama.
</p>

**Paso 2: Automatización del Frontend en Azure Static Web Apps**
<p align="justify">
Para el componente cliente (Web Application), se provisionó un recurso dentro del portal de Azure. Este proceso generó automáticamente un archivo de flujo de trabajo (workflow) en GitHub Actions. Dicho flujo intercepta los cambios en la rama principal, instala las dependencias de Vue.js, compila los artefactos estáticos del lado del cliente y realiza el despliegue automático hacia los servidores de borde de Azure.
</p>

**Paso 3: Contenerización y Despliegue del Backend en Render**
<p align="justify">
Se estructuró un archivo <code>Dockerfile</code> en la raíz del proyecto ASP.NET Core para definir un entorno de compilación multi-etapa. Posteriormente, en el panel de administración de Render, se creó un recurso de tipo <i>Web Service</i> vinculado al repositorio del backend. Render automatiza la compilación de la imagen Docker ante cada actualización y expone el puerto HTTP configurado para producción, asegurando además la inyección de variables de entorno (como la cadena de conexión a la base de datos).
</p>

**Paso 4: Configuración de Políticas CORS**
<p align="justify">
Para permitir la correcta comunicación entre la Aplicación Web (alojada en Azure) y los Servicios Web (alojados en Render), se configuraron las políticas de Intercambio de Recursos de Origen Cruzado (CORS) en el archivo <code>Program.cs</code> del backend, autorizando explícitamente las peticiones HTTP provenientes del dominio de la aplicación web estática.
</p>

---

###### C. Evidencias Gráficas de Despliegue Exitoso

<p align="justify">
En cumplimiento con los criterios de validación de calidad, se presentan las capturas correspondientes a los paneles de administración en la nube y repositorios, demostrando el estado activo y el correcto funcionamiento de los flujos de despliegue:
</p>

<div align="center">
  <h5>Evidencia 1: Configuración Activa de GitHub Pages para la Landing Page</h5>
  <img src="docs/assets/deployment_githubpages.png" alt="GitHub Pages Deployment Evidence" width="80%">
</div>

<br>

<div align="center">
  <h5>Evidencia 2: Flujo de Compilación y Despliegue Exitoso en Azure (Frontend)</h5>
  <img src="docs/assets/deployment_azure_success.png" alt="Azure Static Web Apps Deployment Evidence" width="80%">
</div>

<br>

<div align="center">
  <h5>Evidencia 3: Consola de Administración y Estado "Live" en Render (Backend)</h5>
  <img src="docs/assets/deployment_render_success.png" alt="Render Web Service Deployment Evidence" width="80%">
</div>

##### 5.2.3.8. Team Collaboration Insights during Sprint

<p align="justify">
Durante el Sprint 3, el equipo mantuvo un flujo de trabajo colaborativo enfocado primordialmente en la implementación de los Web Services de AutoService utilizando C# y ASP.NET Core, así como en la actualización de la Web Application para lograr la integración completa. Para garantizar la organización del desarrollo y la estabilidad de la arquitectura, se aplicó estrictamente la estrategia GitFlow, utilizando ramas independientes para cada contexto delimitado (Bounded Context), funcionalidad o mejora implementada durante el Sprint.
</p>

<p align="justify">
Cada integrante trabajó sobre ramas <i>feature/*</i> y <i>hotfix/*</i>, integrando posteriormente sus avances mediante Pull Requests hacia la rama <code>develop</code>. Luego de las validaciones de las pruebas de integración y revisiones de código correspondientes, los cambios fueron consolidados hacia la rama <code>main</code> para su despliegue automático hacia los entornos productivos, utilizando contenedores Docker en Render para el backend y Azure Static Web Apps para el frontend.
</p>

<p align="justify">
La colaboración del equipo se evidenció principalmente en el diseño y desarrollo conjunto de los controladores RESTful, la implementación de la persistencia de datos con Entity Framework Core, la documentación interactiva con Swagger y la conexión exitosa entre el cliente web y los nuevos servicios. Asimismo, se aplicaron rigurosamente las convenciones de versionamiento utilizando <i>Conventional Commits</i>, permitiendo mantener una trazabilidad clara de cada cambio en la lógica de negocio y la infraestructura.
</p>

<p align="justify">
A continuación, se presentan los analíticos y evidencias extraídas directamente de los repositorios del proyecto, las cuales reflejan la actividad constante, integración colaborativa y organización técnica del equipo durante el Sprint 3.
</p>

<div align="center">

  <h5>Evidencia 1: Gráfico de contribuciones por integrante del equipo</h5>
  <img src="docs/assets/sprint3_contributors_graph.png" alt="Sprint 3 Contributors Graph" width="80%">

  <h5>Evidencia 2: Resumen de actividad del Sprint mediante GitHub Pulse</h5>
  <img src="docs/assets/sprint3_pulse_activity.png"  alt="Sprint 3 Pulse Activity" width="80%">

  <h5>Evidencia 3: Gestión colaborativa mediante Pull Requests y merges</h5>
  <img src="docs/assets/sprint3_closed_pull_requests.png" alt="Sprint 3 Closed Pull Requests" width="80%">

  <h5>Evidencia 4: Organización de ramas bajo estrategia GitFlow</h5>
  <img src="docs/assets/sprint3_gitflow_branches.png" alt="Sprint 3 GitFlow Branches" width="80%">

</div>

<br>

<p align="justify">
Las evidencias presentadas demuestran que el equipo mantuvo una participación activa y distribuida durante todo el Sprint, registrando commits significativos, integraciones frecuentes y despliegues continuos hacia los entornos en la nube. Asimismo, el uso de Pull Requests permitió centralizar la revisión del código en C# y asegurar la consistencia del Domain-Driven Design (DDD) antes de cada integración hacia las ramas principales de los repositorios.
</p>

<p align="justify">
Entre las actividades colaborativas más relevantes realizadas de forma conjunta durante este Sprint destacan:
</p>

<ul style="text-align: justify;">
  <li>Desarrollo de los <i>Bounded Contexts</i> y estructuración de la lógica de negocio en C# y ASP.NET Core.</li>
  <li>Implementación de la persistencia de datos relacional mediante migraciones de Entity Framework Core.</li>
  <li>Documentación interactiva de los endpoints y contratos de datos mediante OpenAPI (Swagger).</li>
  <li>Adaptación de los componentes del frontend para consumir los Web Services productivos y reemplazar la Fake API.</li>
  <li>Configuración de la contenerización (Dockerfile), variables de entorno y políticas CORS.</li>
  <li>Despliegue de los servicios en Render y sincronización continua con la aplicación en Azure.</li>
</ul>

<p align="justify">
El repositorio principal utilizado para el trabajo colaborativo de la capa de servicios durante este Sprint fue:
</p>

<p align="center">
  <code>
    <a href="https://github.com/InnovaTechStudio/AutoService-730-AW-Backend" target="_blank">https://github.com/InnovaTechStudio/AutoService-730-AW-Backend</a>
  </code>
</p>

### 5.3. Validation Interviews

#### 5.3.1. Diseño de Entrevistas

<strong>SEGMENTO 1: Mecánicoos Independientes</strong>
<ol>
  <li>Después de ver la página de AutoService, ¿cuál seria tu comemtatio principal sobre el problema que resolvemos para talleres como el tuyo? ¿Qué elemento o frase de la página te llamó más la atención y por qué? 
</li>
  <li>Para crear una orden de trabajo, ¿dónde buscarías la opción? ¿Qué datos son los más importantes para empezar?</li>
  <li>Al añadir una tarea y elegir materiales del inventario, ¿es fácil? ¿Qué información del material necesitas ver sí o sí?</li>
  <li>Qué 3 indicadores del dashboard revisarías cada mañana? ¿Falta alguno?</li>
  <li>Si te falta una pieza en medio de una reparación, ¿qué funcionalidad del inventario te ayudaría más?</li>
  <li>¿Estarias dispuesto a pagar por un plan que ofrece el sistema? ¿Qué plan de precios (Gratis, Pro, Business) elegirías para tu taller?</li>
  <li>¿Qué fue lo más confuso y lo más útil? Si cambiaras una cosa, ¿qué sería?</li>

</ol>


<p><strong>SEGMENTO 2: Dueños de Talleres</strong></p>
<p><em>Este segmento evalúa el contexto del negocio, la percepción del Landing Page, la usabilidad de los flujos principales y la retroalimentación general sobre la solución propuesta.</em></p>
<ol>
  <li><strong>¿Podrías contarme brevemente cómo está organizado tu taller o empresa y qué tamaño tiene el equipo?</strong>
    <br><em>Evalúa:</em> Contexto organizacional y tamaño del negocio para validar los segmentos de mercado objetivo.</li>
  <li><strong>¿Qué herramienta(s) usan actualmente para gestionar clientes, vehículos y órdenes de trabajo?</strong>
    <br><em>Evalúa:</em> Competencia actual y hábitos de trabajo para identificar oportunidades de diferenciación.</li>
  <li><strong>¿Qué problema principal enfrentan al coordinar trabajos y comunicar el avance a los clientes?</strong>
    <br><em>Evalúa:</em> Validación del problema central que AutoService busca resolver.</li>
  <li><strong>¿Cuál crees que es el propósito principal del Landing Page de AutoService?</strong>
    <br><em>Evalúa:</em> Claridad del mensaje y propuesta de valor transmitida en el Landing Page.</li>
  <li><strong>¿Qué entendiste que ofrece AutoService?</strong>
    <br><em>Evalúa:</em> Comprensión de las funcionalidades y beneficios clave de la plataforma.</li>
  <li><strong>¿Te pareció claro cuál es el siguiente paso después de ver el Landing Page?</strong>
    <br><em>Evalúa:</em> Efectividad del Call to Action y claridad del funnel de conversión.</li>
  <li><strong>¿Qué parte del Landing Page te resultó más útil?</strong>
    <br><em>Evalúa:</em> Identificación de los elementos más valiosos para el usuario.</li>
  <li><strong>¿Qué parte del Landing Page te pareció confusa o difícil de entender?</strong>
    <br><em>Evalúa:</em> Detección de áreas de mejora en la comunicación y diseño del Landing Page.</li>
  <li><strong>¿Cómo describirías el proceso de registro o acceso a la aplicación?</strong>
    <br><em>Evalúa:</em> Intuición y facilidad del flujo de onboarding.</li>
  <li><strong>¿Te parece claro qué datos debes ingresar para iniciar sesión o registrarte?</strong>
    <br><em>Evalúa:</em> Claridad de los campos requeridos en el formulario de autenticación.</li>
  <li><strong>Si quisieras crear una orden de trabajo, ¿sabes qué información debes ingresar?</strong>
    <br><em>Evalúa:</em> Comprensión de los datos mínimos necesarios para crear una orden de trabajo.</li>
  <li><strong>¿Te resulta fácil identificar dónde agregar cliente, vehículo y servicio?</strong>
    <br><em>Evalúa:</em> Usabilidad de la navegación y jerarquía de información en la interfaz.</li>
  <li><strong>¿Puedes ver con claridad el estado actual de una orden de trabajo?</strong>
    <br><em>Evalúa:</em> Visibilidad y claridad del seguimiento de estados de las órdenes.</li>
  <li><strong>¿Quedó claro cómo se actualiza el progreso de un trabajo?</strong>
    <br><em>Evalúa:</em> Comprensión del flujo de actualización de tareas y su reflejo en el progreso.</li>
  <li><strong>¿Entendiste cómo se notifica al cliente sobre el avance del servicio?</strong>
    <br><em>Evalúa:</em> Claridad del sistema de notificaciones y comunicación con el cliente.</li>
  <li><strong>¿Qué aspecto cambiarías primero para que la aplicación sea más útil?</strong>
    <br><em>Evalúa:</em> Identificación de prioridades de mejora desde la perspectiva del dueño de taller.</li>
  <li><strong>¿Usarías AutoService si estuviera disponible hoy? ¿Por qué?</strong>
    <br><em>Evalúa:</em> Intención de uso y percepción general de valor de la solución.</li>
</ol>

#### 5.3.2. Registro de Entrevistas

#### Entrevista 1: Técnico Independiente

- **Nombre:** David Klisman Paredes
- **Edad:** 24
- **Residencia:** Lima, Surco 
- **Ocupación:** Técnico Mecánico Automotriz  

- **Inicio:** 0:34 
- **Duración:** 

**Link:**  
[Ver video](https://upcedupe-my.sharepoint.com/:v:/g/personal/u20241d185_upc_edu_pe/IQBDv0iKhKtESLAQ9iFYBZ-7Abkdhh1HzTCEaXD5VrUCK_0?e=fnTCzd)

**Resumen:**
<p style="text-align: justify;">
Durante la entrevista, el participante identificó que la plataforma AutoService resuelve principalmente el desorden operativo y la pérdida de tiempo en los talleres, destacando la gestión centralizada de tareas, órdenes de trabajo e inventario. Valoró positivamente la propuesta de control y confianza transmitida en la landing page, así como la estructura visual de la plataforma. Sugirió hacer más visible la creación de órdenes de trabajo mediante accesos directos o favoritos, incorporar autocompletado para tareas repetitivas y facilitar la consulta rápida del stock de repuestos. Los indicadores más relevantes para él son la cantidad de vehículos en el taller, las entradas programadas y los ingresos generados. Respecto a los planes, optaría inicialmente por el plan gratuito para evaluar la herramienta antes de migrar a una opción superior según sus necesidades. Como mejora, recomendó implementar un modo oscuro y reforzar algunas funcionalidades relacionadas con la gestión de inventario y compras.
</p>

**Evidencia:**

![Entrevista Tencnico Taller](docs/assets/interview-validate/inter-validate-m1.png)

---
#### Entrevista 2: Técnico Independiente

- **Nombre:** Antenor Ayala
- **Edad:** 32
- **Residencia:** Ayacucho, Huamanga
- **Ocupación:** Técnico Mecánico Automotriz  

- **Inicio:** 0:24 
- **Duración:** 8:40

**Link:**  
[Ver video](https://upcedupe-my.sharepoint.com/:v:/g/personal/u20241d185_upc_edu_pe/IQBXMt0MwDxHTrXJ1c65IOT7AcAH-dWDwYEQ1vPeY50nAzE?e=TIxuLC)

**Resumen:**
<p style="text-align: justify;">
El entrevistado mostró una percepción muy positiva de AutoService, destacando que la plataforma puede ayudar a organizar mejor las tareas, el inventario y la gestión diaria del taller. Consideró que el sistema sería útil para complementar el trabajo manual y facilitar el control de repuestos y procesos. Como sugerencia principal, indicó que la plataforma debería ser más accesible y fácil de conocer para usuarios con poca experiencia en herramientas digitales, además de mejorar su difusión. Valoró especialmente la posibilidad de consultar inventarios y propuso funciones como la ubicación exacta de piezas dentro del taller y acceso rápido a proveedores cuando no haya stock disponible. Respecto a los planes, manifestó que inicialmente probaría una versión gratuita, pero estaría dispuesto a migrar al plan Pro si percibe beneficios claros y genera confianza. Finalmente, resaltó que la interfaz es atractiva, organizada e innovadora, aunque considera importante simplificar el acceso para usuarios menos familiarizados con la tecnología y ampliar las funcionalidades del plan básico.
</p>

**Evidencia:**

![Entrevista Tencnico Taller](docs/assets/interview-validate/inter-validate-m2.png)

---
#### Entrevista 3: Administrador

- **Nombre y Apellido:** Juan Calisaya
- **Edad:** 30 años
- **Distrito de Residencia:** Santa Anita, Lima
- **Ocupación:** Propietario y Administrador de Taller Automotriz
- **Fecha:** 18 de junio de 2026
- **Inicio de la Entrevista:** 00:01
- **Duración:** 12:49

**URL del Video (Microsoft Stream):**  
[Ver video](https://upcedupe-my.sharepoint.com/:v:/g/personal/u20241e299_upc_edu_pe/IQAKH0LwbS9hR6iCQO9yvjKpAQVicbqjpS3d1hd_KQnQm9o?e=3eALzP&nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJTdHJlYW1XZWJBcHAiLCJyZWZlcnJhbFZpZXciOiJTaGFyZURpYWxvZy1MaW5rIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXcifX0%3D)



<p style="text-align: justify;">
Juan Calisaya es propietario y administrador de un taller automotriz que cuenta con cuatro colaboradores y atiende entre 15 y 20 vehículos por semana. Actualmente gestiona la información mediante registros manuales, hojas de cálculo en Excel y comunicación con clientes a través de WhatsApp.

Durante la validación, comprendió correctamente que AutoService es una solución orientada a la gestión digital de talleres automotrices, permitiendo centralizar la información de clientes, vehículos y órdenes de trabajo. Consideró que el Landing Page comunica adecuadamente la propuesta de valor y facilita la comprensión de los beneficios ofrecidos por la plataforma.

Respecto a la aplicación, destacó la facilidad del proceso de registro y la organización intuitiva de los módulos. Logró identificar sin dificultad los procesos de registro de clientes, vehículos y órdenes de trabajo, así como los mecanismos de asignación de tareas y seguimiento de servicios. Asimismo, comprendió claramente los estados de avance de las órdenes de trabajo y el funcionamiento del sistema de notificaciones para mantener informados a los clientes.

Como sugerencia de mejora, propuso incorporar reportes de productividad y estadísticas operativas para apoyar la toma de decisiones dentro del taller. Finalmente, manifestó que utilizaría AutoService debido a los beneficios relacionados con la centralización de la información, la mejora de la comunicación con los clientes y la optimización de los procesos administrativos.
</p>

**Evidencia:** 
![Entrevista Administrador](docs/assets/interview-validate/inter-validate-admin1.png)

---
#### Entrevista 4: Administrador

- **Nombre y Apellido:** Sebastián Rojas
- **Edad:** 24 años
- **Distrito de Residencia:** Villa El Salvador, Lima
- **Ocupación:** Administrador y Encargado de Logística de Taller Automotriz
- **Fecha:** 18 de junio de 2026
- **Inicio de la Entrevista:** 00:04
- **Duración:** 10:55

**URL del Video (Microsoft Stream):** 
[Ver video](https://upcedupe-my.sharepoint.com/:v:/g/personal/u20241e299_upc_edu_pe/IQDAeIojk9-qRp0t-QPDNmzpAb58CmafSrSigXD0jIsM48U?e=nucE9d&nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJTdHJlYW1XZWJBcHAiLCJyZWZlcnJhbFZpZXciOiJTaGFyZURpYWxvZy1MaW5rIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXcifX0%3D)


<p style="text-align: justify;">
Sebastián Rojas se desempeña como administrador y encargado de logística de un taller automotriz que atiende aproximadamente entre 15 y 20 vehículos por semana. Actualmente la gestión de información se realiza principalmente mediante hojas de cálculo en Excel, registros en WhatsApp y documentación física para respaldar procesos administrativos y operativos.

Durante la evaluación del Landing Page, identificó correctamente que AutoService busca digitalizar y optimizar la gestión de talleres automotrices mediante herramientas que permiten organizar clientes, vehículos, órdenes de trabajo y procesos internos. Consideró que la propuesta de valor es clara y que la plataforma puede contribuir a reducir errores relacionados con el manejo de información y la coordinación de actividades.

En la validación de la aplicación, destacó la simplicidad del proceso de registro y la facilidad para comprender el flujo de trabajo propuesto por el sistema. Logró identificar correctamente las etapas necesarias para registrar clientes, asociar vehículos y crear órdenes de trabajo. Asimismo, valoró positivamente la posibilidad de asignar tareas a los mecánicos, realizar seguimiento al avance de los servicios y mantener una visión centralizada de la operación del taller.

Respecto al monitoreo de servicios, comprendió cómo se actualizan los estados de las órdenes de trabajo y cómo los avances registrados por los colaboradores pueden utilizarse para informar a los clientes sobre el progreso de sus vehículos. Consideró que esta funcionalidad mejora la transparencia y facilita la comunicación entre el taller y sus clientes.

Como principal sugerencia de mejora, recomendó incorporar reportes avanzados relacionados con ingresos, productividad de colaboradores, rendimiento operativo y estadísticas para la toma de decisiones estratégicas. Finalmente, indicó que utilizaría AutoService debido a que ofrece una gestión más colaborativa, organizada y eficiente que las herramientas que emplea actualmente.
</p>

**Evidencia:** 
![Entrevista Administrador](docs/assets/interview-validate/inter-validate-admin2.png)


---
#### Entrevista 5: Administrador

- **Nombre y Apellido:** Jaime Ruiz
- **Edad:** 30 años
- **Distrito de Residencia:** Puno, Puno
- **Ocupación:** Dueño y Administrador de Taller Automotriz
- **Fecha:** 18 de junio de 2026
- **Inicio de la Entrevista:** 00:14
- **Duración:** 15:18

**URL del Video (Microsoft Stream):** 
[Ver video](https://upcedupe-my.sharepoint.com/:v:/g/personal/u20241e299_upc_edu_pe/IQASv_VScko6S7Lj2qfoNu1NASDn0X3oJZCkGj95LjlQ0j8?nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJTdHJlYW1XZWJBcHAiLCJyZWZlcnJhbFZpZXciOiJTaGFyZURpYWxvZy1MaW5rIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXcifX0%3D&e=FNLJy0)


<p style="text-align: justify;">
Jaime Ruiz es dueño y administrador de un taller automotriz ubicado en la ciudad de Puno. Su negocio atiende aproximadamente entre 15 y 20 vehículos por semana y cuenta con personal encargado de atención al cliente y actividades operativas relacionadas con el mantenimiento y reparación de vehículos. Actualmente, la gestión de la información se realiza principalmente mediante hojas de cálculo en Excel, comunicación por WhatsApp y registros manuales para el seguimiento de clientes y servicios.

Durante la validación del Landing Page, el entrevistado identificó correctamente que AutoService es una plataforma orientada a mejorar la gestión y organización de talleres automotrices. Comprendió que la solución permite realizar un seguimiento más eficiente de los vehículos, mejorar la comunicación con los clientes y optimizar el control de los procesos internos del negocio. Asimismo, destacó especialmente la funcionalidad relacionada con el seguimiento de órdenes de trabajo y el monitoreo del estado de los vehículos, ya que considera que los clientes valoran conocer el progreso de los servicios realizados.

Respecto a la aplicación web, indicó que el proceso de registro e inicio de sesión es sencillo, intuitivo y accesible para usuarios con conocimientos tecnológicos básicos. Señaló que los formularios presentan claramente la información requerida y permiten comprender fácilmente el flujo general de la plataforma.

Durante la evaluación de los módulos principales, Jaime logró identificar correctamente el proceso para registrar clientes, asociar vehículos y generar órdenes de trabajo. Comprendió que la plataforma permite almacenar información relevante del cliente, incluyendo datos de contacto, información del vehículo y detalles relacionados con las fallas o servicios solicitados. Asimismo, destacó la posibilidad de asignar mecánicos responsables y realizar un seguimiento detallado de cada trabajo realizado.

El entrevistado también valoró positivamente la organización de la información dentro de la plataforma, indicando que facilita el acceso a los datos de clientes recurrentes y contribuye a fortalecer la relación con ellos mediante un mejor control de los servicios realizados. Consideró que esta funcionalidad puede favorecer la fidelización de clientes y mejorar la calidad del servicio brindado por el taller.

En relación con el monitoreo de órdenes de trabajo, manifestó que los estados de avance son claros y permiten identificar rápidamente si un servicio se encuentra pendiente, en proceso o finalizado. Además, destacó que esta información facilita la supervisión del trabajo realizado por los colaboradores y mejora la coordinación interna del taller.

Respecto al flujo general de la aplicación, indicó que la estructura basada en clientes, vehículos y órdenes de trabajo resulta lógica y fácil de comprender. Consideró que la secuencia de operaciones refleja adecuadamente el proceso real que se sigue dentro de un taller automotriz y permite mantener un mejor control sobre cada servicio realizado.

Como sugerencia de mejora, propuso incorporar reportes de productividad y estadísticas relacionadas con los servicios ejecutados, con el objetivo de apoyar la toma de decisiones y proporcionar una visión más completa del desempeño del negocio. Consideró que este tipo de información sería valiosa para optimizar la gestión operativa y administrativa del taller.

Finalmente, Jaime Ruiz manifestó que utilizaría AutoService si estuviera disponible comercialmente, ya que considera que la plataforma le permitiría centralizar la información de clientes, colaboradores, vehículos y repuestos en un único sistema. Asimismo, destacó que la solución contribuiría a mejorar la comunicación con los clientes, reducir el tiempo destinado a tareas administrativas y aumentar la eficiencia de las operaciones diarias del taller.
</p>

**Evidencia:** 
![Entrevista Administrador](docs/assets/interview-validate/inter-validate-admin3.png)



#### 5.3.3. Evaluaciones según heurísticas
**UX Heuristics & Principles Evaluation**  
**Usability – Inclusive Design – Information Architecture**

**CARRERA		:** Ingeniería de Software  
**CURSO		:** Aplicaciones Web  
**SECCIÓN		:** 17953  
**PROFESORES		:** Todos  
**AUDITOR		:** PircaIndustries  
**CLIENTE		:** Francia Torres, Jhony Manuel, Montoya Nina, Paula Fernanda, Palacios Tinoco Adrian Fernando, Ramos Hinostroza, Diego Antonio y Ramos Mera, Neo Daniel.

## 

## **SITE o APP A EVALUAR:**

## AutoService

## **TAREAS A EVALUAR:**

El alcance de esta evaluación incluye la revisión de la usabilidad de las siguientes tareas:

1. Landing Page  
2. Registro e Inicio Sesión  
3. Panel Principal  
4. Clientes  
5. Vehículos  
6. Inventario y Repuestos

No están incluidas en esta versión de la evaluación las siguientes tareas:

1. Notificaciones  
2. Configuraciones de accesibilidad

## **ESCALA DE SEVERIDAD:**

*Los errores serán puntuados tomando en cuenta la siguiente escala de severidad*

| *Nivel* | *Descripción* |
| :---- | :---- |
| *1* | *Problema superficial: puede ser fácilmente superado por el usuario o ocurre con muy poca frecuencia. No necesita ser arreglado a no ser que exista disponibilidad de tiempo.* |
| *2* | *Problema menor: puede ocurrir un poco más frecuentemente o es un poco más difícil de superar para el usuario. Se le debería asignar una prioridad baja resolverlo de cara al siguiente reléase* |
| *3* | *Problema mayor: ocurre frecuentemente o los usuarios no son capaces de resolverlos. Es importante que sean corregidos y se les debe asignar una prioridad alta.* |
| *4* | *Problema muy grave: un error de gran impacto que impide al usuario continuar con el uso de la herramienta. Es imperativo que sea corregido antes del lanzamiento.* |

## **TABLA RESUMEN:**

| *\#* | *Problema* | *Escala de severidad* | *Heurística/Principio violada(o)* |
| :---: | ----- | :---: | ----- |
| 1 | Logotipo de tamaño muy reducido en encabezado y pie de página | 2 | Diseño estético y minimalista |
| 2 | Imagen descentrada con margen inferior desproporcionado | 1 | Diseño estético y minimalista |
| 3 | Inconsistencia en la altura de los botones de navegación | 1 | Heurística 4: Consistencia y estándares |
| 4 | Botones de navegación (flechas) inactivos | 3 | Control y libertad del usuario |
| 5 | Envío de formulario sin validación de campos vacíos | 3 | Prevención de errores |
| 6 | Falta de traducción en el título del portal de seguimiento | 2 | Consistencia y estándares |
| 7 | Texto del marcador de posición (placeholder) cortado | 2 | Diseño estético y minimalista |
| 8 | Ausencia de logotipo o nombre comercial en vistas de autenticación | 2 | Reconocimiento antes que recuerdo |
| 9 | Ausencia de mensajes de error al enviar formularios vacíos | 3 | Ayudar a los usuarios a reconocer, diagnosticar y recuperarse de errores |
| 10 | Duplicidad de registros por falta de control de peticiones simultáneas en el formulario de creación de vehículo | 3 | Usability: “Prevención de errores” y “Visibilidad del estado del sistema” |
| 11 | Distorsión visual y recorte inadecuado en la previsualización de la imagen del vehículo | 2 | Usability: “Relación entre el sistema y el mundo real” y “Estética y diseño minimalista” |
| 12 | Ausencia de mensajes de validación y feedback visual ante el envío de campos obligatorios vacíos | 3 | Usability: “Ayuda a los usuarios a reconocer, diagnosticar y recuperarse de errores” y “Visibilidad del estado del sistema” |
| 13 | Presencia de etiquetas de traducción sin procesar (raw keys) en la pantalla de detalle del vehículo | 2 | Information Architecture: “Rotulado” |
| 14 | Duplicidad en el registro de clientes debido a la falta de bloqueo en peticiones simultáneas del formulario de registro de cliente | 3 | Usability: “Prevención de errores” y “Visibilidad del estado del sistema” |
| 15 | Presencia de claves de localización rotas (raw translation keys) en modales de edición y eliminación de clientes | 2 | Information Architecture: “Rotulado” |
| 16 | Despliegue de errores críticos mediante diálogos de alerta nativos del navegador | 2 | Usability: “Ayuda a los usuarios a reconocer, diagnosticar y recuperarse de errores” y “Consistencia y estándares”. |
| 17 | Sobreposición de los inputs para ingresar nuevo artículo | 2 | Diseño estético y minimalista |
| 18 | Overflow en el formulario no controlado | 2 | Diseño estético y minimalista |
| 19 | Internacionalización a medias | 2 | Relación entre el sistema y el mundo real  |
| 20 | Interfaz duplicada y sin respetar espacios | 2 | Prevención de errores (Heurística \#5) / Flexibilidad y eficiencia de uso (Heurística \#7)  |
| 21 | Selector de filtrado por mecánico vacío y sin estado inicial claro | 2 | Prevención de errores (Heurística \#5) / Visibilidad del estado del sistema (Heurística \#1)   |
| 22 | Falta de control de estados vacíos (Empty States) cuantitativos en el Panel Principal | 1 | Reconocimiento antes que recuerdo (Heurística \#6) / Estética y diseño minimalista (Heurística \#8) |

## 

## **DESCRIPCIÓN DE PROBLEMAS:**

**PROBLEMA \#1: Logotipo de tamaño muy reducido en encabezado y pie de página**

Severidad: 2

Heurística violada: Diseño estético y minimalista 

Problema: El logotipo de la empresa presenta dimensiones muy reducidas, lo que dificulta su correcta apreciación tanto en el encabezado (header) como en el pie de página (footer) de la plataforma.

<img width="886" height="125" alt="Image" src="https://github.com/user-attachments/assets/6ec32309-fc93-4185-b245-c90197783347" />

<img width="886" height="158" alt="Image" src="https://github.com/user-attachments/assets/e6df9516-42a5-4174-82be-12c511c1b39a" />

Recomendación; Aumentar el tamaño y la proporción del logotipo para asegurar la legibilidad y reforzar la identidad visual de la marca en todas las pantallas.

**PROBLEMA \#2: Imagen descentrada con margen inferior desproporcionado**

Severidad: 1

Heurística violada: Diseño estético y minimalista

Problema: La imagen ilustrativa en la sección que presenta el problema y la solución no se encuentra centrada, presentando un espacio vacío desproporcionado en su parte inferior. 

<img width="886" height="513" alt="Image" src="https://github.com/user-attachments/assets/7f93766f-ae09-4e4c-b704-0298f31a0ee7" />

Recomendación;  Ajustar los estilos CSS de la imagen y su contenedor para asegurar una alineación simétrica y eliminar el espacio residual innecesario. 

**PROBLEMA \#3: Inconsistencia en la altura de los botones de navegación**

Severidad: 1

Heurística violada: Consistencia y estándares

Problema: Los botones de acción ubicados en la barra de navegación ("Login" y el selector de idioma "ES") presentan alturas diferentes, lo cual rompe la consistencia visual de la interfaz. 

<img width="886" height="60" alt="Image" src="https://github.com/user-attachments/assets/f3aee22c-2183-4fd5-b700-894959929e0e" />

Recomendación;  Homogeneizar las dimensiones (altura y padding) de todos los elementos interactivos dentro de la barra de navegación para mantener un estándar visual.

**PROBLEMA \#4: Botones de navegación (flechas) inactivos**

Severidad: 3

Heurística violada: Control y libertad del usuario

Problema: En la sección "Designed for simplicity and real workshop needs", los controles de navegación (flechas direccionales) no ejecutan ninguna acción ni retroalimentación al ser presionados por el usuario.

<img width="886" height="431" alt="Image" src="https://github.com/user-attachments/assets/2a6e9455-9df3-4585-b81c-2fb520d574f5" />

Recomendación;  Implementar la interactividad correspondiente al carrusel de imágenes, o en su defecto, ocultar dichos controles hasta que la funcionalidad esté completamente desarrollada. 

**PROBLEMA \#5: Envío de formulario sin validación de campos vacíos**

Severidad: 3

Heurística violada: Prevención de errores

Problema: El formulario de contacto permite el envío de datos completamente vacíos, mostrando erróneamente un mensaje modal de confirmación exitosa ("Message sent\!"). 

<img width="886" height="629" alt="Image" src="https://github.com/user-attachments/assets/66448cbf-e6ec-4c29-99d4-2affc1d5563c" />

Recomendación;  Establecer validaciones obligatorias en los campos del formulario y deshabilitar el botón de envío ("Send Message") hasta que todos los datos requeridos sean ingresados correctamente.

**PROBLEMA \#6: Falta de traducción en el título del portal de seguimiento**

Severidad: 2

Heurística violada: Consistencia y estándares

Problema: Al interactuar con el inicio de sesión y seleccionar el idioma inglés ("EN"), al navegar hacia la sección "Are you a customer of the workshop?", el título principal ("Portal de Seguimiento") permanece en español, generando inconsistencia en la localización.

<img width="427" height="661" alt="Image" src="https://github.com/user-attachments/assets/610b7426-d2fd-4a2b-a707-54d841c2aac9" />

<img width="700" height="488" alt="Image" src="https://github.com/user-attachments/assets/76651783-e552-49c0-8f9a-710498b98bd3" />

Recomendación;  Revisar y asegurar que las variables de internacionalización (i18n) cubran la totalidad de los elementos de texto en las vistas cuando se alterna entre idiomas.

**PROBLEMA \#7: Texto del marcador de posición (placeholder) cortado**

Severidad: 2

Heurística violada: Diseño estético y minimalista

Problema: En el portal de seguimiento, el texto indicativo (placeholder) dentro del campo de texto en la versión en español excede el límite visible y se recorta ("Ingresa el código de tu orc...").

<img width="886" height="663" alt="Image" src="https://github.com/user-attachments/assets/3ec813cd-f8b0-4596-96ab-f5195d080521" />

Recomendación;  Reducir la longitud del texto del marcador de posición o incrementar el ancho del campo de entrada para garantizar que las instrucciones sean completamente visibles.

**PROBLEMA \#8: Ausencia de logotipo o nombre comercial en vistas de autenticación**

Severidad: 2

Heurística violada: Reconocimiento antes que recuerdo

Problema: Las pantallas destinadas al inicio de sesión y al registro carecen de elementos de identidad corporativa, no encontrándose presente ni el logotipo ni el nombre del producto de manera explícita. 

<img width="886" height="473" alt="Image" src="https://github.com/user-attachments/assets/b52d4341-41e6-42de-b894-7f70b301f2bb" />

Recomendación;  Incorporar el logotipo o el nombre comercial de la plataforma en la parte superior del formulario de autenticación para otorgar contexto inmediato al usuario. 

**PROBLEMA \#9: Ausencia de mensajes de error al enviar formularios vacíos**

Severidad: 3

Heurística violada: Ayudar a los usuarios a reconocer, diagnosticar y recuperarse de errores

Problema: Al accionar los botones de confirmación en las vistas de inicio de sesión y registro sin haber completado la información, el sistema omite generar mensajes de advertencia o retroalimentación visual sobre la obligatoriedad de los campos.

<img width="575" height="639" alt="Image" src="https://github.com/user-attachments/assets/2dd73106-8c96-4486-8ddd-73c0a5d14a11" /><img width="575" height="639" alt="Image" src="https://github.com/user-attachments/assets/cf280474-9c46-4400-82fb-f8fa4aec52f9" />

Recomendación;  Añadir mensajes de error explícitos adyacentes a los campos vacíos (por ejemplo, textos en color rojo) y aplicar estilos de error en los bordes de las cajas de texto cuando la validación falla.

**PROBLEMA \#10: Duplicidad de registros por falta de control de peticiones simultáneas en el formulario de creación de vehículo**

Severidad: 3

Heurística violada: Usabilidad \- “Prevención de errores” y “Visibilidad del estado del sistema” 

Problema: Al hacer clic en el botón "Guardar" del modal de creación de vehículo, el sistema experimenta un tiempo de latencia sin ofrecer retroalimentación visual inmediata. Durante este intervalo, la interfaz mantiene el botón interactivo y el modal abierto. Si el usuario hace clic múltiples veces por frustración o incertidumbre, la aplicación procesa cada pulsación de manera independiente, lo que resulta en la inserción de registros duplicados en el listado de vehículos (como se observa con las dos tarjetas idénticas de placa 12345678 asociadas a Juan Pérez).

<img width="865" height="414" alt="Image" src="https://github.com/user-attachments/assets/10c267d1-4c5e-45e1-9212-a0713a8180e0" />

<img width="868" height="415" alt="Image" src="https://github.com/user-attachments/assets/106f6773-94e1-4f98-9b37-9be9d8187260" />

Recomendación:  Implementar un estado de carga visual en el botón "Guardar" al recibir el primer clic (por ejemplo, mostrando un indicador giratorio o spinner y cambiando el texto a "Guardando..."). De manera simultánea, se debe deshabilitar temporalmente el botón "Guardar" y el botón "Cancelar" para evitar interacciones repetidas mientras se procesa la solicitud. El modal solo debe cerrarse una vez que el flujo se haya completado con éxito, refrescando la vista principal.

**PROBLEMA \#11: Distorsión visual y recorte inadecuado en la previsualización de la imagen del vehículo**

Severidad: 2

Heurística violada: Usabilidad \- “Relación entre el sistema y el mundo real” y “Estética y diseño minimalista”

Problema: Al adjuntar una imagen del vehículo en el formulario de creación, la caja de previsualización de la interfaz no respeta el formato o relación de aspecto original de la fotografía. El contenedor obliga a la imagen a ajustarse a un formato extremadamente apaisado y recortado (solo visible como una franja del cielo en la primera captura). Esta distorsión dificulta que el usuario verifique visualmente si cargó la fotografía correcta antes de guardarla.

<img width="886" height="425" alt="Image" src="https://github.com/user-attachments/assets/39b2bce0-783e-44a6-9b43-53078f972989" />

Recomendación:  Ajustar el contenedor de la imagen en la interfaz del frontend para que mantenga una relación de aspecto estándar (como 16:9 o 4:3) y aplique técnicas de escalado que aseguren que el automóvil quede centrado y completamente visible dentro de la caja de previsualización sin recortarse de forma drástica. Se sugiere añadir un botón para "Reemplazar imagen" o "Eliminar" directamente en la miniatura de previsualización.

**PROBLEMA \#12: Ausencia de mensajes de validación y feedback visual ante el envío de campos obligatorios vacíos**

Severidad: 3

Heurística violada: Usabilidad \- “Ayuda a los usuarios a reconocer, diagnosticar y recuperarse de errores” y “Visibilidad del estado del sistema”

Problema: Cuando el usuario hace clic en el botón "Guardar" sin haber completado los campos requeridos marcados con asterisco rojo (Cliente propietario \* y Placa \*), la interfaz bloquea el registro del vehículo (comportamiento correcto), pero no proporciona ninguna indicación visual del error. El usuario no recibe notificaciones de texto, resaltados en rojo en los campos vacíos ni mensajes flotantes que indiquen qué información falta completar, lo cual genera incertidumbre sobre si el botón funciona correctamente.

<img width="886" height="425" alt="Image" src="https://github.com/user-attachments/assets/bbd128be-b01b-48c3-b7c6-2fde8415e44b" />

Recomendación:  Al presionar "Guardar", si existen campos obligatorios vacíos, la interfaz debe cancelar el envío, enfocar automáticamente el primer campo con error, resaltar los bordes de los campos vacíos en color de advertencia (rojo) y mostrar un mensaje descriptivo inmediatamente debajo de ellos (ej. "Este campo es obligatorio"). Opcionalmente, se puede mostrar una alerta emergente (toast notification) en la esquina superior del panel indicando al usuario que revise el formulario.

**PROBLEMA \#13: Presencia de etiquetas de traducción sin procesar (raw keys) en la pantalla de detalle del vehículo**

Severidad: 2

Heurística violada: Arquitectura de la Información \- “Rotulado”

Problema: En la ficha informativa del propietario del vehículo, la etiqueta correspondiente al correo electrónico se muestra en la pantalla como common.email en lugar de una etiqueta amigable y legible para el usuario en su respectivo idioma (como "Correo electrónico" o "Email"). Esto denota una falta de localización en el frontend y reduce la calidad visual del producto ante el administrador.

<img width="886" height="425" alt="Image" src="https://github.com/user-attachments/assets/5b2ad70c-824d-45e5-aef5-07b2101a6b78" />

Recomendación:  Reemplazar el identificador técnico de la cadena de traducción (common.email) en el frontend por su valor localizado correspondiente en español ("Correo electrónico") e inglés ("Email"), asegurando que la interfaz resuelva correctamente las propiedades del diccionario de traducción antes de renderizar la vista.

**PROBLEMA \#14: Duplicidad en el registro de clientes debido a la falta de bloqueo en peticiones simultáneas del formulario de registro de cliente**

Severidad: 3

Heurística violada: Usabilidad \- “Prevención de errores” y “Visibilidad del estado del sistema”

Problema: Al guardar un nuevo cliente ("Jhon Hernandez"), el botón "Guardar" no se deshabilita ni muestra un indicador de carga durante el proceso de almacenamiento. Si el usuario realiza múltiples clics consecutivos en el botón antes de que el servidor responda, la interfaz ejecuta múltiples peticiones de inserción. Esto se evidencia en la vista del listado de clientes, donde aparecen tres registros idénticos con el mismo DNI y datos de contacto creados en el mismo instante.

<img width="886" height="425" alt="Image" src="https://github.com/user-attachments/assets/7953bbdc-d90c-4199-b16b-e3c435c87538" /><img width="886" height="425" alt="Image" src="https://github.com/user-attachments/assets/c74db998-1185-4316-9963-5d25731d543d" />

Recomendación: Deshabilitar los botones de acción ("Guardar" y "Cancelar") inmediatamente después del primer clic y añadir un indicador de carga (spinner) en el interior del botón principal. El formulario debe limpiarse y cerrarse de manera automática solo cuando se confirme que la petición de guardado ha sido exitosa.

**PROBLEMA \#15: Presencia de claves de localización rotas (raw translation keys) en modales de edición y eliminación de clientes**

Severidad: 2

Heurística violada: Arquitectura de la Información \- “Rotulado”

Problema: Al interactuar con el módulo de clientes, varios textos clave de la interfaz no se renderizan correctamente y exponen nombres de variables del sistema en lugar de texto en lenguaje natural. Se identifican las siguientes etiquetas rotas:

* **Modal de edición:** “customers.form.editTitle” (Título) y “customers.form.update” (Botón de confirmación).  
* **Modal de eliminación:** “customers.delete.title” (Título), “customers.delete.description” (Descripción), “customers.delete.cancel” (Botón de cancelar) y “customers.delete.confirm” (Botón de confirmar). Esto afecta negativamente la confianza del usuario final en la madurez técnica de la aplicación.

<img width="886" height="425" alt="Image" src="https://github.com/user-attachments/assets/974629b8-ff29-4144-9f80-498b240f1c24" /><img width="886" height="425" alt="Image" src="https://github.com/user-attachments/assets/468d6d47-7ab1-4cd7-a9b1-bee3ec08a2b0" />

Recomendación: Configurar y mapear adecuadamente las claves correspondientes en los archivos de localización de idiomas del frontend (español e inglés). Asegurar que la librería de traducción se inicialice antes de renderizar estos modales dinámicos.

**PROBLEMA \#16: Despliegue de errores críticos mediante diálogos de alerta nativos del navegador**

Severidad: 2

Heurística violada: Usabilidad \- “Ayuda a los usuarios a reconocer, diagnosticar y recuperarse de errores” y “Consistencia y estándares”.

Problema: Cuando ocurre un fallo técnico al intentar eliminar un cliente (por ejemplo, "Jhon Hernandez"), la interfaz de usuario delega el manejo del error a una alerta emergente nativa del navegador (window.alert) que muestra el mensaje genérico "Error al eliminar el cliente". Este tipo de alertas bloquean toda la interacción del navegador, tienen un aspecto visual ajeno a la línea gráfica de la aplicación y carecen de un formato amigable que sugiera al usuario cómo solucionar el problema o por qué ocurrió.

<img width="886" height="440" alt="Image" src="https://github.com/user-attachments/assets/b2d85c36-5142-4c27-89bf-a93b76aa43f2" />

Recomendación: Reemplazar el cuadro de alerta nativo por un componente de notificación del sistema integrado dentro de la aplicación (toast banner o una alerta modal estilizada con los colores del sistema de diseño). El mensaje debe ser descriptivo e indicar una razón clara (ej. "No se pudo eliminar el cliente porque tiene vehículos o servicios activos asociados").

**PROBLEMA \#17: Sobreposición de los inputs para ingresar nuevo artículo**

Severidad: 2

Heurística violada: Diseño estético y minimalista

Problema: Al tratar de crear un nuevo artículo, el apartado de texto para la marca está sobrepuesto en el de categoría, lo cual no resulta un problema que imposibilite al usuario ingresar los datos, sin embargo, a nivel de diseño y estético es necesario encargarse de ello.

<img width="713" height="969" alt="Image" src="https://github.com/user-attachments/assets/cbfa8155-e38e-4c54-9640-0fc1773bee09" />

Recomendación:

Manejar el diseño flexible y las media queries del formulario para que el ingreso de la información sea más óptimo.

**PROBLEMA \#18: Overflow en el formulario no controlado**

Severidad: 2

Heurística violada: Diseño estético y minimalista

Problema: El input para el stock mínimo está saliéndose de los límites del formulario, lo que está ocasionando a su vez un scroll innecesario que está sobreponiéndose al contenedor de imagen del material.

<img width="584" height="144" alt="Image" src="https://github.com/user-attachments/assets/7bd77a6e-4547-41e9-8f18-a2db2d1f2d2d" />

<img width="533" height="723" alt="Image" src="https://github.com/user-attachments/assets/21848e28-2d74-4c40-bb4d-45de5c732da5" />

<img width="563" height="202" alt="Image" src="https://github.com/user-attachments/assets/7033fa9b-9bb2-4e58-9c08-2a7ecdf7402c" />

Recomendación:

Controlar el espacio dirigido para cada apartado del formulario y mantener la flexibilidad con las media queries por posibles cambios de resolución en la pantalla.

**PROBLEMA \#19: Internacionalización a medias**

Severidad: 2

Heurística violada: Relación entre el sistema y el mundo real 

Problema: Aún existen zonas en las que la información no está recogiendo de forma correcta la traducción hacia los lenguajes de la página y solo está mostrando la dirección. Esto, para el usuario objetivo, podría resultar un problema de comprensión ya que no sabría qué es lo que la página está tratando de comunicar y es necesaria su revisión.

<img width="526" height="706" alt="Image" src="https://github.com/user-attachments/assets/f41baf42-eaba-4900-84b1-fd74ab448630" />

<img width="309" height="156" alt="Image" src="https://github.com/user-attachments/assets/81a15c2f-dc26-4d8c-919e-e49e7924a476" />

Recomendación:

Revisar minuciosamente la información con internacionalización y verificar que todos los textos se estén mostrando de forma exitosa en la página.

**PROBLEMA \#20: Interfaz duplicada y sin respetar espacios**

Severidad: 2

Heurística violada: Prevención de errores (Heurística \#5) / Flexibilidad y eficiencia de uso (Heurística \#7) 

Problema: En el campo "Cuenta de Mecánico", el usuario ya ingresó un correo electrónico completo (manolito.rojas@gmail.com), pero la interfaz duplica el dominio mostrando un texto fijo abajo (@gmail.com). Esto confunde al usuario sobre si debe ingresar el correo completo o solo el usuario, además de sugerir un formato rígido (nombre+apellido) que limita el uso de correos corporativos o de otros proveedores. Ademas, al terminar con el formulario las palabras salen del contenedor

<img width="552" height="869" alt="Image" src="https://github.com/user-attachments/assets/eed70cfc-5b0c-4215-adfd-6070b17e103d" />

<img width="642" height="552" alt="Image" src="https://github.com/user-attachments/assets/86a8750d-b25d-4d3a-8646-39de606b1a29" />

Recomendación: Eliminar la etiqueta estática `@gmail.com` externa al campo. Permitir que el usuario ingrese libremente cualquier dirección de correo electrónico válida y cambiar el texto de ayuda por algo más flexible, como: *"Ingrese el correo electrónico del mecánico"*. Agregar también algun acortador de frases cuando la cadena sea demasiado larga para que no sobrepase el espacio asignado.

**PROBLEMA \#20: Duplicidad en tabla**

Severidad: 1

Heurística violada: Consistencia y estándares (Heurística \#4) 

Problema: En la tabla de la sección "Tareas de la Orden", la cabecera presenta una columna duplicada. La etiqueta **"Materiales"** aparece dos veces (como tercera y quinta columna), lo que genera confusión visual y desorganización en la presentación de los datos. 

<img width="886" height="431" alt="Image" src="https://github.com/user-attachments/assets/829a1c23-51ee-4eeb-9e70-163aeb16f142" />

Recomendación: Revisar el componente de la tabla para eliminar la columna duplicada de **"Materiales"** o, en caso de que corresponda a un dato distinto, corregir el texto de la cabecera con el nombre correcto (por ejemplo: "Cantidad", "Acciones", etc.). 

**PROBLEMA \#21: Selector de filtrado por mecánico vacío y sin estado inicial claro** 

Severidad: 2

Heurística violada: Prevención de errores (Heurística \#5) / Visibilidad del estado del sistema (Heurística \#1) 

Problema: En la vista del "Tablero de tareas" (versión en español), al desplegar el filtro de "Mecánico", la lista desplegable muestra el mensaje *"No available options"* en inglés, a pesar de que el sistema está configurado en español. Además, el selector se muestra completamente en blanco sin un texto instructivo inicial (como "Seleccionar mecánico"), lo que genera incertidumbre sobre si existen mecánicos registrados en el sistema o si se trata de un fallo de carga de datos.

<img width="886" height="405" alt="Image" src="https://github.com/user-attachments/assets/f807c0eb-98b2-4377-ba18-a4a774f7f723" />

Recomendación: Implementar un estado por defecto legible para el selector (por ejemplo, "Todos los mecánicos" o "Seleccionar..."). Asimismo, asegurar que los mensajes de las listas vacías estén correctamente internacionalizados con vue-i18n para cambiar dinámicamente a "No hay opciones disponibles" cuando el idioma seleccionado sea el español. 

**PROBLEMA \#22: Falta de control de estados vacíos (Empty States) cuantitativos en el Panel Principal** 

Severidad: 1

Heurística violada: Reconocimiento antes que recuerdo (Heurística \#6) / Estética y diseño minimalista (Heurística \#8)

Problema: En el "Panel Principal del Taller", los contenedores destinados a mostrar los gráficos de "Ingresos semanales", "Actividad reciente" y "Servicios frecuentes" se renderizan completamente vacíos y desproporcionados cuando no hay datos registrados en el sistema. La gráfica muestra un eje numérico vertical flotando sin barras ni referencias temporales claras en el eje X, mientras que las secciones inferiores carecen de un mensaje aclaratorio o ilustración amigable, dejando cajas grises desoladas.

<img width="1949" height="894" alt="Image" src="https://github.com/user-attachments/assets/736dcbe0-9265-433b-96fc-eb1d58abb956" /> 

Recomendación: Implementar componentes de "Empty State" controlados. Cuando los arreglos de datos de las órdenes o ingresos estén vacíos, se debe ocultar el lienzo de la gráfica o la tabla vacía y, en su lugar, mostrar un texto sutil con un diseño limpio que indique al usuario algo como: *"No hay actividad registrada esta semana. Las métricas aparecerán cuando crees tu primera orden de trabajo"*.

### 5.4. Video About-the-Product
[Pendiente]


## Conclusiones

### Conclusiones y Recomendaciones

<p align="justify">
A continuación, se presentan las conclusiones derivadas del desarrollo de los primeros cinco capítulos del proyecto AutoService, así como las recomendaciones estratégicas para la continuidad de los siguientes Sprints:
</p>

<p align="justify"><b>Conclusiones:</b></p>
<ul style="text-align: justify; margin-top: 0.5em; margin-bottom: 1.5em; padding-left: 1.5em;">
  <li style="margin-bottom: 0.8em;">
    <strong>Implementación Integral de la Solución:</strong> Se logró desarrollar e integrar exitosamente una arquitectura compuesta por un frontend en Angular y un backend en Spring Boot, permitiendo la comunicación entre ambas capas mediante servicios REST y garantizando el funcionamiento integral de la plataforma.
  </li>
  <li style="margin-bottom: 0.8em;">
    <strong>Arquitectura Escalable y Mantenible:</strong> La aplicación de Domain-Driven Design (DDD) y la organización mediante Bounded Contexts permitió estructurar adecuadamente los dominios del negocio, favoreciendo la mantenibilidad, modularidad y escalabilidad del sistema.
  </li>
  <li style="margin-bottom: 0.8em;">
    <strong>Automatización y Despliegue Continuo:</strong> La integración de GitHub con las plataformas de despliegue permitió automatizar los procesos de construcción y publicación de la aplicación, facilitando la entrega continua y la disponibilidad del sistema.
  </li>
  <li style="margin-bottom: 0.8em;">
    <strong>Persistencia y Gestión de Datos:</strong> La implementación de una base de datos relacional mediante Spring Data JPA permitió garantizar la persistencia y gestión consistente de la información del sistema.
  </li>
  <li style="margin-bottom: 0.8em;">
    <strong>Madurez en la Gestión del Desarrollo:</strong> El uso de GitFlow, Pull Requests, Conventional Commits y documentación de APIs contribuyó a mantener un proceso de desarrollo colaborativo, organizado y alineado con buenas prácticas de ingeniería de software.
  </li>
</ul>

<p align="justify"><b>Recomendaciones:</b></p>
<ul style="text-align: justify; margin-top: 0.5em; margin-bottom: 1.5em; padding-left: 1.5em;">
  <li style="margin-bottom: 0.8em;">
    <strong>Fortalecimiento de la Seguridad:</strong> Implementar mecanismos avanzados de autenticación, autorización y gestión de roles para garantizar la protección de los recursos de la plataforma.
  </li>
  <li style="margin-bottom: 0.8em;">
    <strong>Incorporación de Pruebas Automatizadas:</strong> Ampliar la cobertura de pruebas unitarias, de integración y de aceptación para incrementar la confiabilidad del sistema.
  </li>
  <li style="margin-bottom: 0.8em;">
    <strong>Monitoreo y Observabilidad:</strong> Incorporar herramientas de monitoreo, registro de eventos y seguimiento de errores para mejorar la estabilidad operativa de la solución.
  </li>
  <li style="margin-bottom: 0.8em;">
    <strong>Evolución Funcional:</strong> Continuar incorporando funcionalidades y mejoras basadas en la retroalimentación de los usuarios y las necesidades del negocio.
  </li>
</ul>


---

## Bibliografía

<p align="justify" style="margin-left: 2em; text-indent: -2em; margin-bottom: 0.8em;">
  Angular Team. (2024). <i>Angular Documentation</i>. Google. <a href="https://angular.io/docs" target="_blank">https://angular.io/docs</a>
</p>

<p align="justify" style="margin-left: 2em; text-indent: -2em; margin-bottom: 0.8em;">
  Brandolini, A. (2021). <i>Introducing EventStorming: An act of deliberate collective learning</i>. Leanpub. <a href="https://leanpub.com/introducing_eventstorming" target="_blank">https://leanpub.com/introducing_eventstorming</a>
</p>

<p align="justify" style="margin-left: 2em; text-indent: -2em; margin-bottom: 0.8em;">
  Brown, S. (2020). <i>The C4 model for visualising software architecture</i>. C4 Model. <a href="https://c4model.com/" target="_blank">https://c4model.com/</a>
</p>

<p align="justify" style="margin-left: 2em; text-indent: -2em; margin-bottom: 0.8em;">
  Cucumber. (s.f.). <i>Gherkin Reference: Syntax and Keywords</i>. <a href="https://cucumber.io/docs/gherkin/" target="_blank">https://cucumber.io/docs/gherkin/</a>
</p>

<p align="justify" style="margin-left: 2em; text-indent: -2em; margin-bottom: 0.8em;">
  EmailJS. (2024). <i>EmailJS Official Documentation</i>. <a href="https://www.emailjs.com/docs/" target="_blank">https://www.emailjs.com/docs/</a>
</p>

<p align="justify" style="margin-left: 2em; text-indent: -2em; margin-bottom: 0.8em;">
  Evans, E. (2003). <i>Domain-Driven Design: Tackling Complexity in the Heart of Software</i>. Addison-Wesley Professional. <a href="https://www.oreilly.com/library/view/domain-driven-design-tackling/0321125215/" target="_blank">https://www.oreilly.com/library/view/domain-driven-design-tackling/0321125215/</a>
</p>

<p align="justify" style="margin-left: 2em; text-indent: -2em; margin-bottom: 0.8em;">
  GitHub. (2024). <i>GitHub Actions and GitHub Pages Documentation</i>. <a href="https://docs.github.com/" target="_blank">https://docs.github.com/</a>
</p>

<p align="justify" style="margin-left: 2em; text-indent: -2em; margin-bottom: 0.8em;">
  Gothelf, J., & Seiden, J. (2021). <i>Lean UX: Designing Great Products with Agile Teams</i> (3.ª ed.). O'Reilly Media. <a href="https://www.oreilly.com/library/view/lean-ux-3rd/9781492048596/" target="_blank">https://www.oreilly.com/library/view/lean-ux-3rd/9781492048596/</a>
</p>

<p align="justify" style="margin-left: 2em; text-indent: -2em; margin-bottom: 0.8em;">
  Spring Framework. (2024). <i>Spring Boot Reference Guide</i>. VMware. <a href="https://docs.spring.io/spring-boot/docs/current/reference/htmlsingle/" target="_blank">https://docs.spring.io/spring-boot/docs/current/reference/htmlsingle/</a>
</p>

<p align="justify" style="margin-left: 2em; text-indent: -2em; margin-bottom: 0.8em;">
  Swagger. (s.f.). <i>OpenAPI Specification and Documentation Tools</i>. <a href="https://swagger.io/" target="_blank">https://swagger.io/</a>
</p>

<p align="justify" style="margin-left: 2em; text-indent: -2em; margin-bottom: 0.8em;">
  Velneo. (2023). <i>Por qué usar un software de gestión ERP en talleres mecánicos</i>. <a href="https://velneo.com/blog/software-gestion-erp-talleres-mecanicos/" target="_blank">https://velneo.com/blog/software-gestion-erp-talleres-mecanicos/</a>
</p>

---

## Anexos

<div align="center">
  <h3 style="border-bottom: none;">Anexo A: Guía de Entrevistas por Segmento</h3>
</div>

<p align="justify">
A continuación, se presentan las guías de preguntas estructuradas utilizadas durante el proceso de <i>Requirements Elicitation</i> para los tres segmentos objetivo del proyecto. Estas preguntas fueron diseñadas para identificar puntos de dolor, procesos actuales y expectativas de los usuarios.
</p>

<p><strong>Segmento 1: Mecánicos Independientes</strong></p>
<table style="width: 100%; border-collapse: collapse; margin-bottom: 1.5em;">
  <thead>
    <tr style="background-color: #f2f2f2;">
      <th style="border: 1px solid #ddd; padding: 8px;">#</th>
      <th style="border: 1px solid #ddd; padding: 8px;">Pregunta de Entrevista</th>
    </tr>
  </thead>
  <tbody>
    <tr><td style="border: 1px solid #ddd; padding: 8px; text-align: center;">1</td><td style="border: 1px solid #ddd; padding: 8px;">¿Cuánto tiempo llevas trabajando como mecánico? ¿Podrías contarme cómo es un día típico en tu trabajo dentro del taller?</td></tr>
    <tr><td style="border: 1px solid #ddd; padding: 8px; text-align: center;">2</td><td style="border: 1px solid #ddd; padding: 8px;">¿Cómo registras actualmente la información de tus clientes, vehículos y trabajos?</td></tr>
    <tr><td style="border: 1px solid #ddd; padding: 8px; text-align: center;">3</td><td style="border: 1px solid #ddd; padding: 8px;">¿Cuáles son los principales problemas que enfrentas al gestionar los trabajos del taller?</td></tr>
    <tr><td style="border: 1px solid #ddd; padding: 8px; text-align: center;">4</td><td style="border: 1px solid #ddd; padding: 8px;">¿Cómo informas a tus clientes sobre el estado de sus vehículos?</td></tr>
    <tr><td style="border: 1px solid #ddd; padding: 8px; text-align: center;">5</td><td style="border: 1px solid #ddd; padding: 8px;">¿Qué tan seguido te llaman o escriben clientes para preguntar por el estado de su auto?</td></tr>
    <tr><td style="border: 1px solid #ddd; padding: 8px; text-align: center;">6</td><td style="border: 1px solid #ddd; padding: 8px;">¿Crees que tus clientes confían en el servicio que brindas? ¿Por qué?</td></tr>
    <tr><td style="border: 1px solid #ddd; padding: 8px; text-align: center;">7</td><td style="border: 1px solid #ddd; padding: 8px;">¿Llevas un historial de los trabajos realizados por vehículo o cliente?</td></tr>
    <tr><td style="border: 1px solid #ddd; padding: 8px; text-align: center;">8</td><td style="border: 1px solid #ddd; padding: 8px;">Si existiera una plataforma que te ayude a organizar tus trabajos y mostrar el progreso al cliente, ¿la usarías? ¿Por qué?</td></tr>
    <tr><td style="border: 1px solid #ddd; padding: 8px; text-align: center;">9</td><td style="border: 1px solid #ddd; padding: 8px;">¿Qué funcionalidad te sería más útil en una herramienta digital para tu trabajo diario?</td></tr>
  </tbody>
</table>

<p><strong>Segmento 2: Talleres Automotrices - Empresas</strong></p>
<table style="width: 100%; border-collapse: collapse; margin-bottom: 1.5em;">
  <thead>
    <tr style="background-color: #f2f2f2;">
      <th style="border: 1px solid #ddd; padding: 8px;">#</th>
      <th style="border: 1px solid #ddd; padding: 8px;">Pregunta de Entrevista</th>
    </tr>
  </thead>
  <tbody>
    <tr><td style="border: 1px solid #ddd; padding: 8px; text-align: center;">1</td><td style="border: 1px solid #ddd; padding: 8px;">¿Cuántas personas trabajan en su taller y cómo están organizadas sus funciones?</td></tr>
    <tr><td style="border: 1px solid #ddd; padding: 8px; text-align: center;">2</td><td style="border: 1px solid #ddd; padding: 8px;">¿Cómo gestionan actualmente los clientes, vehículos y órdenes de trabajo?</td></tr>
    <tr><td style="border: 1px solid #ddd; padding: 8px; text-align: center;">3</td><td style="border: 1px solid #ddd; padding: 8px;">¿Qué problemas tienen al coordinar el trabajo entre mecánicos o áreas?</td></tr>
    <tr><td style="border: 1px solid #ddd; padding: 8px; text-align: center;">4</td><td style="border: 1px solid #ddd; padding: 8px;">¿Cómo hacen seguimiento al estado de cada vehículo en reparación?</td></tr>
    <tr><td style="border: 1px solid #ddd; padding: 8px; text-align: center;">5</td><td style="border: 1px solid #ddd; padding: 8px;">¿Tienen algún sistema para medir ingresos, servicios realizados o rendimiento del taller?</td></tr>
    <tr><td style="border: 1px solid #ddd; padding: 8px; text-align: center;">6</td><td style="border: 1px solid #ddd; padding: 8px;">¿Cómo se comunican con los clientes sobre el avance del servicio?</td></tr>
    <tr><td style="border: 1px solid #ddd; padding: 8px; text-align: center;">7</td><td style="border: 1px solid #ddd; padding: 8px;">¿Han tenido problemas de desconfianza o reclamos por parte de clientes?</td></tr>
    <tr><td style="border: 1px solid #ddd; padding: 8px; text-align: center;">8</td><td style="border: 1px solid #ddd; padding: 8px;">Si existiera un sistema que te permita gestionar tu taller y mostrar a tus clientes el progreso en tiempo real, ¿lo usarías?</td></tr>
    <tr><td style="border: 1px solid #ddd; padding: 8px; text-align: center;">9</td><td style="border: 1px solid #ddd; padding: 8px;">¿Qué funcionalidades consideras indispensables en un sistema de gestión para talleres?</td></tr>
  </tbody>
</table>

<p><strong>Segmento 3: Clientes - Propietarios de vehículos</strong></p>
<table style="width: 100%; border-collapse: collapse; margin-bottom: 1.5em;">
  <thead>
    <tr style="background-color: #f2f2f2;">
      <th style="border: 1px solid #ddd; padding: 8px;">#</th>
      <th style="border: 1px solid #ddd; padding: 8px;">Pregunta de Entrevista</th>
    </tr>
  </thead>
  <tbody>
    <tr><td style="border: 1px solid #ddd; padding: 8px; text-align: center;">1</td><td style="border: 1px solid #ddd; padding: 8px;">¿Podrías contarme sobre la última vez que llevaste tu vehículo a un taller? ¿Qué servicio necesitabas?</td></tr>
    <tr><td style="border: 1px solid #ddd; padding: 8px; text-align: center;">2</td><td style="border: 1px solid #ddd; padding: 8px;">Durante el servicio, ¿cómo te informaban sobre el estado de tu vehículo?</td></tr>
    <tr><td style="border: 1px solid #ddd; padding: 8px; text-align: center;">3</td><td style="border: 1px solid #ddd; padding: 8px;">¿Tuviste alguna duda o preocupación mientras tu auto estaba en el taller? ¿Cuál fue?</td></tr>
    <tr><td style="border: 1px solid #ddd; padding: 8px; text-align: center;">4</td><td style="border: 1px solid #ddd; padding: 8px;">¿Alguna vez has sentido desconfianza hacia un taller? ¿Qué situación generó eso?</td></tr>
    <tr><td style="border: 1px solid #ddd; padding: 8px; text-align: center;">5</td><td style="border: 1px solid #ddd; padding: 8px;">¿Te gustaría poder ver el progreso de la reparación de tu auto en tiempo real desde tu celular o computadora? ¿Por qué?</td></tr>
    <tr><td style="border: 1px solid #ddd; padding: 8px; text-align: center;">6</td><td style="border: 1px solid #ddd; padding: 8px;">¿Qué tipo de información te gustaría ver mientras tu vehículo está en el taller?</td></tr>
    <tr><td style="border: 1px solid #ddd; padding: 8px; text-align: center;">7</td><td style="border: 1px solid #ddd; padding: 8px;">¿Qué tan cómodo te sientes usando plataformas digitales o aplicaciones para consultar información de servicios?</td></tr>
    <tr><td style="border: 1px solid #ddd; padding: 8px; text-align: center;">8</td><td style="border: 1px solid #ddd; padding: 8px;">Si existiera una plataforma que te permita ver el estado de tu vehículo, costos y trabajos realizados, ¿la usarías? ¿Qué te gustaría que incluya?</td></tr>
  </tbody>
</table>

<div align="center">
  <h3 style="border-bottom: none;">Anexo B: Gestión del Product Backlog en Jira Software</h3>
</div>

<p align="justify">
<b>Referencia:</b> InnovaTech Studio. (2026). <i>Product Backlog de AutoService</i>. Atlassian Jira Software. <a href="https://innovatechstudio.atlassian.net/jira/software/projects/ASS/boards/1" target="_blank">https://innovatechstudio.atlassian.net/jira/software/projects/ASS/boards/1</a>
</p>

<p align="justify">
Se presenta la gestión de historias de usuario, épicas y tareas técnicas mediante la herramienta Jira Software. El tablero refleja la priorización de los ítems del backlog y el estado de avance de las tareas planificadas para el Sprint 1.
</p>

<div align="center">
  <img src="docs/assets/anexos_jira.png" alt="Jira Product Backlog Screenshot" width="80%">
</div>

<br>

<div align="center">
  <h3 style="border-bottom: none;">Anexo C: Prototipado y Diseño de Interfaces en Figma</h3>
</div>

<p align="justify">
<b>Referencia:</b> InnovaTech Studio. (2026). <i>Design System y Mockups de AutoService</i>. Figma. <a href="https://www.figma.com/design/rOJ6k8HLfI85lI8Xsik6TN/AUTOSERVICE-AW?node-id=1-2&t=aYBkJzt0CQrAU6qH-1" target="_blank">https://www.figma.com/design/rOJ6k8HLfI85lI8Xsik6TN/AUTOSERVICE-AW</a>
</p>

<p align="justify">
Se adjunta el diseño de alta fidelidad de la plataforma, incluyendo el Design System (colores, tipografías y componentes), los wireframes y los mockups interactivos que definen la experiencia de usuario (UX) y la interfaz (UI) de AutoService.
</p>

<div align="center">
  <h5>Captura del Diseño de Interfaces - Figma</h5>
  <img src="docs/assets/anexos_figma.png" alt="Figma UI/UX Design Screenshot" width="80%">
</div>

<br>

<div align="center">
  <h3 style="border-bottom: none;">Anexo D: Modelado de Dominio y Flujos en Miro</h3>
</div>

<p align="justify">
<b>Referencia:</b> InnovaTech Studio. (2026). <i>EventStorming y User Flows de AutoService</i>. Miro. <a href="https://miro.com/welcomeonboard/ME8rSzFiTWh0M3k1SC80N0RZelVpKzBCdk5LNTZsTzhDSEJORE4ybE5ta25rUVd1ZFVNZndDS1ExZm0xSkdNVHFuc3E3QTN1QzQrcFFzYnUrYzN1NE5HTFdLQ1ZtbnNpYUN3cWJiblZ5dVdCQS9rY3dnSjlBdnNPSDh4Tk41alBnbHpza3F6REdEcmNpNEFOMmJXWXBBPT0hdjE=?share_link_id=615806054520" target="_blank">Enlace al tablero interactivo en Miro</a>
</p>

<p align="justify">
Se presenta el modelado colaborativo del dominio del negocio mediante la técnica de EventStorming, así como los diagramas de flujo de usuario (User Flows) que detallan la navegación lógica para los distintos actores del sistema.
</p>

<div align="center">
  <h5>Captura del Tablero de Modelado - Miro</h5>
  <img src="docs/assets/anexos_miro.png" alt="Miro EventStorming Screenshot" width="80%">
</div>

### 5.4. Video About-the-Product
[Pendiente]
-->
