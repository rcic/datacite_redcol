.. _Format:

Format (Formato)(O)
===========

**3.14.1. Nombre según el esquema de metadatos utilizado**

**datacite:format**

**3.14.2. Etiqueta normalizada (Idioma Español)**

Formato

**3.14.3. Definición y alcance de la propiedad**

Hace referencia a la manifestación física o digital del recurso, se puede incluir el medio del recurso. El formato es una guía para el usuario que le permite determinar el software o hardware necesario para operar el recurso.

**3.14.4. Niveles de persistencia (M/MA/R/O)**

Recomendado (R)

**3.14.5. Niveles de ocurrencia (R / NR)**

Repetible (R) : 0-n veces

**3.14.6. Propiedades, atributos y especificadores**

-   **Propiedad Principal Formatos (formats) (R, 1-n):** Incluye la información de los formatos de archivo de los datasets

    -   **SubPropiedad Formato (format) (R, 1-n):** Use la Manifestación física o digital del recurso como un valor.

**3.14.7. Forma de Descripción recomendada**

-   El campo formato del recurso de información está íntimamente ligado con el contenido y la extensión de los nombres de los archivos adjuntos.

-   La práctica recomendada consiste en seleccionar un valor de la lista registrada de IANA de tipos de medios de Internet (tipos MIME) http://www.iana.org/assignments/media-types/media-types.xhtml

-   Adicionalmente incluye información del soporte (físico/digital) utilizado y el medio requerido para acceder al recurso (Cloud, CD, DVD, etc..) si aplica.

**3.14.8. Equivalencias Dublin Core**

-   dc.format

-   dc.format.mimetype

-   dc.format.medium

**3.14.9. Ejemplos (XML y DATAVERSE)**

-   **Ejemplo XML**

..
+-----------------------------------------------------------------------+
| \<formats>                                                            |
|                                                                       |
| \<format>application/xml\</format>                                    |
|                                                                       |
| \</formats>                                                           |
+-----------------------------------------------------------------------+
..

-   **Ejemplo Dataverse**

..
+---------------------------------------------+
|.. image:: _static/image14_1.png             |
|   :name: img_dataverse14                    |
+---------------------------------------------+
..
