.. _DescripcionAplicacion:

Descripción general del perfil de aplicación
===========
El esquema de metadatos DataCite, incorpora un modelo de descripción que vá más allá del concepto tradicional de “campos de metadatos” para describir contenidos. Este modelo establece el concepto de “propiedades de metadatos”, que se definen como campos de metadatos compuestos que incluyen subcampos (subpropiedades), atributos, especificadores y vocabularios asociados.

Para el análisis de cada uno de las propiedades de metadatos que son utilizados por este conjunto de directrices, se tuvo en cuenta los siguientes componentes de evaluación:

-**Nombre de la propiedad principal**: Describe el nombre normalizado de la propiedad

-**Nombre según el esquema de metadatos utilizado**: Determina el modelo de metadatos aplicado para la definición y utilización de la propiedad.

-**Etiqueta normalizada (Idioma Español**): Nombre de la propiedad de metadatos en idioma español.

-**Definición y alcance de la propiedad**: Se exponen con precisión los conceptos de las propiedades/subpropiedades/atributos y se determina de forma clara y sencilla los objetivos que se quieren alcanzar en cada uno.

-**Niveles de persistencia (M/MA/R/O)**: Son las propiedades de existencia de los metadatos definidas así:

 -**Obligatorio = Mandatory (M)**: La propiedad siempre debe estar presente en los metadatos. No se permite un valor vacío para la propiedad.
 
 -**Obligatorio si es aplicable = Mandatory if Applicable (MA)**: Cuando se puede obtener el valor de la propiedad, debe estar presente en los metadatos.
 
 -**Recomendado = Recommended (R)**: Aunque su uso no es obligatorio, se recomienda el uso de la propiedad.
   
 -**Opcional = Optional (O)**: No es importante si la propiedad se usa o no, pero si se usa puede proporcionar información complementaria sobre el recurso.
   
**Niveles de ocurrencia (R / NR)**: Se especifica la repetibilidad o no repetibilidad de cada propiedad según su naturaleza.

   **Repetible (R)**: La propiedad de metadatos puede utilizarse 1 o más veces (1-n)
   
   **No repetible (NR)**: La propiedad de metadatos debe utilizarse solamente una vez. (1)
   
**Propiedades, atributos y especificadores**: Este apartado muestra las diversas formas de representar las propiedades a partir de su especificidad y sus características sintácticas.

**Forma de descripción recomendada**: Aquí se indica la forma correcta de la descripción de la propiedad según la normatividad internacional aplicada ó las mejores prácticas aplicables incluidas sus restricciones.

**Equivalencias Dublin Core**: Aquí se describen la relación de la propiedad con los campos del esquema de metadatos Dublin Core según el tipo de contenido referenciado al describir el recurso

**Ejemplos (XML y DATAVERSE)**: Se describen ejemplos de la forma correcta para la descripción de la propiedad, adicionalmente se muestran ayudas de despliegue de los archivos XML durante transacciones interoperabilidad (Protocolo OAI-PMH). Adicionalmente presenta un modelo de aplicación en el sistema Dataverse.



.. toctree::
   :numbered:
   :maxdepth: 1
   
   Identifier
   Creator
   Title
   Publisher
   PublicationYear
   Subject
   Contributor
   Date
   Language
   ResourceType
   AlternateIdentifier
   RelatedIdentifier
   Size
   Format
   Version
   Rights
   Description
   Geolocation
   FundingReference
   ElementosRelacionados  
