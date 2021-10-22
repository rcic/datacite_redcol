.. _ResourceType:

ResourceType (Tipo de datos) (M)
===========

**3.10.1. Nombre según el esquema de metadatos utilizado**

**datacite:resourceType**

**3.10.2. Etiqueta normalizada (Idioma Español)**

Tipología del Recurso (Tipo de datos)

**3.10.3. Definición y alcance de la propiedad**

-   Esta propiedad describe el tipo y naturaleza asociado al contenido del recurso. Se recomienda utilizar para esta propiedad valores tomados de vocabularios controlados:

    -   Vocabulario de Tipología Documental Normalizada COAR (M,1): Hace referencia al tipo de publicación basándose en un vocabulario controlado normalizado, el cual es utilizado por el usuario para identificar la categoría asociada al recurso que está mostrando.

**3.10.4. Niveles de persistencia (M/MA/R/O)**

-   Tipología Documental Normalizada COAR: Obligatorio (M,1)

-   Naturaleza del contenido DataCite (resourceTypeGeneral): Obligatorio (M,1)

**3.10.5. Niveles de ocurrencia (R / NR)**

Repetible (R) según los distintos contextos de aplicación de la tipología documental asociada.

**3.10.6. Propiedades, atributos y especificadores**

-   **Propiedad Principal Tipo de recurso de datos (resourceType) (M,1-n):** Utilice una etiqueta de texto libre para identificar el tipo de recurso como valor. Aunque se puede utilizar una etiqueta en cualquier idioma, se recomienda utilizar las etiquetas preferidas (Preferred Labels) establecidas en el vocabulario de tipologías **COAR versión 3.0**[^12]**.**

    -   **Atributo Tipología y Naturaleza del contenido DataCite (resourceTypeGeneral) (M,1):** Este atributo permite especificar el tipo de contenido asociado a la tipología documental descrita del recurso de información. Se debe tener en cuenta los siguientes tipos de contenido y su codificación normalizada según el vocabulario controlado propuesto por DataCite.

    -   **Atributo URI del identificador de la tipología COAR (resourceTypeCOAR)(R,1):** Este atributo permite especificar la URI asociada a la tipología documental normalizada según el **vocabulario de tipologías** **COAR versión 3.0,** en especial las tipologías adaptadas para datos de investigación (dataset).

**3.10.7. Forma de descripción recomendada**

-   Revise la forma adecuada para seleccionar el tipo de recurso, se recomienda utilizar los vocabularios de tipologías documentales de COAR y de Tipologías de DataCite.

    -   **Tipología y Naturaleza del Contenido del Recurso:** Se debe seleccionar el tipo de contenido del recurso según vocabulario controlado provisto por DataCite (**resourceTypeGeneral**):

.. image:: _static/image34.png
   :scale: 35%
   :name: table_tipologiaNat1

.. image:: _static/image35.png
   :scale: 35%
   :name: table_tipologiaNat2

-   **Tipología Documental Normalizada COAR para Datos de investigación:** Se debe seleccionar la etiqueta normalizada (término preferido) que corresponda con el tipo de recurso. Así mismo debe estar debidamente relacionado con una URI asociada del tipo PURL. Las tipologías adaptadas para datos de investigación (dataset) son:

