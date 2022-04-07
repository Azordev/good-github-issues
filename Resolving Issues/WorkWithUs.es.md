# Cómo trabajar con Azordev creando tareas

- [Cómo trabajar con Azordev creando tareas](#cómo-trabajar-con-azordev-creando-tareas)
  - [Como encontrar las tareas](#como-encontrar-las-tareas)
  - [Como solicitar que me asignen a una tarea](#como-solicitar-que-me-asignen-a-una-tarea)
  - [Como empezar a solucionar la tarea a la que fui asignado](#como-empezar-a-solucionar-la-tarea-a-la-que-fui-asignado)
    - [¿Qué debo hacer si aún no tengo permisos en el repositorio?](#qué-debo-hacer-si-aún-no-tengo-permisos-en-el-repositorio)
    - [¿Qué debo hacer si ya tengo permisos en el repositorio?](#qué-debo-hacer-si-ya-tengo-permisos-en-el-repositorio)
  - [¿Qué debo hacer luego de crear el Pull Request?](#qué-debo-hacer-luego-de-crear-el-pull-request)
  - [¿Cuándo me pagan?](#cuándo-me-pagan)
  - [Condiciones](#condiciones)
  - [Negociación](#negociación)
  - [FAQ](#faq)
    - [¿Qué es el Code Review?](#qué-es-el-code-review)

Si te interesa empezar a trabajar como freelancer para Azordev resolviendo tareas, puedes seguir esta guía sobre el flujo de trabajo que existe en Azordev:

## Como encontrar las tareas

1. Ve a GitHub y entra en la [organización de Azordev](https://github.com/Azordev/).
2. Allí verás unos repositorios fijados, esos son los repositorios que se están trabajando actualmente. Siéntete libre de navegar por ellos, revisarlos, estudiarlos y busca el que más te llame la atención o más se adapte a tus conocimientos.
3. Una vez hayas escogido algún repositorio, puedes dirigirte a la sección de `issues` para ver las tareas que estén disponibles.

## Como solicitar que me asignen a una tarea

1. Notarás que hay algunas tareas que no tienen a nadie asignado, esas tareas están libres de ser tomadas, siempre y cuando no tengan ninguna label `Blocked` or `Need design`.
2. Una vez hayas encontrado alguna issue que te llame la atención, entra en el issue y comenta que te gustaría ser asignado, por ejemplo: "Me gustaría ayudar a resolver esta issue", un encargado te leerá y te asignará la issue.

## Como empezar a solucionar la tarea a la que fui asignado

Una vez hayas realizado el paso anterior sobre [como solicitar que te asignen a una tarea](#como-solicitar-que-me-asignen-a-alguna-tarea), puedes empezar a solucionarla.

Esto depende de si [ya tienes permisos en el repositorio](#ya-tienes-permiso-en-el-repositorio), o [si aún no se te han dado permisos](#aún-no-tienes-permisos-en-el-repositorio). Explicaré los dos casos a continuación

### ¿Qué debo hacer si aún no tengo permisos en el repositorio?

Si aún no tienes permisos en el repositorio, puedes solicitar permisos escribiéndonos a [contacto@azordev.com](mail:contacto@azordev.com) o comentando en el issue que te den permisos.

Si por alguna razón no te hemos dado permiso todavía, y quieres comenzar a trabajar sin esperar, puedes crear un Fork de nuestro repositorio y trabajar desde allí. Puedes seguir esta documentación de GitHub acerca de [como crear un fork](https://docs.github.com/es/get-started/quickstart/fork-a-repo), allí explican qué son, cómo se crean, para qué sirven y cómo puedes colaborar usandolas.

Una vez tengas permisos o hayas creado un fork, puedes continuar con la [siguiente sección](#qué-debo-hacer-si-ya-tengo-permisos-en-el-repositorio)

### ¿Qué debo hacer si ya tengo permisos en el repositorio?

Si ya tienes permisos en el repositorio o has creado un fork, puedes seguir los siguientes pasos:

1. Una vez ya estés asignado, puedes ir al README.md de ese repositorio para ver cómo puedes clonarlo y correrlo.
2. Cuando ya tengas el repositorio clonado en tu PC, lo primero que debes hacer es crear una rama para ese issue, nosotros usamos la siguiente nomenclatura para el nombre de las ramas: `fix|feat/#{issuenumber}`, si el issue trata sobre añadir una nueva funcionalidad se utiliza "feat" al inicio, pero si trata sobre arreglar algún bug, se utiliza "fix". El resultado sería por ejemplo: `fix/#5` o `feat/#1`.
3. Ya con la rama creada, puedes empezar a trabajar en tu issue, una vez tengas los cambios listos, haces el push hacia esa rama: `git add .` -> `git commit -m "{descripción corta de tus cambios}"` -> `git push origin {nombre de tu rama}`. El resultado sería algo así, por ejemplo: `git commit -m "added background color in home view"` -> `git push origin fix/#5`.
4.  Una vez hayas realizado el push, github te invitará a hacer un Pull Request, haces el pull request apuntando hacia la rama principal de nuestro repositorio, le agregas un título y descripción agradable que nos ayude a entender el cambio que has realizado y esperas por el Code Review.

## ¿Qué debo hacer luego de crear el Pull Request?

Una vez hayas terminado tus cambios y hayas creado el Pull Request, los encargados de Azordev entrarán a revisar tus cambios, a este proceso se le conoce como [Code Review](#code-review).

Durante esa revisión se te pueden dejar comentarios de cambios necesarios, así como sugerencias. Las sugerencias no son obligatorias pero generalmente son acerca de lo que se considera buena práctica o no, si se aplica o no, no es mucha la diferencia, pero si te interesa aprender de buenas prácticas y mejorar tu código puedes aprovechar esos comentarios para aprender lo que no te enseñan en los cursos.

Por otro lado, los comentarios acerca de cambios necesarios serán acerca de cosas que no funcionen o que no se vean nada bien en el código y necesiten una mejora. Estos cambios serán necesario aplicarlos ya que afectan el trabajo de los demás developers del equipo, y son cambios que no pueden llevarse con errores a la rama principal.

Por lo normal, luego de hacer el pull request, el flujo es el siguiente:

1. Varios encargados de Azordev revisan tu código, pueden aprobarlo, comentar o requerir cambios.
2. Si hay comentarios, lo correcto sería contestarlo, la mayoría de las veces los comentarios serán dudas acerca de tus cambios. Si hay cambios requeridos, lo correcto sería: 
    1. ¿Estás de acuerdo con el cambio?: Realiza un nuevo commit con el cambio y haz el push para que se suba a la rama.
    2. ¿Crees que no es necesario o no tiene que ver con la tarea que resuelves?: Háblalo con el equipo para que movamos el comentario hacia una nueva tarea.
    3. ¿Crees que realmente hay una mejor manera de hacerlo?: Háblalo con el equipo para ver la mejor manera de hacer las cosas y así aprendemos y mejoramos todos.
3. Una vez los comentarios hayan sido completados, si no salen más comentarios, entonces el pull request se fusionará con la rama principal, se cerrará el issue al que fuiste asignado, y se te anotarán los puntos de esfuerzo de ese issue para el pago.

## ¿Cuándo me pagan?

Una vez cerrado el issue que estabas asignado, serás anotado en la nómina para pagarte al final del mes. Normalmente entre el 28 del mes y el 5 del mes siguiente. Para más información de los pagos revise la sección de pagos
<!-- TODO: Añadir sección de pagos donde explique los métodos de pago y etc -->

## Condiciones

A pesar de ser un puesto de freelancer y que no tengas ninguna obligación dentro de la empresa, siempre recuerda que la responsabilidad, la honestidad y el compañerismo son cualidades de un desarrollador profesional, y serán valoradas por la empresa. Por otro lado, para mantener el orden y el respeto dentro de la empresa, no detener el flujo de trabajo ni afectar a los demás con nuestro trabajo, existen las siguientes condiciones:

1. Para ser asignado a un issue siempre debes comentar el issue y pedir que se te asigne. Algún encargado asignará al primero que pida el issue siempre que no haya un motivo para no hacerlo.
2. Cada persona puede estar asignado a un máximo de 2 issues, así que primero concéntrate en los issues que ya tienes, para poder pedir algún otro que te guste.
3. Si una persona lleva más de 4 días asignado a un issue sin subir ningún Pull Request o interactuar, se le escribirá para ver el estado de la tarea, en caso de que el desarrollador no pueda hacerla por cualquier motivo, será desasignado para que otro tome la tarea. En caso de que el desarrollador sí pueda y quiera hacerla o ya tenga algo avanzado, se le darán unos días más para que termine el pull request.
4. Nunca debes hacer el push hacia la rama principal, siempre debes crear una rama individual desde la que trabajes los cambios requeridos para completar tu issue.
5. Si se nota algún comportamiento malicioso, como abusar de los permisos de escritor en el repositorio para desasignar a otros de sus tareas, cerrar issues que no estén completos, o intentar dañar pull requests de otros, etc... Será betado completamente de Azordev y no podrá trabajar con nosotros como Freelancer ni como Developer.
6. Tratamos de que sea un área amigable y donde todos se sientan seguros, por lo que el respeto será muy importante dentro de la comunicación en Azordev. 

## Negociación

Estamos completamente abiertos a opiniones y comentarios acerca de las tareas y cómo mejorarlas. Un caso que puede darse, por ejemplo, es que una issue sea demasiado grande o la estimación de esfuerzo sea demasiado baja. En esos casos el desarrollador puede sugerir dividir las issues en varias partes o subirle la estimación de esfuerzo.

Pueden conversar con nosotros acerca de cualquier cosa y nosotros lo consideraremos para mejorarlo.

## FAQ

### ¿Qué es el Code Review?

El code review es una práctica que consiste en revisar los pull requests de tus compañeros para validar que todo esté correcto, muchas veces se dejan comentarios con buenas prácticas de código, consultando por ciertas líneas de código que sean confusas, y en general son con la intención de ayudar a mejorar el código entregado y probar la calidad o que funcione, antes de fusionarlo con la rama principal.