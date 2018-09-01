## Guías rápidas para la creación y uso de vocabularios consensuados para publicar datos abiertos.
### Artículo 2. Ventajas del uso de vocabularios (dirigido a miembros de las administraciones públicas - expertos de dominio - y usuarios)


**¿Qué es un vocabulario?**

Un vocabulario define conceptos y las relaciones utilizadas para describir y representar un área de interés. (Definición adaptada de la [W3C](https://www.w3.org/standards/semanticweb/ontology)). En otras palabras, un vocabulario es un modelo común que permite describir el conocimiento asociado a un dominio, y que se define formalmente mediante un lenguage legible por máquinas.

**¿Para qué son útiles los vocabularios en el contexto de la publicación de datos abiertos?**

- **Permiten describir los datos de una forma más precisa**, evitando de esta manera ambigüedades en el uso de los datos (por ejemplo, ¿qué significa esta columna? ¿qué valores tiene? ¿qué significa la ausencia de valor en una celda del CSV?). En todo momento se podrá enlazar con la definición completa de lo que significa una columna de la tabla correspondiente a un conjunto de datos (por ejemplo, http://vocab.linkeddata.es/datosabiertos/def/sector-publico/territorio#distrito)
- **Permiten describir los datos de una forma más homogénea y reutilizable**. Al compartir estos modelos consensuados con otras administraciones públicas (y con otros departamentos de la misma administración), que también publican y/o usan datos similares, se facilita la homogeneización de todos los datos. De esta manera, todas las ciudades publicarán sus datos de manera similar, facilitando su reutilización (no hace falta crear adaptadores a cada formato de datos cada vez que una aplicación tiene que desplegarse en una administración distinta, lo que hace posible que se creen aplicaciones “globales” aplicables a cualquier ciudad).
- **La información irá mejorando su calidad con el tiempo**. Tener modelos consensuados permite identificar qué datos faltan en nuestras fuentes de datos originales y determinar si se pueden encontrar, así como identificar buenas prácticas en la representación de los datos que pueden dar lugar a mejoras en las fuentes de datos originales.
- **Los conjuntos de datos se pueden relacionar más fácilmente entre sí**. En la creación de vocabularios siempre se intentan reutilizar fragmentos de otros vocabularios que ya han sido consensuados previamente, lo que facilita no sólo mayor homogeneidad, sino también la posibilidad de enlazar los conjuntos de datos entre sí. Por ejemplo, tres conjuntos de datos (locales comerciales, bicicletas de alquiler y censo de la ciudad) que usan datos del callejero de la ciudad, podrán enlazarse más fácilmente entre sí para hacer consultas cruzadas si se unifica la manera de representar los datos de calles de la ciudad

**¿Qué actores son necesarios para crear un buen vocabulario?**

Para la creación de vocabularios se requiere la participación de los siguientes actores:
- **ingenieros de ontologías**, expertos en desarrollo de vocabularios.
- **expertos del dominio**, aquellas personas con el conocimiento en el área que se va a modelar.
- **usuarios**, aquellos que utilizarán los datos.

**¿Cómo se desarrolla un vocabulario?**

Existen varias metodologías para desarrollar vocabularios; cada una de ellas proporciona sus propias guías para describir las actividades que se deben llevar a cabo, los actores involucrados, y los resultados esperados tras cada actividad. Particularmente, en este proyecto la metodología que usaremos involucra cuatro actividades: Especificación de Requisitos, Implementación,  Publicación del Vocabulario y Mantenimiento. Los detalles relacionados con las tareas que se realizan en estas actividades y la participación de los actores, descritos anteriormente, se pueden encontrar en el [Artículo 3. ¿Cómo desarrollar vocabularios?](https://github.com/opencitydata/vocab.linkeddata.es/blob/master/metodologia-desarrollo-vocabularios.md).

--

Esta nota ha sido creada en el contexto de la actividad "D1 - Desarrollo de vocabularios y estructuras de datos" del proyecto “Desarrollo de la Iniciativa Plataforma de Gobierno Abierto, Colaborativa e Interoperable”. Han participado en su edición tanto los adjudicatarios del proyecto (UPM, Localidata) como responsables de las ciudades involucradas en este proyecto (Zaragoza, Madrid, Santiago de Compostela, A Coruña).

Cómo hacer referencia a este documento:
Espinoza P, Corcho O, Crespo HE (2018) Guías rápidas para la creación y uso de vocabularios consensuados para publicar datos abiertos. 2. Ventajas del uso de vocabularios (dirigido a miembros de las administraciones públicas - expertos de dominio - y usuarios). DOI: xxxxxx
