
<p align="center">
    <img src="http://foro.comunidadargentum.com/images/dragonbyte_mmogaming/misc/vbulletin4_logo.png" />
</p>
<h1 align="center">
    <span>Guía de contribución a Argentum Online </span>
</h1>

  
:+1::tada: Antes que nada, ¡gracias por tomarte el tiempo y contribuir con Argentum Online! :tada::+1:

Lo que sigue a continuación es una serie de lineamientos para contribuir a cualquiera de los proyectos que se encuentran hospedados en la [Organización de Argentum Online](https://github.com/argentumonline) en GitHub. Estos son lineamientos, no reglas. Por favor, usá tu mejor juicio, y sentite libre de proponer cambios a este documentos creando un Pull Request.

#### Tabla de Contenidos
- [Código de Conducta](#código-de-conducta)
- [Canales de comunicación disponibles](#canales-de-comunicación-disponibles)
- [¿Qué debo saber antes de comenzar?](#qué-debo-saber-antes-de-comenzar)
  - [Decisiones de diseño en Argentum Online](#decisiones-de-diseño-en-argentum-online)
  - [Decisiones sobre mecánicas de juego en Argentum Online](#decisiones-sobre-mecánicas-de-juego-en-argentum-online)
- [¿Cómo puedo contribuir?](#cómo-puedo-contribuir)
  - [Reportando bugs](#reportando-bugs)
  - [Proponiendo mejoras](#proponiendo-mejoras)
  - [Contribuyendo al código fuente](#contribuyendo-al-código-fuente)
    - [Desarrollo local](#desarrollo-local)
  - [Pull Requests](#pull-requests)
- [Guias de estilo](#guias-de-estilo)
  - [Nombres de Branches](#nombres-de-branches)
  - [Mensajes de Commit](#mensajes-de-commit)
  - [Guía de estilos para cada lenguaje](#guía-de-estilos-para-cada-lenguaje)
  - [Etiquetas (Labels)](#etiquetas-labels)
    - [Labels para tipos de Issues](#labels-para-tipos-de-issues)
    - [Etiquetas de Categoría](#etiquetas-de-categoría)
    - [Pull Request Labels](#pull-request-labels)

## Código de Conducta

Este proyecto y todos los participantes están gobernados por el [Código de Conducta de Argentum Online](.github/CODE_OF_CONDUCT.md). Participando en el desarrollo, se espera que te adhieras a este código. Por favor, reporta cualquier comportamiento inaceptable enviando un correo a [direccion@comunidadargentum.com](mailto:codeofconduct@comunidadargentum.com).

## Canales de comunicación disponibles

> **Nota:** Por favor, no crees un Issue para hacer una pregunta sin antes haber pasado por uno de estos canales.

El proyecto Argentum Online mantiene varios medios de comunicación con todos los miembros de su comunidad (ya sean desarrolladores, diseñadores, o jugadores).

* [Foro Oficial de Argentum Online](http://foro.comunidadargentum.com)
* [ Discord de Argentum Online](https://discord.gg/argentumonline) es un servicio de Chat destinado a toda la comunidad del juego, incluyendo a los jugadores del Servidor Oficial de Argentum Online. Si te interesa participar de discusiones sobre desarrollo, te recomendamos participar de los siguientes canales:
    * Usa el canal `#🧙🏽programacion` para discusiones acerca del código del juego y sus herramientas
    * Usa el canal `#🌏mapeo` para discusiones acerca de los mapas del juego y las herramientas para construirlos
    * Usa el canal `#🎨graficacion` para discusiones acerca de los gráficos del juego
    * Usa el canal `#💡ideas ` para proponer nuevas ideas y mecánicas para el juego
    * Hay muchos otros canales para que puedas interactuar con la comunidad. 

## ¿Qué debo saber antes de comenzar?

### Decisiones de diseño en Argentum Online

Argentum Online es un juego MMORPG Open Source, lo que significa que su código es abierto para que cualquier usuario lo descargue y cree sus propios forks, pero esto no significa que las mecánicas a implementar sean decididas por la comunidad abiertamente.
El Staff del proyecto es el único equipo autorizado a tomar decisiones y aprobar cambios sobre la arquitectura del juego. Cualquier recomendación y contribución es bienvenida, y nos comprometemos a trabajar con los usuarios que contribuyan para adaptar cualquier propuesta a los requerimientos del juego.

### Decisiones sobre mecánicas de juego en Argentum Online
Debido a que Argentum Online es un juego, las decisiones sobre las mecánicas nuevas deben pasar por los equipos de Game Design y Balance, que son los que se encargan de asegurarse que cualquier propuesta encaje junto al resto de las mecánicas y que no generen un desbalance en el juego.
Si deseas proponer una nueva mecánica o cambio a una mecánica existente, te recomendamos que antes de contribuir el código crees un Issue en Github siguiendo los lineamientos para solicitudes de features, y luego utilices [los canales de comunicaciones disponibles](#canales-de-comunicación-disponibles) para discutirlo con dichos equipos.


## ¿Cómo puedo contribuir?

### Reportando bugs
Antes de crear un reporte de bug, por favor revisa que el mismo no haya sido reportado con anterioridad o esté pendiente de implementación. Cuando crees un reporte, por favor escribe la mayor cantidad de detalles completando el [template obligatorio propuesto](https://github.com/argentumonline/.github/blob/master/.github/ISSUE_TEMPLATE/bug_report.md)
La información requerida en ese template nos va a ayudar a validar el bug lo más rápido posible

> **Nota:** Si encuentras un Bug reportado con estado **Closed** que parezca ser el mismo bug que estás experimentando, por favor crea un nuevo issue y asegurate de poner una referencia al issue anterior.

### Proponiendo mejoras
Existen diferentes tipos de mejoras que se pueden proponer, que pueden incluir desde cambios menores a funcionalidad existente, o nuevas funcionalidades.
Antes de crear un issue para proponer una mejora, por favor revisa si la misma no fue propuesta por otra persona.
Cuando crees un issue con una propuesta, por favor escribe la mayor cantidad de detalles completando el [template obligatorio](https://github.com/argentumonline/.github/blob/master/.github/ISSUE_TEMPLATE/feature_request.md)
La información requerida en ese template nos va a ayudar a evaluar la propuesta lo más rápido posible.

### Contribuyendo al código fuente
Argentum Online está compuesto por varios proyectos (cliente, servidor, herramientas, etc). ¿No estás seguro por dónde empezar? Podrías comenzar por revisar los issues que contengan las etiquetas `beginner` y `help-wanted`.

* `beginner` - Issues que solo deberían requerir cambios en algunas líneas de código.
* `help-wanted` - Issues para los que se requiere un poco más de conocimientos sobre la plataforma.

#### Desarrollo local

Todos los componentes del juego pueden ser desarrollados y testeados localmente. Para los casos en donde herramientas de terceros sean necesarias (base de datos, gestor de colas, etc), los pasos de instalación y configuración estarán explicados en cada uno de los repositorios.
Adicionalmente, haremos un esfuerzo para proveer archivos `docker-compose` siempre que podamos para facilitar el desarrollo local

### Pull Requests

Los procesos descriptos a continuación tienen como propósito:

- Mantener una calidad de código aceptable para la contribución de código
- Involucrar a la comunidad en el trabajo de mejorar Argentum Online a diario
- Habilita la posibilidad de que los encargados de revisar el código tengan un espacio para hacerlo.

Por favor, sigue estos pasos para que tu contribución sea considerada por los mantenedores del código:

1. Sigue las instrucciones para [abrir pull requests](PULL_REQUEST_TEMPLATE.md)
2. Sigue las [Guias de estilo](#Guias-de-estilo)
3. Después de crear tu pull request, verifica que todos los [status checks](https://help.github.com/articles/about-status-checks/) estén pasando correctamente

> NOTA: ¿Qué pasa si un status check está fallando? Si un status check falla, y consideras que la falla no está relacionada con tu cambio, por favor deja un comentario en el Pull Request explicando por qué consideras que no está relacionado. Un responsable del mantenimiento revisará y evaluará la situación, trabajando contigo para que se los checks se resuelvan.  

Mientras que los requisitos arriba mencionados tienen que ser cumplidos antes de que tu código sea revisado, los reviewers pueden pedirte que hagas cambios adicionales al diseño, pruebas o cualquier otra cosa que se considere necesario antes de que el PR sea aceptado.

## Guias de estilo

### Nombres de Branches
Para asegurarnos de que la automatización ejecutada sobre cada repositorio siga un patrón determinado, considera la siguiente convención de nombres para los branches:
* Usa `feature/nombreDescriptivo` si el branch contiene un refactor o nueva funcionalidad o mecánica que no esté relacionado a un arreglo de un bug
* Usa `fix/numeroIssue-nombreDescriptivo` si el branch contiene un arreglo a un bug reportado. Si estás creando un bugfix para un issue que no se encuentra reportado, por favor considera reportarlo primero para poder referenciarlo.

### Mensajes de Commit

* Limitar la primer línea a 72 caracteres o menos.
* Poner referencias a Issues o Pull Requests solo después de la primer línea
* Ser lo más descriptivo posible a la hora explicar el/los cambios introducidos.

### Guía de estilos para cada lenguaje
Para cada uno de los lenguajes usados en el proyecto, contamos con una guía de estilos.
* Para VB6
* Para C#
* Para PHP
* Para C++


### Etiquetas (Labels)

Esta sección explica las etiquetas (labels) que usamos para ayudarnos a administrar y conocer el etado de las tareas. Muchas de estas etiquetas se usan en todos los repositorios, aunque otras son específicas para algunos de ellos.

[La búsqueda de GitHub](https://help.github.com/articles/searching-issues/) facilita la tarea de usar etiquetas (labels) para encontrar grupos de Issues o Pull Requests en los que puedes estar interesado. Te recomendamos que leas el artículo para saber más sobre consultas específicas.

Si tenes una sugerencia para agregar alguna etiqueta nueva, por favor abre un Pull Request en el repositorio correspondiente y nuestro equipo de mantenedores se encargará de evaluarla e implementarla.

#### Labels para tipos de Issues
| Label name                |                                                                                                                                                                                                           |
|---------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| `enhancement`             | Solicitud de cambio a una funcionalidad                                                                                                                                                                   |
| `bug`                     | Bugs confirmados o reportes que parecen serlo.                                                                                                                                                            |
| `question`                | Pregunta sobre cómo realizar algo en particular. Por favor referirse a .                                                                                                                                  |
| `feedback`                | Feedback sobre algun cambio en una mecánica o proceso.                                                                                                                                                    |
| `help-wanted`             | El equipo de Argentum Online apreciaría mucho la ayuda en la resolución de uno de estos Issues                                                                                                            |
| `beginner`                | Issues que no son complejos re resolver, y perfectos para cualquiera que quiera comenzar a contribuir en Argentum Online.                                                                                 |
| `more-information-needed` | Se requiere más información para poder resolver este Issue (Ej. pasos para reproducirlo).                                                                                                                 |
| `blocked`                 | Issues que se encuentra bloqueado por otro Issue que aun no fue resuelto.                                                                                                                                 |
| `duplicate`               | Issues que es un duplicado de otro Issue ya reportado. Se requiere confirmación.                                                                                                                          |
| `wontfix`                 | El equipo de Argentum Online no va a resolver este Issue por alguna razon. Las razones normalmente se dejarán por escrito en como comentario en el Issue.                                                 |
| `wrong-repo`              | Issue reportado en el repositorio equivocado (Ej. un bug reportado en [Cliente](https://github.com/argentumonline/client-vb6) fue reportado en [Servidor](https://github.com/argentumonline/server-vb6)). |


#### Etiquetas de Categoría

| Label name      | Description                                                                                   |
|-----------------|-----------------------------------------------------------------------------------------------|
| `windows`       | Relacionado a un proyecto corriendo en Windows.                                                 |
| `linux`         | Relacionado a un proyecto corriendo en Linux.                                                   |
| `mac`           | Relacionado a un proyecto corriendo en macOS.                                                   |
| `documentation` | Relacionado a cualquier tipo de documentación.                                                |
| `performance`   | Relacionado a temas de rendimiento.                                                           |
| `security`      | Relacionado a la seguridad.                                                                   |
| `ui`            | Relacionado a temas de interfaz gráfica.                                                      |
| `crash`         | Relacionado a cualquiera de los proyectos que dejen de funcionar de forma repentina           |
| `auto-indent`   | Relacionado a temas de auto indentación                                                       |
| `encoding`      | Related a temas de encoding de caracteres                                                     |
| `network`       | Related to network problems or working with remote files (e.g. on network drives).            |
| `git`           | Relacionado a temas de funcionalidad de Git (Ej: problemsa con archivos .gitignore problems). |

#### Pull Request Labels

| Label name         | Description                                                                  |
|--------------------|------------------------------------------------------------------------------|
| `work-in-progress` | Pull request que está siendo trabajado y no está listo para ser revisado.    |
| `needs-review`     | Pull request ya finalizado y pendiente de revisión.                          |
| `under-review`     | Pull request que está siendo revisado.                                       |
| `requires-changes` | Pull request que necesita cambios después de haber sido revisado.            |
| `needs-testing`    | Pull request que requiere pruebas manuales para verificar su funcionamiento. |

#

>NOTA: Este documento fue creado en base a la guía de contribución del [proyecto Atom](https://github.com/atom/atom/blob/master/CONTRIBUTING.md)