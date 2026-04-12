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