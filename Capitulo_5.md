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

<!--  PENDIENTE PARA ENTREGA FINAL TB2
### 5.3. Validation Interviews

#### 5.3.1. Diseño de Entrevistas
[Pendiente]

#### 5.3.2. Registro de Entrevistas
[Pendiente]

#### 5.3.3. Evaluaciones según heurísticas
[Pendiente]

### 5.4. Video About-the-Product
[Pendiente]
-->