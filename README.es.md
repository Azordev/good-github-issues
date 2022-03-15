# Issues

- [Issues](#issues)
  - [¿Qué es un issue?](#qué-es-un-issue)
  - [Qué debe contener un issue?](#qué-debe-contener-un-issue)
    - [Descripción:](#descripción)
    - [Capturas de pantalla:](#capturas-de-pantalla)
    - [Lista de tareas:](#lista-de-tareas)
    - [Referencias:](#referencias)
  - [¿Qué se debe considerar cuando se escribe un issue?](#qué-se-debe-considerar-cuando-se-escribe-un-issue)
    - [Un issue a la vez](#un-issue-a-la-vez)
    - [Títulos son importantes](#títulos-son-importantes)
    - [Si aplica, no olvides añadir:](#si-aplica-no-olvides-añadir)
- [Bibliografía:](#bibliografía)

[Azordev](https://github.com/Azordev/) gestiona casi todo su trabajo a través de GitHub. Por eso es importante que sean issues detalladas y bien creadas. A continuación se muestran algunas de las mejores prácticas para escribir issues de GitHub de forma apropiada.

Buenos issues le brindarán más ayuda al facilitar que los colaboradores externos extiendan su proyecto y lo ayuden.

## ¿Qué es un issue?

Cuando hablamos de issues estamos hablando de problemas, estos problemas pueden presentarse de varias maneras, incluyendo discusiones respecto a qué tecnología usar en un proyecto o como organizar su estructura.

Un issue representa una tarea de un proyecto o un problema que necesita una solución para avanzar con dicho proyecto, y puede ir destinado a un desarrollador, diseñador, copywriter, o a cualquiera que esté dentro o fuera del proyecto y tenga la capacidad para solucionarla.

Siempre las tareas deben estar lo suficientemente bien explicadas para que alguien que no pertenezca al proyecto pueda tomarla y colaborar sin problemas.

Para esto puede seguir la siguiente guía, la cual estará dividida en dos partes, una respecto al contenido que debe llevar un issue y otra que habla sobre cosas a considerar para crear un buen issue.

## Qué debe contener un issue?

### Descripción: 

Lo primero que debes agregar a tu issue es una descripción clara sobre el problema, preferiblemente visto desde el punto de vista de un usuario, lo que llaman [Historias de usuario](https://es.wikipedia.org/wiki/Historias_de_usuario).

Por lo general nosotros seguimos la siguiente estructura para la descripción de los issues:

- Contexto: explica las condiciones por las cuales tú escribes el issue. — “Desde que nos movimos a la última versión de Express.js, hemos experimentado algunos problemas de rendimiento (#14 and #15) en producción.”
- Problema o idea: el contexto debe conducir a algo, una idea o un problema al que estés enfrentando. — “No hemos tenido manera de ver facilmente el impacto de rendimiento antes de lanzar nuestros cambios a producción.”
- Solution or next step: en caso de tener alguna idea de cómo se podría avanzar con el problema puede añadir una solución, sino, puede añadir un siguiente paso. — “Buscar qué herramientas son buenas para medir el rendimiento de un servidor en NodeJs”

### Capturas de pantalla:

Siempre que aplique, debe añadir fotos de lo que se refiere el issue para dar mayor contexto a los desarrolladores y todos puedan entender mejor el problema del que se habla.

### Lista de tareas:

Posiblemente la parte más importante, dado que es realmente en estos puntos en los que se fija el desarrollador a la hora de resolver el problema.

Puedes tomar la checklist como la lista de parámetros mínimos que deben cumplirse para que se considere solucionado un problema.

### Referencias:

Dado que las issues deben permanecer cortas, las referencias serán un punto de apoyo donde los desarrolladores pueden ir a buscar más información aparte de la suministrada en el issue.

Si es un issue complejo, puedes agregar documentación o cualquier cosa que pueda ayudar al desarrollador a dar el siguiente paso.

Un ejemplo de uso es cuando se pide añadir estilos a una página web y nos basamos en un diseño, ya sea en figma o adobe xd o si está en un PDF, podemos agregar el enlace a este diseño, aparte de los screenshots en su respectiva sección.

## ¿Qué se debe considerar cuando se escribe un issue?

### Un issue a la vez

Es bastante importante evitar issues que describan demasiado. Cada error o petición de funcionalidad deben ser documentadas en su propio issue.

- Mal — “El formulario necesita un campo de `subject`. También, el botón de enviar no funciona.” (Sepáralo en dos issues.)
- Bien — “Añadir un campo de `subject` al formulario”
- Good — “El botón de enviar causa error 405”

A menudo es inevitable que los issues se vuelvan complejos, especialmente con peticiones de grandes funcionalidades. ¡Añadir un montón de detalle a un issue es genial!, pero cuando un issue complejo puede ser separado en múltiples issues, eso los hace más fácil de resolver.

### Títulos son importantes

Mantén tus títulos cortos y descriptivos. No intentes añadir un montón de información en el título.

Por ejemplo, en vez de escribir el título “El campo de búsqueda causa error cuando escribes más de 50 carácteres y presionas `enter`.”, el detalle específico — como el error que pasa cuando presionas `enter` — puede ser explicado en el cuerpo del issue.

### Si aplica, no olvides añadir:

- **Enlaces** — Incluye todos los enlaces a la vista específica de la aplicación que estás describiendo.
- **Capturas de pantalla** — Una imagen dice más de 1.000 palabras (un gif dice 1.000.000). Una captura de pantalla puede ayudar a aclarar el problema que mencionas en el issue.
- **@ yo** — Si tú sabes con certeza qué personas deben ser notificadas, asegúrate de mencionarlas en el issue.
- **Etiquetas** — Usa las etiquetas para clasificar tus issues, también tú puedes usarlas para crear una manera fácil de filtrarlos. Nosotros utilizamos normalmente tres tipos de etiquetas: 

  1. **Estimación de esfuerzo:** Menciona cuánto esfuerzo requiere la tarea para ser completada. Puedes seguir [this guide](https://docs.google.com/document/d/1ZaiuNGsNSQvZgB6Gr20imG9VFEB5YPNDfD5PaDoYPPg/edit?usp=sharing) para tener una idea de cómo funcionan las etiquetas de esfuerzo en Azordev.
  2. **Tipo de tareas:** Como se mencionó en [¿Qué es un issue?](#qué-es-un-issue), pueden existir distintos tipos de tareas. Tareas para diseñadores, por ejemplo, pueden llevar la label `design`, mientras que tareas para desarrolladores pueden dividirse por tecnologías, por ejemplo `javascript`, `css`, o pueden dividirse por tipo de tarea, por ejemplo: `api`, `logic`, `style`.
  3. **Prioridad:** Este label estipula qué tan pronto se requiere que se solucione algún issue, pueden ser tres o más: `low`, `mid`, `high`

# Bibliografía:

- [Writing a proper issue](https://medium.com/nyc-planning-digital/writing-a-proper-github-issue-97427d62a20f)
- [How we write our github issues](https://wiredcraft.com/blog/how-we-write-our-github-issues/)
- [Effort Estimation guide](https://docs.google.com/document/d/1ZaiuNGsNSQvZgB6Gr20imG9VFEB5YPNDfD5PaDoYPPg/edit?usp=sharing)