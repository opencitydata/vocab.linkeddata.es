## Guías rápidas para la creación y uso de vocabularios consensuados para publicar datos abiertos.
### Artículo 1. Contexto y ventajas estratégicas generales (dirigido a administraciones públicas)

En la última década han proliferado en España multitud de portales de datos abiertos gubernamentales en todos los ámbitos de la administración, siguiendo una tendencia que se ha consolidado en todo el mundo tanto desde la perspectiva legal (con leyes y acuerdos supra-nacionales, nacionales, autonómicos e incluso locales, todos ellos relacionados con la [reutilización de la información del sector público](https://datos.gob.es/es/documentacion?f%5B0%5D=field_doc_tx_type%3A316)) como tecnológica (con sistemas abiertos y propietarios que dan soporte al proceso de publicación y explotación de datos). En especial, son de destacar los portales de datos abiertos de los municipios, que según los datos disponibles en https://datos.gob.es/es/iniciativas a 30 de julio de 2018 suman un total de 225 entidades locales en España.

Desde el año 2015, en el que comenzó la red temática española sobre datos abiertos y ciudades inteligentes, se ha venido manteniendo el repositorio http://vocab.linkeddata.es/datosabiertos/ para la publicación de vocabularios que puedan servir como base para la publicación de datos abiertos, y la organización en GitHub https://github.com/opencitydata, donde se gestiona el ciclo de vida de dichos vocabularios. En otra de las guías rápidas de esta serie se describe qué es y qué papel juega un vocabulario en la publicación de datos abiertos (enlace).

En todo caso, se debe tener en cuenta que, excepto en casos puntuales, hasta ahora la mayor parte del desarrollo de estos vocabularios ha sido realizada de manera voluntaria por grupos de trabajo informales (por ejemplo, los del grupo de trabajo AENOR de datos abiertos y ciudades inteligentes, los de la iniciativa OjoAlData100), en el contexto de algunos proyectos de I+D+i (por ejemplo, el vocabulario de contratación pública [PPROC](http://contsem.unizar.es/def/sector-publico/pproc)), o en el contexto de trabajos fin de grado y fin de máster realizados por estudiantes (por ejemplo, los vocabularios de [contaminación acústica](https://github.com/opencitydata/medio-ambiente-contaminacion-acustica) o de [equipamientos](https://github.com/opencitydata/sociedad-bienestar-equipamientos-municipales)). Un [informe](https://datos.gob.es/es/documentacion/vocabularios-de-representacion-de-datos-abiertos-en-ciudades-digitales) reciente encargado por red.es repasa algunas de las características (y limitaciones) de dichos vocabularios.

Teniendo en cuenta este contexto, puede surgir la pregunta de “¿por qué es relevante utilizar vocabularios consensuados para la publicación de datos abiertos?”. En este documento pretendemos dar algunas razones por las que puede ser útil invertir esfuerzo en la creación de dichos vocabularios:

**1. Otros también lo hacen**

  En España (y con las iniciativas anteriormente mencionadas) no somos los únicos que estamos trabajando en la definición de vocabularios consensuados para la publicación de datos abiertos. Algunas iniciativas internacionales relevantes en el área de datos abiertos son:
  - Los vocabularios W3C para representar organizaciones ([W3C Organization Ontology](https://www.w3.org/TR/vocab-org/)), datos de sensores ([SSN Ontology](https://www.w3.org/TR/vocab-ssn/)), datos estadísticos y multidimensionales ([RDF Data Cube](https://www.w3.org/TR/vocab-data-cube/)), etc.
  - Los [vocabularios “core”](https://ec.europa.eu/isa2/solutions/core-vocabularies_en) definidos por la iniciativa europea [ISA2](https://ec.europa.eu/isa2/home_en) en el contexto del marco de interoperabilidad europeo. Estos vocabularios sencillos determinan cómo representar personas, organizaciones, lugares, servicios públicos, eventos, etc.
  - Los vocabularios que están siendo desarrollados por instituciones como la European Publications Office, para la representación de procesos de contratación pública.

Tampoco es el dominio de los datos abiertos (y las ciudades) el único en el que se están realizando esfuerzos para la creación de vocabularios consensuados. Por ejemplo, son conocidos en otras disciplinas los portales de vocabularios para biología ([BioPortal](https://bioportal.bioontology.org/)), . Y también hay portales genéricos que permiten realizar búsquedas en vocabularios, como la iniciativa [schema.org](https://schema.org/) o el portal [Linked Open Vocabularies](https://lov.linkeddata.es/).

**2. Reducimos el Total Cost of Ownership (TCO) global**

  Si tenemos en cuenta el esfuerzo que los reutilizadores de nuestros datos públicos tienen que emplear para analizar los datos tal y como han sido publicados por cada municipio (con distintas estructuras de datos, formatos, convenciones para la descripción de códigos, etc.), y homogeneizarlos para crear aplicaciones globales, que puedan ser desplegadas en todo el territorio nacional, llegaremos a la conclusión de que es preferible que los productores de datos lleguen a un acuerdo para publicar los datos de manera homogénea (usando las mismas estructuras siempre que sea posible, los mismos formatos y las mismas convenciones), facilitando la labor global de toda la comunidad de reutilización de datos. Esto no quiere decir que todo el trabajo tenga que recaer sobre los productores de datos (los municipios), pues quizás se puede llegar a acuerdos con algunos reutilizadores, en iniciativas público-privadas, para que ayuden a realizar esta homogeneización.

**3. Los productores de datos pueden colaborar en la explotación de los datos, incrementando su competitividad y la calidad de las aplicaciones que los explotan**

  Si se homogeneizan los datos que se producen, se puede colaborar en la creación de visualizaciones, en el desarrollo de scripts y programas que faciliten la curación de los datos, en el desarrollo de aplicaciones, etc., reduciendo el coste total de desarrollo (al no tener que desarrollar desde cero o crear adaptadores para N municipios) y facilitando la creación de servicios de valor añadido mucho más robustos y/o innovadores, al poder concentrar el esfuerzo en una única línea de código.

**4. Se aprende de los datos que otros tienen y se puede mejorar la gestión interna de los datos**

Al consensuar estructuras de datos comunes, se pueden identificar atributos que no son cubiertos por los datos de los que se dispone dentro de la organización municipal, y que pueden ser interesantes. También se puede aprender de cómo se ha mejorado la calidad de los datos en otras organizaciones, e intercambiar experiencias.

**5. Si no se dispone de un conjunto de datos y se quiere incorporar en la organización en el futuro, ya hay un ejemplo a seguir**

El modelo que se ha creado de manera consensuada puede ser útil en el caso de que una organización (un municipio) no disponga de datos de un tipo concreto pero quiera comenzar a gestionarlos. Al disponer de un modelo consensuado, ya no necesita realizar la labor de desarrollo del modelo de datos a utilizar, pues ya ha sido creado previamente por otras organizaciones que tenían experiencia en su tratamiento.

Estas son algunas de las razones que pueden justificar la adopción de una estrategia de desarrollo consensuado de vocabularios para datos abiertos. Para facilitar la muy necesaria labor de discusión y de realización de acuerdos sobre dichos vocabularios existen metodologías, procedentes del área de la Ingeniería Ontológica, que pueden ser aplicadas. La aplicación de estas metodologías para cada conjunto de datos y vocabulario a explorar dará como resultado no sólo una representación formal del modelo consensuado como los que han sido identificados al comienzo de este documento (por ejemplo, la W3C Organization Ontology, el Core Public Vocabulary sobre personas, muchas de las clases de schema.org, etc.) sino también suficiente documentación adicional (preguntas de competencia e historias de usuario, especificación de requisitos, modelos conceptuales de alto nivel, etc.) para permitir comprender la razón por la que se ha llegado a un determinado acuerdo o el ámbito en el que se puede utilizar el vocabulario en cuestión.

***

Esta nota ha sido creada en el contexto de la actividad "D1 - Desarrollo de vocabularios y estructuras de datos" del proyecto “Desarrollo de la Iniciativa Plataforma de Gobierno Abierto, Colaborativa e Interoperable”. Han participado en su edición tanto los adjudicatarios del proyecto (UPM, Localidata) como los responsables de las ciudades involucradas en este proyecto (Zaragoza, Madrid, Santiago de Compostela, A Coruña).

Cómo hacer referencia a este documento:

Corcho O, Espinoza P (2018) Guías rápidas para la creación y uso de vocabularios consensuados para publicar datos abiertos. 1. Contexto y ventajas estratégicas generales (dirigido a administraciones públicas). DOI: xxxxxx
