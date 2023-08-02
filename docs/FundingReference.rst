.. _FundingReference:

Referencia de Financiación (FundingReference) (O)
===========

**3.19.1. Nombre según el esquema de metadatos utilizado**

*datacite:fundingReference*

**3.19.2. Etiqueta normalizada (Idioma Español)**

Referencia de financiación, organización financiadora del proyecto.

**3.19.3. Definición y alcance de la propiedad**

Contiene información de la Institución o Entidad relacionada con el apoyo financiero o la cofinanciación del proyecto y del producto de investigación que se está registrando.

**3.19.4. Niveles de persistencia (M/MA/R/O)**

Recomendado (R)

**3.19.5. Niveles de ocurrencia (R / NR)**

Repetible (R): 0-n

**3.19.6. Propiedades, atributos y especificadores**

-   **Propiedad Principal Referencias de Financiación (fundingReferences) (MA, 0-n):** Entidad que agrupa todas las entidades que financian proyectos de investigación.

    -   **SubPropiedad: Referencia de Financiación(fundingReference) (MA, 0-n):** Entidad que identifica específicamente a una entidad que financia proyectos de investigación.

        -   *SubPropiedad: Nombre del financiador (funderName) (M, 1):* Nombre del proveedor de financiamiento (Financiador). Ej: Departamento Administrativo de Ciencia, Tecnología e Innovación, MinCiencias.

        -   *SubPropiedad: Identificador único de la entidad financiadora (funderIdentifier) (R, 0-1):* Número de identificación único de la entidad financiadora. Es una propiedad opcional y única para cada **FundingReference** agregado. Ej: 0000 0001 2222 4476

            -   *Atributo Tipo de identificador único de la entidad financiadora (funderIdentifiertype) (R, 0-1):* Este atributo opcional permite especificar el número estandarizado de la entidad financiadora. Se debe tener en cuenta los siguientes tipos de identificador y su codificación normalizada según el vocabulario controlado propuesto:

+-------------------------------------+----------------------------------------------------------+-------------------------------------------+
|  **Vocabulario Normalizado**        |  **Esquema de Dominio del Vocabulario (SchemeURI)**      |     **Descripción del Elemento**          |   
|  (funderIdentifierType)             |                                                          |                                           |
+=====================================+==========================================================+===========================================+
| FUNDREF                             | http://www.crossref.org/fundref/                         | Crossref Funder Registry                  |
+-------------------------------------+----------------------------------------------------------+-------------------------------------------+
| GRID                                | https://grid.ac/                                         | Global Research Identifier Database       |
+-------------------------------------+----------------------------------------------------------+-------------------------------------------+
| ISNI                                | http://www.isni.org/                                     |International Standard Name Identifier     |
|                                     |                                                          |(ISO 27729)                                |
+-------------------------------------+----------------------------------------------------------+-------------------------------------------+
| ROR                                 | https://ror.org/                                         | Research Organization Registry Community  | 
+-------------------------------------+----------------------------------------------------------+-------------------------------------------+
| OTHERS                              |                                                          | Incluye otro tipo de identificadores para |
|                                     |                                                          | instituciones financiadoras y             |
|                                     |                                                          | patrocinadoras                            |   
+-------------------------------------+----------------------------------------------------------+-------------------------------------------+ 


Descargar Tabla [#]_ :download:`xlsx <_Downloads/3.19.6. Propiedades, atributos y especificadores.xlsx>`

                 -   *Atributo URI del Esquema (SchemeURI) (R, 0-1):* El URI del esquema de identificadores de entidades de financiación asociados con el atributo *funderIdentifiertype*

    -   *SubPropiedad: Número de adjudicación (awardNumber) (O, 1):* Esta propiedad de uso opcional, incluye el número de adjudicación exclusivamente al nombre de la entidad. Esta propiedad está pensada como un complemento aclaratorio a la propiedad *funderName*. Para el caso de proyectos financiados por MinCiencias, este atributo debe contener el número de contrato del proyecto de investigación para proyectos financiados.

            -   *Atributo URI de adjudicación (arwardURI) (R, 0-1):* Este atributo permite especificar la URI de la página del proyecto proporcionada por la organización financiadora para obtener más información de la adjudicación, concesión o financiamiento (grant).

    -   *SubPropiedad: Proyecto de Investigación / Título de adjudicación (awardTitle) (R, 0-n):* Esta propiedad de uso opcional, incluye el nombre del proyecto, adjudicación o subvención.

            -   *Atributo: ID del Proyecto de Investigación (arwardID) (O, 0-1):* Este atributo permite especificar un identificador normalizado asignado al proyecto de investigación.

**3.19.7. Forma de descripción recomendada**

    -   Para nombres de entidades utilizar el nombre completo tal y como se ha registrado legalmente con su sigla correspondiente de tal forma que la sintaxis sea: "Nombre de la Entidad" + "-" + "Sigla".

    -   En caso de múltiples entidades responsables del apoyo financiero, se debe repetir el elemento tantas veces como sea necesario. Se definen jerarquías en las entidades financiadoras, enumerar las partes de la jerarquía de mayor a menor y separarlas con puntos seguidos de un espacio. Si no queda clara la existencia de una jerarquía, o si se desconoce cuál es la parte más grande y más pequeña del cuerpo, facilitar el nombre de la entidad tal como aparece en la copia electrónica.

    -   Se debe tener claridad de la diferencia entre una entidad patrocinadora (*sponsor) y entidad financiadora (funder*). Mientras que la primera es aquella organización que asume la responsabilidad legal de la conducción general del proyecto, la segunda es la organización que proporciona los fondos para la ejecución del proyecto. Una organización puede ser tanto patrocinadora como financiadora.

**3.19.8. Equivalencias Dublin Core**

    -   dc.description.sponsorship

    -   dc.description.funder

**3.19.9. Ejemplos (XML y DATAVERSE)**

-   *Ejemplo XML*

..
+-----------------------------------------------------------------------+
| .. image:: _static/image19_2.png                                      |
|   :name: ejemplo_xml3                                                 |                                
+-----------------------------------------------------------------------+
..
-   *Ejemplo Dataverse*
..
+-----------------------------------------------------------------------+
| .. image:: _static/image19_3.png                                      |
|   :name: ejemplo_xml3                                                 |                                
+-----------------------------------------------------------------------+
..
