.. _ElementosRelacionados:

Elementos Relacionados (RelatedItem) (O)
===========

**3.20.1. Nombre según el esquema de metadatos utilizado**

*datacite:relatedItem*

**3.20.2. Etiqueta normalizada (Idioma Español)**

Elementos relacionados

**3.20.3. Definición y alcance de la propiedad**

Esta propiedad contiene la descripción ampliada de los recursos
relacionados con el recursos que se está describiendo. Esta propiedad,
se puede usar para describir todo tipo de recursos donde la propiedad
*relatedIdentifier* no se puede usar porque el recurso relacionado no
tiene un identificador (por ejemplo, documentos de trabajo, literatura
gris, etc..).

**3.20.4. Niveles de persistencia (M/MA/R/O)**

Opcional (O)

**3.20.5. Niveles de ocurrencia (R / NR)**

Repetible (R) 0-n veces.

**3.20.6. Propiedades, atributos y especificadores**

-   *Propiedad Principal Elementos relacionados (relatedItems) (O,0-n):* Descripción de los distintos elementos relacionados

    -   *SubPropiedad Elemento relacionado (relatedItem) (R,1-n):* Detalle ampliado de un recurso relacionado

        -   *Atributo Tipo de Elemento relacionado (relatedItemType) (M,1):* Contiene la tipología documental asociada a la naturaleza del recurso. Se debe utilizar el mismo vocabulario definido anteriormente para el atributo *resourceTypeGeneral* de la propiedad *resourceType.*

        -   *Atributo Tipo de relación (relationType) (M,1):* Descripción de la relación del recurso que se está registrando (A) y el recurso relacionado (B). Se debe utilizar el mismo vocabulario definido anteriormente para el atributo *relationType* de la propiedad *relatedIdentifier*

    -   *SubPropiedad identificador relacionado (relatedItemIdentifier)(O,0-1):* Información del identificador del elemento relacionado

        -   *Atributo Tipo de identificador relacionado (relatedItemIdentifierType) (O,0-1):* Contiene el tipo del identificador del elemento relacionado. Se debe utilizar el mismo vocabulario definido anteriormente para el atributo *relatedIdentifierType* de la propiedad *relatedIdentifier*

        -   *Atributo: Esquema de metadatos relacionado (relatedMetadataScheme) (O, 0-1):* Este atributo permite establecer un esquema de metadatos utilizado para describir la relación del identificador. Este atributo debe ser únicamente utilizado si el atributo anterior *relationType* es utilizado y este contiene los valores (HasMetadata/IsMetadataFor).

        -   *Atributo: URI del esquema de metadatos relacionado (schemeURI) (O, 0-1):* Este atributo permite establecer la URI normalizada del esquema de metadatos utilizado para describir la relación del identificador en un formato estándar (XSD,DDT, Turtle) . Este atributo debe ser únicamente utilizado si el atributo anterior *relationType* es utilizado y este contiene los valores (HasMetadata/IsMetadataFor).

        -   *Atributo: Tipo de esquema de metadatos relacionado (schemeType) (O, 0-1):* Este atributo contiene el tipo de formato del esquema de metadatos que fue vinculado en el atributo anterior schemeURI (XSD,DDT, Turtle). Este atributo debe ser únicamente utilizado si el atributo anterior relationType es utilizado y este contiene los valores (HasMetadata/IsMetadataFor).

    -   *SubPropiedad Autores (Creators) (O,0-n):* Describa los distintos autores del recurso relacionado.

        -   *SubPropiedad Autor (Creator) (O,0-n):* La institución o persona responsable por la creación del recurso relacionado.

            -   *Atributo Nombre completo (creatorName) (R,1)*

            -   *Atributo Tipo de autor (nameType)(O,0-1)*

            -   *Atributo Nombre (givenName)(O,0-1)*

            -   *Atributo Apellido (familyName)(O,0-1)*

    -   *SubPropiedad Títulos del recurso relacionado (titles)(R,1-n):* Describa los distintos títulos del recurso relacionado

        -   *SupPropiedad Título del recurso relacionado (title)(R,1-n):* Título propiamente dicho del recurso relacionado

            -   *Atributo IDIOMA (xml:lang) (O, 0-1):* Este atributo especifica el idioma utilizado en la descripción. Se debe tener en cuenta su codificación normalizada según el vocabulario propuesto por el estándar ISO 639-3 utilizando carácteres en UTF-8 (https://iso639-3.sil.org/code_tables/download_tables**)**

            -   *Atributo Tipo de Título del recurso relacionado (titleType)(O,0-1):* Especifica el tipo de título del siguiente vocabulario controlado:

  ..
  +----------------------------+------------------------------------------+
  |Vocabulario Normalizado     |    Descripción                           |
  +============================+==========================================+
  |AlternativeTitle            |    Título Alternativo / Variantes del    |
  |                            |    Título                                |
  +----------------------------+------------------------------------------+
  |Subtitle                    |      Subtítulo (Recomendado unificar en  |
  |                            |      Título: Subtítulo)                  |
  +----------------------------+------------------------------------------+
  |TranslatedTitle             |      Título Traducido                    |
  +----------------------------+------------------------------------------+
  |Other                       |      Otros Títulos                       |
  +----------------------------+------------------------------------------+
  ..

-   *Subpropiedad Año de publicación (publicationYear)(O,0-1):* Especifica el año de publicación del recurso relacionado

-   *SubPropiedad Volumen (volume)(O,0-1): Especifica el volumen de un recurso continuo relacionado*

-   *Subpropiedad Ejemplar (issue)(O,0-1): Especifica el ejemplar de unrecurso continuo relacionado*

-   *Subpropiedad Número (number)(O,0-1): Especifica el número de un recurso continuo relacionado*

    -   *Atributo Tipo del número del ejemplar (numberType) (O,0-1):* Tipo de número del artículo relacionado seleccionado del siguiente vocabulario controlado:

  ..
  +----------------------------+
  |Vocabulario Normalizado     |
  +============================+
  |Article                     |
  |                            |
  +----------------------------+
  |Chapter                     |
  |                            |
  +----------------------------+
  |Report                      |
  +----------------------------+
  |Other                       |
  +----------------------------+
  ..

-   *SubPropiedad Página inicial (firstPage)(O,0-1):* Indica la página inicial del recurso

-   *SubPropiedad Página Final (lastPage)(O,0-1):* Indica la página final del recurso

-   *SubPropiedad Editor (Publisher)(O,0-1):* El nombre de la entidad que posee, archiva, publica impresiones, distribuye, libera, emite o produce el recurso. Esta propiedad se utilizará para formular la cita, así que considere la prominencia del rol.

-   *SubPropiedad Número de Edición (edition)(O,0-1):* Edición o versión del artículo relacionado.

-   *SubPropiedad Colaboradores (Contributors)(O,0-n):*

    -   *SubPropiedad Colaborador (Contributor)(R,1-n):* The institution or person responsible for collecting, managing, distributing, or otherwise contributing to the development of the resource.

        -   *Atributo tipo de Rol (contributorType)(R,1):* El tipo de colaboración del recurso relacionado. Se debe utilizar el mismo vocabulario definido anteriormente para el atributo *contributorType* de la propiedad *contributor*

        -   *Atributo Nombre completo (contributorName)(R,1)*

        -   *Atributo Tipo de autor (nameType)(O,0-1)*

        -   *Atributo Nombre (givenName)(O,0-1)*

        -   *Atributo Apellido (familyName)(O,0-1)*

**3.20.7. Forma de Descripción Normalizada (RDA / RCAA2 / ISBD)**

-   Utilice este campo para describir detalles específicos de publicaciones seriadas que previamente se codificaban en un campo de descripción con descriptionType= "*SeriesInformation*"

-   El atributo *relationType=\"IsPublishedIn*\" se puede utilizar para incluir información de la serie, como título, volumen, número, página, etc.

-   El atributo *relatedItemType, utiliza el mismo vocabulario controlado de tipologías documentales asociadas a la naturaleza del contenido de la propiedad **resourceType* y su atributo *resourceTypeGeneral*

**3.20.8. Equivalencias Dublin Core**

-   dc.relation

-   dc.relation.ispartofseries

-   dc.relation.ispartofjournal

-   dc.relation.ispartofbook

-   dc.relation.ispartofconference

**3.20.9. Ejemplos (XML y DATAVERSE)**

-   Ejemplo XML
..
+-----------------------------------------------------------------------+
| .. image:: _static/image20_3.png                                      |
|   :scale: 35%                                                         |
|   :name: ejemplo_xml3                                                 |                                
+-----------------------------------------------------------------------+
..
-   Ejemplo Dataverse
..
+-----------------------------------------------------------------------+
| .. image:: _static/image20_4.png                                      |
|   :scale: 35%                                                         |
|   :name: ejemplo_xml3                                                 |                                
+-----------------------------------------------------------------------+
| .. image:: _static/image20_5.png                                      |
|   :scale: 35%                                                         |
|   :name: ejemplo_xml3                                                 |                                
+-----------------------------------------------------------------------+
..
