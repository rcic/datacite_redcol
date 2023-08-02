.. _AlternateIdentifier:

Alternate Identifier (Identificador alternativo)(O)
===========

**3.11.1. Nombre según el esquema de metadatos utilizado**

**datacite:alternateIdentifier**

**3.11.2. Etiqueta normalizada (Idioma Español)**

Identificador alternativo

**3.11.3. Definición y alcance de la propiedad**

Un identificador o identificadores distintos del identificador primario aplicado al recurso que se está registrando. Puede ser cualquier cadena alfanumérica que sea única dentro de su dominio de emisión. Puede utilizarse para identificadores locales. Este campo debe usarse para describir distintos identificadores de la misma instancia (misma ubicación, mismo archivo)

**3.11.4. Niveles de persistencia (M/MA/R/O)**

Recomendado (R)

**3.11.5. Niveles de ocurrencia (R / NR**)

Repetible (R): 0-n veces

**3.11.6. Propiedades, atributos y especificadores**

-   **Propiedad Principal Identificadores Alternativos (alternateIdentifiers)(R, 0-n)**: Permite describir distintos identificadores de la misma instancia (misma ubicación, mismo archivo)

    -   **SubPropiedad Identificador Alternativo (alternateIdentifier) (R, 0-n)**: Esta propiedad permite especificar el valor del identificador alternativo que se le ha otorgado al recurso.

        -   **Atributo: Tipo de identificador alternativo (alternateIdentifierType) (M, si alternateIdentifier es utilizado, 1):** Este atributo permite especificar el tipo de identificador alternativo que se le ha otorgado al recurso. Se debe tener en cuenta los siguientes tipos de identificadores y su codificación normalizada según el vocabulario controlado propuesto:

              +-------------------------+------------------------------------------------------------+----------------------------------------+
              |Vocabulario Normalizado  | **Descripción del atributo**                               | **Dominio de Vocabulario**             |
              |                         |                                                            |                                        |
              +=========================+============================================================+========================================+
              |  ARK                    | Clave de recursos de archivo                               | datacite                               |
              +-------------------------+------------------------------------------------------------+----------------------------------------+
              |  ARXIV                  | Identificador de https://arxiv.org/                        | datacite                               |
              +-------------------------+------------------------------------------------------------+----------------------------------------+
              |  BIBCODE                | Códigos bibliográficos del Sistema de Datos Astrofísicos   | datacite                               |
              |                         | bibcodes se pueden resolver a través de                    |                                        |
              |                         | http://adsabs.harvard.edu/abs/bibcode                      |                                        |                   
              +-------------------------+------------------------------------------------------------+----------------------------------------+
              |  DOI                    | Identificador de Objeto Digital. Código alfanumérico que   | datacite                               |
              |                         | sirva para identificar de forma única un documento digital.|                                        |
              |                         |                                                            |                                        |                   
              +-------------------------+------------------------------------------------------------+----------------------------------------+
              |  EANN13                 | Número de artículo europeo, ahora renombrado como Número de| datacite                               |
              |                         | artículo internacional, pero que conserva el acrónimo      |                                        |
              |                         | original, es un estándar de código de barras de 13 dígitos |                                        |  
              |                         | que es un superconjunto del sistema del Código de producto |                                        |
              |                         | universal (UPC)                                            |                                        |         
              +-------------------------+------------------------------------------------------------+----------------------------------------+
              |  EISSN                  | Número internacional normalizado de publicaciones seriadas | datacite                               |
              |                         | (versión electrónica), permite identificar de manera única |                                        |
              |                         | una colección seriada evitando posibles errores en la      |                                        |  
              |                         | transcripción del título o información bibliográfica.      |                                        |
              |                         | universal (UPC)                                            |                                        |  
              +-------------------------+------------------------------------------------------------+----------------------------------------+
              | HANDLE                  | Es un identificador persistente, es decir, un sistema de   |  datacite                              |  
              |                         | especificación para nombres e identificación de servicios. |                                        |  
              +-------------------------+------------------------------------------------------------+----------------------------------------+
              |  IGSN                   | Número de muestra internacional Geo; un código alfanumérico| datacite                               |
              |                         | de 9 dígitos que identifica de forma exclusiva muestras de |                                        |
              |                         | nuestro entorno natural y funciones de muestreo            |                                        |  
              |                         | relacionadas                                               |                                        |  
              +-------------------------+------------------------------------------------------------+----------------------------------------+
              |  ISBN                   |Número internacional normalizado de libros, es un           | datacite                               |
              |                         |identificador único para libros, previsto para su uso       |                                        |
              |                         |comercial                                                   |                                        |
              +-------------------------+------------------------------------------------------------+----------------------------------------+
              |  ISSN                   |Número internacional normalizado de publicaciones seriadas, | datacite                               |
              |                         |permite identificar de manera única una colección seriada   |                                        |                           
              |                         |evitando posibles errores en la transcripción del título o  |                                        |                           
              |                         |información bibliográfica                                   |                                        |                           
              +-------------------------+------------------------------------------------------------+----------------------------------------+
              | ISTC                    |Código internacional normalizado de obras textuales, es un  | datacite                               | 
              |                         |identificador único para obras textuales siempre y cuando   |                                        |
              |                         |exista una intención de producir dicha obra en forma de una |                                        |                   
              |                         |o más manifestaciones.                                      |                                        |
              +-------------------------+------------------------------------------------------------+----------------------------------------+
              | LISSN                   | Es un número específico que reúne los diferentes           | datacite                               |
              |                         | soportes en los que se edita una publicación seriada.      |                                        |
              +-------------------------+------------------------------------------------------------+----------------------------------------+
              |LOCAL                    | Identificador Local                                        | RedCol                                 |
              +-------------------------+------------------------------------------------------------+----------------------------------------+
              |  LSID                   |Es el identificador único de las ciencias naturales,        | datacite                               |
              |                         |considerándose una especificación en curso del Nombre       |                                        |                           
              |                         |del Recurso Uniforme (URN) y permite identificar los        |                                        |                           
              |                         |recursos en diferentes almacenes de datos biológicamente    |                                        |
              |                         |significativos.                                             |                                        |  
              +-------------------------+------------------------------------------------------------+----------------------------------------+
              |  PISSN                  |Número internacional normalizado de publicaciones           | datacite                               |
              |                         |seriadas, permite identificar de manera única una colección |                                        |                           
              |                         |seriada evitando posibles errores en la transcripción del   |                                        |                           
              |                         |título o información bibliográfica. (versión impresa)       |                                        |
              |                         |                                                            |                                        |  
              +-------------------------+------------------------------------------------------------+----------------------------------------+
              |PMID                     |ID de PubMed. Número único asignado a cada cita de          | datacite                               |     
              |                         |artículo de revistas biomédicas y de las ciencias naturales.|                                        |
              +-------------------------+------------------------------------------------------------+----------------------------------------+
              | PURL                    |Localizador de recursos uniforme y persistente, se utiliza  | datacite                               |
              |                         |para referenciar un determinado recurso que cambia de       |                                        |                           
              |                         |dirección a lo largo del tiempo desde una misma dirección.  |                                        |                           
              |                         |                                                            |                                        |
              +-------------------------+------------------------------------------------------------+----------------------------------------+
              | UPC                     |Código de producto universal, es un código de barras        | datacite                               |
              |                         |utilizado para rastrear artículos comerciales. Su forma más |                                        |                           
              |                         |común, la UPC-A, consta de 12 dígitos numéricos.            |                                        |                           
              |                         |                                                            |                                        |
              +-------------------------+------------------------------------------------------------+----------------------------------------+
              | URL                     |Localizador Uniforme de Recursos, es la dirección específica| datacite                               |
              |                         |que se le asigna a cada uno de los recursos disponibles     |                                        |                           
              |                         |en la red con el fin de localizarlos e identificarlos       |                                        |                           
              |                         |fácilmente.                                                 |                                        |
              +-------------------------+------------------------------------------------------------+----------------------------------------+
              | URN                     |Nombre del recurso uniforme, permite identificar recursos   | datacite                               |
              |                         |en la web pero no indica exactamente dónde se encuentra     |                                        |                           
              |                         |el recurso                                                  |                                        |                           
              |                         |                                                            |                                        |
              +-------------------------+------------------------------------------------------------+----------------------------------------+
              | W3ID                    |Identificador permanente para aplicaciones web. Se utiliza  | datacite                               |
              |                         |principalmente para publicar vocabularios y ontologías.     |                                        |                           
              |                         |                                                            |                                        |
              +-------------------------+------------------------------------------------------------+----------------------------------------+
              | WOS                     |Número de acceso a la Web of Science, es una identificación | datacite                               |
              |                         |asociada a cada registro del producto, formado por el número|                                        |                           
              |                         |de acceso del productor y un número secuencial.             |                                        |
              +-------------------------+------------------------------------------------------------+----------------------------------------+
              | OTHER                   |Otros tipos de identificadores alternativos del recurso.    | RedCol                                 |
              |                         |asociada a cada registro del producto, formado por el número|                                        | 
              +-------------------------+------------------------------------------------------------+----------------------------------------+    					
                        
   