+-----------+-----------+-----------+----------------------------------+
|           |           | URI       | Descripción                      |
| Concepto  | Etiqueta  |           |                                  |
| Término   | en        | (resource |                                  |
| Preferodo | español   |TypeCOAR)  |                                  |
|           |           |           |                                  |
|           |           |           |                                  |
| (resource |           |           |                                  |
|Type)      |           |           |                                  |
+===========+===========+===========+==================================+
| dataset   | conjunto  | [[h       | Una colección de hechos y datos  |
|           | de datos  | ttp://pur | relacionados codificados en una  |
|           |           | l.org/coa | estructura definida.             |
|           |           | r/resourc |                                  |
|           |           | e_type/c_ |                                  |
|           |           | ddb1]{.ul |                                  |
|           |           | }](http:/ |                                  |
|           |           | /purl.org |                                  |
|           |           | /coar/res |                                  |
|           |           | ource_typ |                                  |
|           |           | e/c_ddb1) |                                  |
+-----------+-----------+-----------+----------------------------------+
| a         | datos     | [[http:// | Estadísticas que se relacionan   |
| ggregated | agregados | purl.org/ | con clases, grupos o categorías  |
| data      |           | coar/reso | generales. Los datos se          |
|           |           | urce_type | promedian, se suman o se derivan |
|           |           | /ACF7-8YT | de otro modo de datos a nivel    |
|           |           | 9]{.ul}]( | individual, y ya no es posible   |
|           |           | http://pu | distinguir las características   |
|           |           | rl.org/co | de los individuos dentro de esas |
|           |           | ar/resour | clases, grupos o categorías.     |
|           |           | ce_type/A |                                  |
|           |           | CF7-8YT9) |                                  |
+-----------+-----------+-----------+----------------------------------+
| clinical  | ensayo    | [[h       | Datos resultantes de un estudio  |
| trial     | clínico   | ttp://pur | de investigación en el que uno o |
| data      |           | l.org/coa | más sujetos humanos se asignan   |
|           |           | r/resourc | prospectivamente a una o más     |
|           |           | e_type/c_ | intervenciones (que pueden       |
|           |           | cb28]{.ul | incluir placebo u otro control)  |
|           |           | }](http:/ | para evaluar los efectos de esas |
|           |           | /purl.org | intervenciones en los resultados |
|           |           | /coar/res | biomédicos o conductuales        |
|           |           | ource_typ | relacionados con la salud.       |
|           |           | e/c_cb28) |                                  |
+-----------+-----------+-----------+----------------------------------+
| compiled  | datos     | [[http:// | Los datos recopilados o reunidos |
| data      | c         | purl.org/ | a partir de fuentes múltiples, a |
|           | ompilados | coar/reso | menudo heterogéneas, que tienen  |
|           |           | urce_type | uno o más puntos de referencia   |
|           |           | /FXF3-D3G | en común, y al menos una de las  |
|           |           | 7]{.ul}]( | fuentes se produjo originalmente |
|           |           | http://pu | para otros fines.                |
|           |           | rl.org/co |                                  |
|           |           | ar/resour |                                  |
|           |           | ce_type/F |                                  |
|           |           | XF3-D3G7) |                                  |
+-----------+-----------+-----------+----------------------------------+
| encoded   | datos     | [[http:// | Los datos cualitativos           |
| data      | co        | purl.org/ | (textuales, video, audio o       |
|           | dificados | coar/reso | imágenes fijas) originalmente    |
|           |           | urce_type | producidos para otros propósitos |
|           |           | /AM6W-6QA | en datos cuantitativos           |
|           |           | W]{.ul}]( | (expresados en matrices unidad   |
|           |           | http://pu | por variable) mediante el uso de |
|           |           | rl.org/co | técnicas de codificación de      |
|           |           | ar/resour | acuerdo con esquemas de          |
|           |           | ce_type/A | categorización predefinidos.     |
|           |           | M6W-6QAW) |                                  |
+-----------+-----------+-----------+----------------------------------+
| exp       | datos     | [[http:// | Datos resultantes del método de  |
| erimental | exper     | purl.org/ | investigación experimental que   |
| data      | imentales | coar/reso | implica la manipulación de       |
|           |           | urce_type | algunas o todas las variables    |
|           |           | /63NG-B46 | independientes incluidas en las  |
|           |           | 5]{.ul}]( | hipótesis.                       |
|           |           | http://pu |                                  |
|           |           | rl.org/co |                                  |
|           |           | ar/resour |                                  |
|           |           | ce_type/6 |                                  |
|           |           | 3NG-B465) |                                  |
+-----------+-----------+-----------+----------------------------------+
| genomic   | datos     | [[http:// | Los datos genómicos se refieren  |
| data      | genómicos | purl.org/ | a los datos del genoma y del ADN |
|           |           | coar/reso | de un organismo. Se utilizan en  |
|           |           | urce_type | bioinformática para recolectar,  |
|           |           | /A8F1-NPV | almacenar y procesar los genomas |
|           |           | 9]{.ul}]( | de los seres vivos. Los datos    |
|           |           | http://pu | genómicos son un término más     |
|           |           | rl.org/co | extenso que los datos de         |
|           |           | ar/resour | secuenciación. Sin embargo, los  |
|           |           | ce_type/A | datos genómicos provienen        |
|           |           | 8F1-NPV9) | principalmente de técnicas de    |
|           |           |           | secuenciación. Puede incluir     |
|           |           |           | datos sin secuenciación, como    |
|           |           |           | datos de microarrays, datos de   |
|           |           |           | paneles de PCR en tiempo real y  |
|           |           |           | datos de estudios                |
|           |           |           | farmacogenómicos.                |
+-----------+-----------+-----------+----------------------------------+
| g         | datos     | [[http:// | Los datos geoespaciales          |
| eospatial | geoe      | purl.org/ | discretos generalmente se        |
| data      | spaciales | coar/reso | representan utilizando datos     |
|           |           | urce_type | vectoriales que consisten en     |
|           |           | /2H0M-X76 | puntos, líneas y polígonos,      |
|           |           | 1]{.ul}]( | mientras que los datos           |
|           |           | http://pu | geoespaciales continuos          |
|           |           | rl.org/co | generalmente se representan      |
|           |           | ar/resour | mediante datos ráster, que       |
|           |           | ce_type/2 | consisten en una cuadrícula de   |
|           |           | H0M-X761) | celdas que cada una tiene su     |
|           |           |           | propio valor.                    |
+-----------+-----------+-----------+----------------------------------+
| l         | cuaderno  | [[http:// | Un cuaderno de laboratorio es un |
| aboratory | de        | purl.org/ | registro principal de la         |
| notebook  | la        | coar/reso | investigación. Los               |
|           | boratorio | urce_type | investigadores utilizan un       |
|           |           | /H41Y-FW7 | cuaderno de laboratorio para     |
|           |           | B]{.ul}]( | documentar sus hipótesis,        |
|           |           | http://pu | experimentos y análisis o        |
|           |           | rl.org/co | interpretación inicial de estos  |
|           |           | ar/resour | experimentos.                    |
|           |           | ce_type/H |                                  |
|           |           | 41Y-FW7B) |                                  |
+-----------+-----------+-----------+----------------------------------+
| me        | datos de  | [[http:// | Datos que resultan de evaluar    |
| asurement | medición  | purl.org/ | propiedades (o características)  |
| and test  | y prueba  | coar/reso | específicas de seres, cosas,     |
| data      |           | urce_type | fenómenos (y / o procesos)       |
|           |           | /DD58-GFS | mediante la aplicación de        |
|           |           | X]{.ul}]( | estándares preestablecidos y / o |
|           |           | http://pu | instrumentos o técnicas          |
|           |           | rl.org/co | especializadas.                  |
|           |           | ar/resour |                                  |
|           |           | ce_type/D |                                  |
|           |           | D58-GFSX) |                                  |
+-----------+-----------+-----------+----------------------------------+
| obse      | datos     | [[http:// | Datos resultantes de la          |
| rvational | observ    | purl.org/ | investigación observacional, que |
| data      | acionales | coar/reso | implica recopilar observaciones  |
|           |           | urce_type | a medida que ocurren (por        |
|           |           | /FF4C-28R | ejemplo, observar                |
|           |           | K]{.ul}]( | comportamientos, eventos,        |
|           |           | http://pu | desarrollo de afecciones o       |
|           |           | rl.org/co | enfermedades, etc.), sin         |
|           |           | ar/resour | intentar manipular ninguna de    |
|           |           | ce_type/F | las variables independientes.    |
|           |           | F4C-28RK) |                                  |
+-----------+-----------+-----------+----------------------------------+
| recorded  | datos     | [[http:// | Datos registrados por medios     |
| data      | re        | purl.org/ | mecánicos o electrónicos, en una |
|           | gistrados | coar/reso | forma que permita recuperar y /  |
|           |           | urce_type | o reproducir la información. Por |
|           |           | /CQMR-7K6 | ejemplo, imágenes o sonidos en   |
|           |           | 3]{.ul}]( | disco o cinta magnética.         |
|           |           | http://pu |                                  |
|           |           | rl.org/co |                                  |
|           |           | ar/resour |                                  |
|           |           | ce_type/C |                                  |
|           |           | QMR-7K63) |                                  |
+-----------+-----------+-----------+----------------------------------+
| s         | datos de  | [[http:// | Datos que resultan del modelado  |
| imulation | s         | purl.org/ | o la representación imitativa de |
| data      | imulación | coar/reso | procesos, eventos o sistemas del |
|           |           | urce_type | mundo real, a menudo utilizando  |
|           |           | /W2XT-701 | programas de computadora.        |
|           |           | 7]{.ul}]( |                                  |
|           |           | http://pu |                                  |
|           |           | rl.org/co |                                  |
|           |           | ar/resour |                                  |
|           |           | ce_type/W |                                  |
|           |           | 2XT-7017) |                                  |
+-----------+-----------+-----------+----------------------------------+
| survey    | datos de  | [[http:// | Datos resultantes de una         |
| data      | encuesta  | purl.org/ | encuesta, que se define como una |
|           |           | coar/reso | investigación sobre las          |
|           |           | urce_type | características de una           |
|           |           | /NHD0-W6S | determinada población mediante   |
|           |           | Y]{.ul}]( | la recolección de datos de una   |
|           |           | http://pu | muestra de esa población y la    |
|           |           | rl.org/co | estimación de sus                |
|           |           | ar/resour | características mediante el uso  |
|           |           | ce_type/N | sistemático de metodología       |
|           |           | HD0-W6SY) | estadística. Se incluyen censos, |
|           |           |           | encuestas por muestreo,          |
|           |           |           | recopilación de datos de         |
|           |           |           | registros administrativos y      |
|           |           |           | actividades estadísticas         |
|           |           |           | derivadas, así como              |
|           |           |           | cuestionarios.                   |
+-----------+-----------+-----------+----------------------------------+

**3.10.8. Equivalencias Dublin Core**

-   dc.type

-   dc.type.coar

-   dc.type.content

**3.10.9. Ejemplos (XML y DATAVERSE)**

-   **Ejemplo XML**
  ..
  +-----------------------------------------------------------------------------+
  |**\<resourceType resourceTypeGeneral=\"Audiovisual\"\>encoded                |
  |data\</resourceType>**                                                       |
  +-----------------------------------------------------------------------------+
  |**\<resourceType resourceTypeGeneral=\"Workflow\"\>Software\</resourceType>**|
  +-----------------------------------------------------------------------------+
  |**\<resourceType resourceTypeGeneral=\"Dataset\"/>**                         |
  +-----------------------------------------------------------------------------+
  |**\<resourceType resourceTypeGeneral=\"Text\"\>survey data\</resourceType>** |
  +-----------------------------------------------------------------------------+
  ..

-   **Ejemplo Dataverse**

.. image:: _static/image36.png
   :scale: 35%
   :name: table_tipologiaNat2
