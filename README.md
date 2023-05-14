![Imagen1](img/Imagen1.jpg)

# AE-2 XML, DTD y XSD

Este es el documento formal requerido para la entrega de la actividad 1 de la asignatura "Lenguajes de Marcas" del primer curso del ciclo de Formación Profesional DAW en la escuela EDIX 2023.
# GRUPO 16
Este trabajo corresponde al Grupo 22, que está formado por:

 - Julián Méndez Podadera

El profesor  es Félix de Pablo.
# URL DEL REPOSITORIO
https://github.com/JulianMendezEdix/ad2_lenguajesDeMarcas

# ENUNCIADO

Vamos a elaborar una estructura de base de datos en XML que permita almacenar los datos de una biblioteca en la red con las siguientes características:

Existen tres tipos de documentos almacenados en la biblioteca: libros, revistas y periódicos. Todos los documentos están identificados por el atributo Id.

Para los libros este atributo empieza con la letra “L” seguido de 4 dígitos identificativos.

Para los periódicos este atributo empieza por la letra “P” seguido de los 4 dígitos identificativos.

En el caso de las revistas empieza por la letra “R”.

Los libros a su vez son clasificados en novela, infantil o didáctico. Cada libro contiene un atributo identificativo de su clase denominado tipo_clase. Dentro de cada libro se tiene un título, varios capítulos con el título en su interior, un índice y una sinopsis. Tanto en libro como en capítulo existe un atributo que contiene el número de páginas del libro o del capítulo, según corresponda. Cada capítulo contiene un elemento denominado contenido, en el que se tiene un atributo con el enlace a la información. <br/>

Las revistas a su vez son clasificadas en: informática, corazón, coches, investigación y otras. Cada revista tiene el atributo tipo_clase identificativo de la clase a la que pertenece. Dentro de cada revista tenemos el título, el número de la revista, un índice de contenido y las secciones. En cada sección y en la revista se tiene un atributo que contiene el número de páginas. Además, en cada sección se tiene la parte denominada contenido, en la que se tiene un atributo con un enlace a la información.

Los periódicos se clasifican en nacionales e internacionales. Cada periódico contiene el atributo tipo_clase identificativo de la clase a la que pertenece y un atributo que incluye la fecha de publicación. Dentro de los periódicos tenemos secciones y un índice. Cada sección debe contener un atributo identificativo del tipo de sección, que puede ser: económica, opinión, deportes, nacional o internacional. Las secciones se dividen en artículos, en donde se define en un atributo el autor. Finalmente, el contenido será el último elemento del árbol, que necesita un atributo que referencie a la información.

La información deberá de ir como nodo elemento a no ser que se especifique lo contrario (como por ejemplo el id que se pide como nodo atributo).

# REQUERIMIENTO 1

## Crear un XML con el modelo de datos indicado en el enunciado.

Captura del archivo 06_DTD_Biblioteca.xml

﻿![req1_1](img\req1_1.png)

## Elaborar un DTD que permita validar el documento XML.

Captura del archivo 06_DTD_Biblioteca.dtd

![Presentación1_page-0001](img\req1_2.png)

![Presentación1_page-0001](img\req1_22.png)

## Validar el documento con alguna aplicación externa e incluir capturas de pantalla.

El código es validado directamente con el DTD en VSCODE con la extensión XML language Support de Red Hat. Como vemos en la siguiente imagen, si ponemos una clase "ovela" en vez de novela nos da error de validación porque el archivo DTD nos pide que el tipo ha de ser novela, no novela.

![Presentación1_page-0001](img\req1_31.png)

También comprobamos que es un documento "bien Formado" en el enlace proporcionado en el enunciado (https://www.w3schools.com/xml/xml_validator.asp)

![Presentación1_page-0001](img\req1_3.png)

# REQUERIMIENTO 2

## Elaborar un XSD que permita validar el documento XML.

Captura del archivo 06_XSD_Biblioteca.xsd que marca la estructura de 06_XSD_Biblioteca.xml

![Presentación1_page-0001](img\req2xsd_31.png)

## Validar el documento con alguna aplicación externa e incluir capturas de pantalla.

el xml language support de red hat tambien valida el xsd.

Chequeamos que nuestro xsd.xml está bien formado y pongo la captura:

![Presentación1_page-0001](img\req2xsdvalid_31.png)

## Conclusiones grupales

Es aburrido trabajar sólo, aunque la tranquilidad es impagable :)

# FIN