Descargar Tabla [#]_ :download:`xlsx <_Downloads/3.11.6. Propiedades, atributos y especificadores.xlsx>`


**3.11.7. Forma de descripción recomendada**

-   **Identificador Alternativo:** Identificador del recurso, puede ser una cadena alfanumérica que sea única dentro de su dominio o emisión.

    -   Para el ingreso de ISBN no incluya guiones (-).

    -   Para el caso del PURL, coloque la URL completa.

    -   Para el Ingreso de DOI no incluya los datos de la URL (http://doi.org)

    -   Pueden utilizarse para identificadores locales (Signaturas, Códigos de barras, Números de inventarios etc)

**3.11.8. Equivalencias Dublin Core**

    -   dc.identifier

    -   dc.identifier.doi

    -   dc.identifier.local

    -   dc.identifier.isbn

    -   dc.identifier.issn

    -   dc.identifier.uri

    -   dc.identifier.url

    -   dc.identifier.other

**3.11.9. Ejemplos (XML y DATAVERSE)**

-   Ejemplo XML

..
                             
+-----------------------------------------------------------------------+
| .. image:: _static/image1001.jpg                                      |
|                                                                       |
|   :name: ejemplo_xml3                                                 |                                
+-----------------------------------------------------------------------+
..

-   Ejemplo Dataverse

+-----------------------------------------------------------------------+
| .. image:: _static/image42.png                                        |
|                                                                       |
|   :name: ejemplo_xml3                                                 |                                
+-----------------------------------------------------------------------+
