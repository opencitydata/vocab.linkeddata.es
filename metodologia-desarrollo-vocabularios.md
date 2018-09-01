## Guías rápidas para la creación y uso de vocabularios consensuados para publicar datos abiertos.
### Artículo 3. ¿Cómo desarrollar vocabularios?

Existen varias metodologías para el desarrollo de vocabularios. Particularmente, en este proyecto la metodología que usaremos se basa en la metodología [NeOn](https://link.springer.com/book/10.1007/978-3-642-24794-1) e involucra cuatro actividades: Especificación de Requisitos, Implementación, Publicación del Vocabulario y Mantenimiento. A continuación, se describe brevemente cada una de las actividades involucradas en el desarrollo. De manera particular se detallan las tareas de la actividad en las que se requiere la intervención de los usuarios y los expertos del dominio. Aquellas tareas que son ejecutadas únicamente por los ingenieros de ontologías se explican con menos detalle pues la intención del presente documento es facilitar la comprensión y promover la colaboración de los expertos y los usuarios durante el desarrollo de este proyecto.

**1. Especificación de Requisitos.**

El objetivo de esta actividad es capturar los requisitos que el vocabulario será capaz de cumplir, por ejemplo, determinar por qué se va a desarrollar, para qué se usará, quiénes serán los usuarios previstos. En la Especificación de Requisitos se requiere contar con un equipo multidisciplinar (generalmente conformado por ingenieros de ontologías, expertos de dominio y usuarios) que mediante un proceso de consenso definirán los requisitos. **La participación de los expertos del dominio durante esta actividad es fundamental** para asegurar una adecuada adquisición del conocimiento. Adicionalmente, esta actividad involucra la ejecución de una serie de tareas que conducen a la elaboración del Documento de Especificación de Requisitos Ontológicos, que constituye su resultado final. A continuación se describen las tareas asociadas a la actividad de Especificación de Requisitos.

La primera tarea es la *Identificación/Intercambio de Datos* en la que los expertos del dominio proveen a los ingenieros de ontologías la información relacionada con el dominio que se está modelando. Por ejemplo: conjuntos de datos, normativas, estándares, etc. La finalidad de esta tarea es proporcionar la información necesaria para que el ingeniero de ontologías tenga una idea general del dominio que tendrá que representar.

En paralelo a la tarea de *Identificación de Datos* se lleva a cabo la tarea de *Especificación de Casos de Uso*, cuyo objetivo es aportar una visión sobre el uso potencial que tendrán los datos que se modelarán. En esta tarea intervienen los expertos de dominio, los usuarios y los ingenieros de ontologías.

Los Casos de Uso, en el contexto del desarrollo de vocabularios, permiten describir situaciones que se desean alcanzar con los datos que sean descritos por el vocabulario y por lo tanto, su objetivo es guiar a la obtención de los requisitos que finalmente tendrán que ser cumplidos por este. La especificación de un Caso de Uso consiste en una descripción en la que se narra un escenario en el que uno o varios actores intervienen y las interacciones necesarias para obtener un resultado o beneficio esperado. A continuación se presenta un ejemplo de un Caso de Uso en el que se da una visión de cómo se podrían utilizar los datos recolectados por una red de sensores de aparcamiento:

  *Nombre: Caso de Uso 1 - Aparcamiento en tiempo real*

  *Descripción: Encontrar plazas de aparcamiento disponibles en determinadas zonas y horas del día es una tarea casi imposible en ciertas ciudades. Ante esta problemática un ayuntamiento ha desplegado una red de sensores en los aparcamientos públicos para obtener datos en tiempo real que le provean información acerca de las plazas libres y ocupadas. Además, ha ubicado paneles de visualización de plazas de aparcamiento disponibles en las calles y ha puesto a disposición de la ciudadanía una aplicación móvil para el estacionamiento guiado. Gracias a estas facilidades, los ciudadanos pueden saber en tiempo real en qué aparcamiento público hay sitios libres para dejar su coche.*

  *Actores: Ciudadano, Aplicación*

  *Flujo: Carlos, mientras conduce su coche de camino al centro de la ciudad, activa mediante un comando de voz la aplicación de aparcamiento. La aplicación solicita la dirección de destino. Carlos especifica a la aplicación la dirección de destino. La aplicación, que tiene acceso al GPS del móvil, inspecciona los datos emitidos por los sensores de aparcamiento, identifica cuáles son los sitios de aparcamiento más cercanos al destino de Carlos desde su ubicación actual, y le recomienda una ruta al lugar donde aparcar. Carlos sigue la ruta sugerida por la aplicación, llega a la plaza y aparca su coche.*

A continuación, la siguiente tarea es la *Definición de Historias de Usuario*. Por cada Caso de Uso se tendrán Historias de Usuario cuyo objetivo es identificar, de forma concisa, los requisitos asociados a los datos que se están modelando. Estas historias son oraciones cortas escritas en el lenguaje común de los expertos o de los usuarios, y en las que se deben identificar tres componentes:

- ¿Quién interviene?
- ¿Qué necesita?
- ¿Qué beneficio obtiene?

La estructura de una historia será: Como (actor) quiero (algo) para obtener (beneficio). Como ejemplo se muestran a continuación las Historias de Usuario generadas en base al Caso de Uso anteriormente descrito:

- *Como ciudadano quiero saber qué sitios, del aparcamiento público, están disponibles a determinada hora y dirección con la finalidad de aparcar mi coche.*

- *Como aplicación requiero obtener los datos del sensor asociado a una plaza de aparcamiento libre para realizar los cálculos necesarios para sugerir al ciudadano el sitio que mejor le convenga. Específicamente, los datos del sensor que necesito son: aparcamiento al que pertenece, número de plaza y su estado.*

Posteriormente, en la tarea de *Propuesta de Requisitos* los ingenieros de ontologías elaboran una propuesta conformada por una serie de Preguntas de Competencia (PC). Las PC son preguntas o frases escritas en lenguage natural que van acompañadas de respuestas o resultados esperados. Estas preguntas se generan a partir de los resultados de las tareas de *Identificación de Datos* y de la *Definición de Historias de Usuario*, y constituyen al final lo que el vocabulario será capaz de cumplir.

Algunos ejemplos de PC y la respuesta/resultado (R) asociadas al contexto del ejemplo anterior son:

- *PC1: ¿Qué es un sensor de aparcamiento?*

  *R1: Un sensor de aparcamiento es un dispositivo que permite detectar la presencia de un coche.*

- *PC2: ¿Cuáles son los estados en los que se puede encontrar un sensor de aparcamiento?*

  *R2: Un sensor de aparcamiento puede estar en dos estados: disponible y ocupado.*

- *PC3: En una determinada fecha, hora y dirección ¿cuál es la ubicación de los sitios de aparcamiento, en los que el sensor asociado marca su estado como disponible?*

  *R3: Listado con las coordenadas de ubicación de los sensores con estado disponible, nombre del aparcamiento al que pertenece el sensor y el número de plaza.*

Tras la *Propuesta de Requisitos*, se realiza la tarea de *Validación de Requisitos* en la que los expertos de dominio y usuarios verifican que las Preguntas de Competencia y sus respuestas/resultados son correctos y fieles a la realidad.

Finalmente, en la tarea de *Formalización de Requisitos* los ingenieros de ontologías elaboran el Documento de Especificación de Requisitos de la Ontología. Este documento es una especificación en la que se detallan el propósito y el alcance del vocabulario, los usuarios esperados, y los requisitos que el vocabulario cumplirá.

**2. Implementación del Vocabulario.**

El objetivo de esta actividad es generar el vocabulario en un lenguage formal legible por máquinas.  En la implementación el ingeniero de ontologías, tomando como entrada el Documento de Especificación de Requisitos, traslada los requisitos a un modelo conceptual que luego se codifica en un lenguage formal y finalmente se evalúa.

Para la tarea de *Modelado y Conceptualización* se requiere la contribución previa de los expertos de dominio para que provean y validen las definiciones que se irán agregando al Glosario de Términos que contendrá los conceptos involucrados en el vocabulario. Durante la *Evaluación* el ingenerio de ontologías comprueba que el vocabulario no contenga malas prácticas, tenga consistencia lógica, y que cumpla los requisitos planteados. Adicionalmente, para comprobar que los requisitos se cumplen, las Preguntas de Competencia son trasladadas a un lenguage de consulta (por ejemplo, SPARQL) que permitirá hacer peticiones de los datos, descritos previamente por el vocabulario, y obtener el resultado esperado.

**3. Publicación del Vocabulario.**

La finalidad de esta actividad es poner el vocabulario online, de tal forma que sea legible por humanos y máquinas, teniendo en cuenta las [buenas prácticas de publicación de vocabularios en la Web](https://www.w3.org/TR/swbp-vocab-pub/). En esta actividad el ingeniero de ontologías se encarga de generar la documentación, en formato html, incluyendo diagramas, descripciones (con la colaboración de los expertos del dominio) y ejemplos con la finalidad de proveer información legible por personas. Finalmente, al contar con la documentación y el código del vocabulario resultante de la actividad de implementación, el vocabulario se publica en la Web.

**4. Mantenimiento del Vocabulario.**

Esta actividad está presente durante todas las actividades anteriores, es decir durante todo el ciclo de vida del desarrollo del vocabulario. Su finalidad es gestionar nuevos requisitos, errores que puedan detectarse, o mejoras que se deseen incluir en el vocabulario. Esta gestión es realizada por el ingeniero de ontologías.

***

Esta nota ha sido creada en el contexto de la actividad "D1 - Desarrollo de vocabularios y estructuras de datos" del proyecto “Desarrollo de la Iniciativa Plataforma de Gobierno Abierto, Colaborativa e Interoperable”. Han participado en su edición tanto los adjudicatarios del proyecto (UPM, Localidata) como los responsables de las ciudades involucradas en este proyecto (Zaragoza, Madrid, Santiago de Compostela, A Coruña).

Cómo hacer referencia a este documento:

Espinoza P, Corcho O (2018) Guías rápidas para la creación y uso de vocabularios consensuados para publicar datos abiertos. 3. ¿Cómo desarrollar vocabularios? . DOI: xxxxxx
