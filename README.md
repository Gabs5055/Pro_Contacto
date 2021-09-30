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
![image](https://user-images.githubusercontent.com/61442828/133843849-663b2e6e-4294-4abb-8223-8d460292f6b6.png)

XML: En un archivo de lenguaje marcado extensible (XML), el cual consiste en un archivo de texto sin formato que utiliza una serie de etiquetas personalizadas con la finalidad de describir tanto la estructura como otras características del documento.
![image](https://user-images.githubusercontent.com/61442828/133843958-e775fe89-7425-45f9-8e81-1ba43a6a621b.png)


Explicar brevemente el estándar SOAP

SOAP: Simple Object Access Protocol es un protocolo estándar que define cómo dos objetos en diferentes procesos pueden comunicarse por medio de intercambio de datos XML.


Explicar brevemente el estándar REST Full

Es un estilo de arquitectura software para sistemas hipermedia distribuidos como la World Wide Web.


¿Qué son los headers en un request? ¿Para qué se utiliza el key Content-type en un header?

En un request los headers son utilizados al lanzar una petición de validación, para permitir al servidor saber qué cabeceras HTTP se utilizarán cuando la petición en cuestión se lance. 
y el key conten type es la propiedad de la cabecera usada para indicar el contenido del recurso.

# EJERCICIO 3
Recomendamos previamente entender los conceptos de la sintaxis “json” antes de arrancar con los ejercicios.
Descargar el POSTMAN (aplicación para realizar request como cliente), adjuntando un screen de resolución para cada ítem:

Realizar un request GET a la URL: https://procontacto-reclutamiento-default-rtdb.firebaseio.com/contacts.json
![image](https://user-images.githubusercontent.com/61442828/133844440-f73baf37-1a12-49ed-acec-5e149eb32d99.png)


Realizar un request POST a la URL anterior, y con body:
{
"name":"Tu nombre",
"email":tunombre.tuapellido@procontacto.com.mx
}
Tip: (Marcar la opción “raw” como body)
![image](https://user-images.githubusercontent.com/61442828/133847484-35c06c74-e24e-4c24-b410-42a1128d0684.png)


Realizar nuevamente un request GET a la URL: https://procontacto-reclutamiento-default-rtdb.firebaseio.com/contacts.json
¿Qué diferencias se observan entre las llamadas el punto 1 y 3?
![image](https://user-images.githubusercontent.com/61442828/133847979-092463df-9227-4d6d-a42c-a55ee6e03a8d.png)
Se puede ver que esta hecho el POST realizado en el ejercicio anterior.

# EJERCICIO 4
Solicitar usuario de Trailhead a ariel.tarsitano@procontacto.com.mx
Cambiar el idioma de Trailhead a inglés.
Realizar los siguientes módulos de Trailhead:
Fundamento de la plataforma Salesforce
Fundamentos de Apex y .NET
Modelado de datos
Fundamentos y base de datos de Apex
Desencadenadores de Apex
Apex Integration Services
 
Se recomienda usar el mismo Playground para todos los módulos solicitados. Excepto que se solicite crear uno nuevo en el enunciado del Módulo.
Para revisar la resolución de los módulos, compartir la URL del perfil público de Trailhead en una liga dentro del Readme.

https://trailblazer.me/id/gdeltororosas

# EJERCICIO 5
Explicar que son conceptualmente, qué datos almacenan en forma estándar y cómo se relacionan el resto (algunos no se relacionan entre sí) cada uno de los siguientes objetos de Salesforce:

Lead
Account
Contact
Opportunity
Product
PriceBook
Quote
Asset
Case
Article

Los campos enumerarlos a través de una lista de texto en el Readme y las relaciones a través de un diagrama UML simple realizado con Drawio.
Ejemplo de diagrama
Drawio: https://app.diagrams.net/

Que una cuenta tiene muchos contactos se representa de la siguiente manera:



Completar el resto de las relaciones agregando el resto de los objetos enumerados.

Exportar el diagrama de Drawio, subirlo al repositorio y agregarlo dentro del readme con la etiqueta para linkear imágenes.

Se puede usar el schema builder de salesforce para entender las relaciones.

https://trailhead.salesforce.com/content/learn/modules/data_modeling/schema_builder

![Untitled Diagram](https://user-images.githubusercontent.com/61442828/135538499-32dd5f09-ab77-432e-8c84-0ce7572a4afe.png)


# EJERCICIO 6

![image](https://user-images.githubusercontent.com/61442828/134262344-0374671b-092e-4eaf-bd12-0ae2e6f9e135.png)
![image](https://user-images.githubusercontent.com/61442828/134263034-c035b8a2-f6fb-40c7-b57d-9989cb0147c1.png)



# EJERCICIO 7
Responder las siguientes preguntas brevemente sobre:
Soluciones de Salesforce
¿Qué es Salesforce?
Es una empresa de SaaS que tiene varios enfoques como lo es atencion al cliente, marketing, inteligencia artificial, gestion de comunidades y su producto mas popular es el CRM llamado sales cloud

¿Qué es Sales Cloud?
CRM de Salesforce que gestiona las relaciones con el cliente y las colaboraciones entre equipos comerciales. Ofrece automatización y productividad para la fuerza de ventas optimizando los procesos comerciales y alineándolos con el marketing de tu empresa y servicio de atención al cliente.
Dispone de gráficos sobre rendimiento en tiempo real y análisis sobre cuentas para que puedas tomar decisiones de forma rápida e inteligente.

¿Qué es Service Cloud?
El software de servicio al cliente Service Cloud proporciona gestión de casos, acceso al cliente en todos los canales, integración a los sistemas de datos preexistentes, aplicaciones de integración preincorporadas, tickets de asistencia, base de conocimientos, enrutamiento y escalamiento, y gestión de colas.

¿Qué es Health Cloud?
Health Cloud se enfoca en las soluciones de compromiso con el paciente que permiten a los coordinadores de atención de la salud interactuar con mayor profundidad con los pacientes en cualquier dispositivo, tomar decisiones de cuidado del paciente más inteligentes y concentrarse en las relaciones individuales con los pacientes.

¿Qué es Marketing Cloud?
Es una plataforma de Salesforce que se usa para invertir en estrategias de e-mail de marketing. Se puede personalizar, planificar y optimizar el customer journey conociendolos cada vez mejor, midiendo los resultados y sacandoles provecho 

Funcionalidades de Salesforce

¿Qué es un RecordType?
Los tipos de registro le permiten ofrecer distintos procesos comerciales, valores de lista de selección y formatos de página a diferentes usuarios. Puede crear tipos de registro para diferenciar sus negociaciones de ventas regulares de sus compromisos de servicios profesionales y ofrecer diferentes valores de lista de selección para cada uno.

¿Qué es un ReportType?
Es una plantilla donde se define objetos, la relacion de los objetos, campos incluidos en los resultados, campos marcados de forma predeterminado y los nombres de los campos que se ven en pantalla 

¿Qué es un Page Layout?
Los formatos de página controlan el formato y la organización de botones, campos, S-Control, Visualforce, vínculos personalizados y listas relacionadas en páginas de registros de objetos. También ayudan a determinar los campos que son visibles, de sólo lectura y obligatorios. Utilice formatos de página para personalizar el contenido de páginas de registros para sus usuarios.

¿Qué es un Compact Layout?
Estas ayudana que el equipo sea mas productivo enseñando informacion clave para de esta manera administrar de mejor manera el trabajo 

¿Qué es un Perfil?
Los perfiles definen como acceden los usuarios a objetos y datos y que pueden hacer en la aplicacion 

¿Qué es un Rol?
Los roles controlan el nivel de visibilidad que un usuario tiene sobre los datos de su organizacion

¿Qué es un Validation Rule?
Un validation rule verifica que los datos ingresados por usuarios en registros cumplen los estándares que especifica antes de poder guardarlos.

¿Qué diferencia hay entre una relación Master Detail y Lookup?
Dentro del lookup no es necesario especificar el registro padre del hijo mientras que dentro del master detail si es necesario especificarlo

¿Qué es un Sandbox?
Entornos que estan aislados de la organizacion de produccion por lo que lo que se realice en estos no afecta 

¿Qué es un ChangeSet?
Es una manera de enviar información sobre personalizaciones desde una organización a otra


¿Para qué sirve el import Wizard de Salesforce?
Este puede ser usado para cargar una base de datos o un archivo

¿Para qué sirve la funcionalidad Web to Lead?
Permite diseñar un formulario incluyendo las preguntas más adecuadas para cada tipo de negocio con el objetivo de insertarlo en un blog o una web corporativa, automatizando así la captación de leads y la integración de los datos de los usuarios en el CRM

¿Para qué sirve la funcionalidad Web to Case?
Da la posibilidad de capturar datos mediante la pagina web llenando u formulario 

¿Para qué sirve la funcionalidad Omnichannel?
Asigna trabajo únicamente a agentes cuyo estado de presencia es Disponible para un canal de servicio específico. Con OmniCanal, los agentes ya no tienen que seleccionar y elegir asignaciones de trabajo desde una cola, lo que ahorra a todo el mundo tiempo, esfuerzo e inteligencia.

¿Para qué sirve la funcionalidad Chatter?
Es una aplicación de colaboración en tiempo real de Salesforce que permite a sus usuarios trabajar juntos, comunicarse y compartir información

Conceptos generales

¿Qué significa SaaS? 
Software as a Service es decir que las empresas ofrecen su software como solucion a problemas

¿Salesforce es Saas?
Sí

¿Qué significa que una solución sea Cloud?
Quiere decir que se puede acceder de manera remota a software, almacenamiento de archivo y procesamiento de datos esto con conexion a internet

¿Qué significa que una solución sea On-Premise?
Se refiere a que el tipo de solucion es un software que se instala dentro de la empresa 

¿Qué es un pipeline de ventas?
Mapa de actividades diarias que componen el proceso de ventas dentro del trabajo que va desde la recepcion del lead marketing hasta el cierre del negocio

¿Qué es un funnel de ventas?
Es una manera de decirle al pipeline de ventas 

¿Qué significa Customer Experience?
Es la imagen que la compañia da al cliente es un paso despues del customer service

¿Qué significa omnicanalidad?
Es cuando la empresa puede prestar los mismos servicios a traves de todos los canales donde esta disponible

¿Qué significa que un negocio sea B2B?
Son aquellas empresas que comercializan sus productos o servicios a otras empresas y quiere decir business to business 

¿Qué significa que un negocio sea B2C?
Quiere decir business to customer y lo que hace es que una empresa comercializa sus productos o servicios a clientes personales

¿Qué es un KPI?
Son metricas que miden el rendimiento o el crecimiento de una empresa 

¿Qué es una API y en qué se diferencia de una Rest API?
Una API es un conjunto de definiciones y protocolos que se utiliza para desarrollar e integrar el software de las aplicaciones y REST es un tipo de API 

¿Qué es un Proceso Batch?
El procesamiento batch o por lotes es el proceso mediante el cual una computadora completa lotes de trabajos, a menudo simultáneamente, en orden secuencial y sin parar

¿Qué es Kanban?
Es parte de las llamadas metodologias agiles donde se ponen tareas en un trablero dividido muy comunmente en las tareas por hacer, realizando y hechas, el tablero debe estar en un lugar donde todo el equipo lo vea 

¿Qué es un ERP? 
Es un conjunto de aplicaciones de software integradas, que nos permiten automatizar la mayoría de las prácticas de negocio relacionadas con los aspectos operativos o productivos de nuestra empresa, facilitando y centralizando la información de todas las áreas que la componen
