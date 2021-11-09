.. _Geolocation:

Geolocation(Ubicación geográfica)(O)
===========

*3.18. Geolocation(Ubicación geográfica)(O)*

*3.18.1. Nombre según el esquema de metadatos utilizado*

*datacite:geoLocation*

*3.18.2. Etiqueta normalizada (Idioma Español)*

Ubicación geográfica

*3.18.3. Definición y alcance de la propiedad*

Este campo se utiliza para describir los lugares geográficos donde se llevaron a cabo las investigaciones o el lugar de referencia dentro del recurso (Región espacial o lugar con nombre donde se recopilaron los datos o sobre los cuales se enfocaron los datos.) ó lugar de publicación del recurso.

*3.18.4. Niveles de persistencia (M/MA/R/O)*

Opcional (O)

*3.18.5. Niveles de ocurrencia (R / NR)*

Repetible (R): 0-n veces. Repita el campo si el recurso incluye ubicaciones geográficas diferentes.

*3.18.6. Propiedades, atributos y especificadores*

-   *Propiedad Principal Ubicaciones Geográficas (geoLocations) (O, 0-n):* Describa todas las posibles regiones espaciales o lugares con nombre donde se recopilaron los datos o sobre los cuales se enfocaron los datos.

-   *SubPropiedad: Ubicación Geográfica (geoLocation) (O, 0-n):* Describa cada una de las posibles ubicaciones geográficas asociadas. Repita esta propiedad para indicar varias ubicaciones diferentes.

    -   *SubPropiedad: Lugar Geográfico (geoLocationPlace) (O, 0-n)*: Descripción de una ubicación geográfica

    -   *SubPropiedad: Punto Geográfico (geoLocationPoint) (O, 0-n):* Un punto de ubicación en el espacio. Un punto contiene un solo par de latitud-longitud.

        -   *SubPropiedad: Punto Longitud (pointLongitude) (M, 1):* Dimensión longitudinal del punto.

        -   *SubPropiedad: Punto Latitud (pointLatitude) (M, 1):* Dimensión latitudinal del punto.

    -   *SubPropiedad: Punto Geográfico (geoLocationBox) (O, 0-n) :* Los límites espaciales de un lugar o cuadro.

        -   *SubPropiedad: Punto Longitud (westBoundLongitude) (M, 1):* Coordenada (Longitud) de la Esquina Superior Izquierda.

        -   *SubPropiedad: Punto Latitud (northBoundLatitude) (M, 1):* Coordenada (Latitud) de la Esquina Superior Izquierda.

        -   *SubPropiedad: Punto Longitud (eastBoundLongitude) (M, 1):* Coordenada (Longitud) de la Esquina Inferior Derecha.

        -   *SubPropiedad: Punto Latitud (southBoundLatitude) (M, 1):* Coordenada (Latitud) de la Esquina Inferior Derecha.

    -   *SubPropiedad: Polígono Geográfico (geoLocationPolygon) (O, 0-n) :* Un área de polígono dibujado, definida por un conjunto de puntos y líneas que conectan los puntos en una cadena cerrada.

        -   *SubPropiedad: Punto Polígono (polygonPoint) (M, 4-n):* Un punto de ubicación en un polígono.

            -   *SubPropiedad: Punto Longitud (pointLongitude) (M, 1):* Dimensión longitudinal del punto.

            -   *SubPropiedad: Punto Latitud (pointLatitude) (M, 1):* Dimensión latitudinal del punto.

    -   *SubPropiedad: Punto dentro de un Polígono (inPolygonPoint ) (M, 4-n):* Para cualquier área delimitada que sea más grande que la mitad de la tierra, defina un punto (aleatorio) en el interior.

        -   *SubPropiedad: Punto Longitud (pointLongitude) (M, 1)*: Dimensión longitudinal del punto.

        -   *SubPropiedad: Punto Latitud (pointLatitude) (M, 1):* Dimensión latitudinal del punto.

*3.18.7. Forma de Descripción Normalizada (RDA / RCAA2 / ISBD)*

-   Cuando describa coordenadas geográficas, se recomienda utilizar las coordenadas codificadas según el modelo WGS 84 (Sistema geodésico mundial). Este modelo usa solo números decimales para las coordenadas. Las longitudes son -180 a 180 (0 es Greenwich, los números negativos son al oeste, los números positivos son al este), las latitudes son -90 a 90 (0 es el ecuador, los números negativos son al sur, los números positivos al norte).

-   Un cuadro (box/geoLocationBox) está definido por dos puntos geográficos. Esquina inferior izquierda (normalmente sur oeste), esquina superior derecha (normalmente noreste). Cada punto está definido por su longitud y latitud.

*3.18.8. Equivalencias Dublin Core*

-   dc.coverage

-   dc.coverage.spatial

*3.18.9. Ejemplos (XML y DATAVERSE)*

-   *Ejemplo XML*
..
+-----------------------------------------------------------------------+
| .. image:: _static/image18_1.png                                      |
|   :scale: 35%                                                         |
|   :name: ejemplo                                                      |                                
+-----------------------------------------------------------------------+
..
-   *Ejemplo Dataverse*
..
+-----------------------------------------------------------------------+
| .. image:: _static/image18_2.png                                      |
|   :scale: 35%                                                         |
|   :name: ejemplo                                                      |                                
+-----------------------------------------------------------------------+
..
