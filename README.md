# Pro_Contacto
Ejercicios resueltos 

# EJERCICIO 2
Las siguientes preguntas están orientadas a la comprensión del protocolo HTTP. Son agnósticas al lenguaje de programación, la idea es comprender los conceptos del estándar:

¿Qué es un servidor HTTP? 

Un servidor HTTP es un software que responde a las peticiones hechas por los usuarios devolviendo paginas.

¿Qué son los verbos HTTP? Mencionar los más conocidos

-GET: El método GET  solicita una representación de un recurso específico. Las peticiones que usan el método GET sólo deben recuperar datos.

-HEAD: El método HEAD pide una respuesta idéntica a la de una petición GET, pero sin el cuerpo de la respuesta.

-POST: El método POST se utiliza para enviar una entidad a un recurso en específico, causando a menudo un cambio en el estado o efectos secundarios en el servidor.
-PUT: El modo PUT reemplaza todas las representaciones actuales del recurso de destino con la carga útil de la petición.
-DELETE: El método DELETE borra un recurso en específico
-CONNECT: El método CONNECT establece un túnel hacia el servidor identificado por el recurso.
-OPTIONS: El método OPTIONS es utilizado para describir las opciones de comunicación para el recurso de destino.
-TRACE: El método TRACE  realiza una prueba de bucle de retorno de mensaje a lo largo de la ruta al recurso de destino.
-PATCH: El método PATCH  es utilizado para aplicar modificaciones parciales a un recurso.

¿Qué es un request y un response en una comunicación HTTP? ¿Qué son los headers? 
Un REQUEST es un comando que permite enviar todo tipo de peticion HTTP a un URL especifico y procesar la respuesta del servidor HTTP, y el RESPONSE es la respuesta que manda el servidor HTTP al cliente tras recibir un REQUEST y los headers son toda la informacion que se transmite del usuaria y del sevidor HTTP 

¿Qué es un queryString? (En el contexto de una url)
Se utiliza para hacer referencia a una interaccion con una base de datos. Es la parte de una URL donde contiene los datos que deben de pasar a aplicaciones WEB.

¿Qué es el responseCode? ¿Qué significado tiene los posibles valores devueltos?
El responseCode indica si se completo satisfactoriamente una solicitud HTTP especifica y se dividen en 5 grupos:
1-Respuestas informativas (100–199),
2-Respuestas satisfactorias (200–299),
3-Redirecciones (300–399),
4-Errores de los clientes (400–499),
5-Errores de los servidores (500–599).

¿Cómo se envía la data en un Get y cómo en un POST? 
El método GET envía la información codificada del usuario en el header del HTTP request, directamente en la URL. La página web y la información codificada se separan por un interrogante ?
Con el método HTTP POST también se codifica la información, pero ésta se envía a través del body del HTTP Request, por lo que no aparece en la URL.

¿Qué verbo http utiliza el navegador cuando accedemos a una página?
GET

Explicar brevemente qué son las estructuras de datos JSON y XML dando ejemplo de estructuras posibles.
JSON:es un formato basado en texto estándar para representar datos estructurados en la sintaxis de objetos de JavaScript

XML: En un archivo de lenguaje marcado extensible (XML), el cual consiste en un archivo de texto sin formato que utiliza una serie de etiquetas personalizadas con la finalidad de describir tanto la estructura como otras características del documento.


Explicar brevemente el estándar SOAP
SOAP: Simple Object Access Protocol es un protocolo estándar que define cómo dos objetos en diferentes procesos pueden comunicarse por medio de intercambio de datos XML.

Explicar brevemente el estándar REST Full
Es un estilo de arquitectura software para sistemas hipermedia distribuidos como la World Wide Web.

¿Qué son los headers en un request? ¿Para qué se utiliza el key Content-type en un header?
En un request los headers son utilizados al lanzar una petición de validación, para permitir al servidor saber qué cabeceras HTTP se utilizarán cuando la petición en cuestión se lance. 
y el key conten type es la propiedad de la cabecera usada para indicar el contenido del recurso.
