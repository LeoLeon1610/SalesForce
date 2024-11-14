<h1>Evaluación práctica para el rol de administrador</h1> 

------------


Me presento, mi nombre es Leonardo León, candidato a la vacante del rol de administrador dentro de la empresa Procontacto.

------------
<h2 style="color: #3A67FF;">Ejercicio 1: Instalación del ambiente</h2>

Adjunto la evidencia de la intalación de las programas requeridos, mediante una captura de pantalla del barra de tareas de mi ordenador.
<center>
    <img src="https://github.com/LeoLeon1610/SalesForce/blob/main/Ejercicio%201.png?raw=true" alt="Ejercicio 1">
</center>

------------

<h2 style="color: #3A67FF;">Ejercicio 2: Comprensión del protocolo HTTP</h2>

**1.	¿Qué es un servidor HTTP?**

Un servidor HTTP es un software que recibe y responde solicitudes que le llegan a través del protocolo HTTP. Cuando entras a una página web, el navegador se comunica con un servidor HTTP para pedirle que te envíe el contenido de la página.

**2.	¿Qué son los verbos HTTP? Mencionar los más conocidos**

Son acciones que el navegador o alguna app le pide al servidor. Los más conocidos son:
- GET: para obtener datos.
- POST: para enviar datos.
- PUT: para actualizar datos.
- DELETE: para borrar datos.

**3.	¿Qué es un request y un response en una comunicación HTTP? ¿Qué son los headers?**

**Request**: es la solicitud que tu navegador (o app) le manda al servidor para pedir algo, como una página web.

**Response**: es la respuesta que el servidor te envía, por ejemplo, el contenido de la página o un mensaje de error.

**Headers**: son datos extra que se envían junto con el request o el response, como el tipo de contenido que esperas recibir o el lenguaje,  (JSON, HTML, XML, etc.).

**4.	¿Qué es un queryString? (En el contexto de una url)**

Es la parte de la URL que empieza después de un signo de interrogación ?. Se usa para enviar parámetros adicionales al servidor. Por ejemplo: ?user=leonardo&age=23, donde "user" y "age" son los parámetros.


**5.	¿Qué es el responseCode? ¿Qué significado tiene los posibles valores devueltos?**

Es un código numérico que el servidor envía en la respuesta para decir cómo fue la operación:
- 1xx Informativo
- 2xx Éxito
- 3xx Redirección
- 4xx Errores del cliente(uno muy común 404; la página no se encontró)
- 5xx Error del servidor


**6.	¿Cómo se envía la data en un Get y cómo en un POST?**

La data se envía de la siguiente manera según el verbo utilizado:
- En GET, la data va en la URL como parámetros (query string).
- En POST, la data va en el cuerpo del request, no en la URL, lo que permite enviar más información o datos sensibles.

**7.	¿Qué verbo http utiliza el navegador cuando accedemos a una página?**

Generalmente usa GET para pedir el contenido de la página.

**8.	Explicar brevemente qué son las estructuras de datos JSON y XML dando ejemplo de estructuras posibles.**

JSON (JavaScript Object Notation): es un formato de texto que usa llaves {} y comillas dobles para organizar los datos. Ejemplo:

```json
{
  "nombre": "Leonardo",
  "edad": 25
}
```
XML (Extensible Markup Language): usa etiquetas similares a HTML para estructurar datos. Ejemplo:

```xml
<persona>
  <nombre>Leonardo</nombre>
  <edad>23</edad>
</persona>
```
**9.	Explicar brevemente el estándar SOAP**

SOAP es un protocolo de comunicación que usa XML para enviar mensajes entre servidores y clientes. Es más estricto y formal que REST.

**10.	Explicar brevemente el estándar REST Full**

REST es un estilo de arquitectura que permite comunicarte con servidores usando URLs y verbos HTTP (GET, POST, etc.). Es más ligero que SOAP y se utiliza mucho en aplicaciones web.

*Diferencias clave:*

SOAP es un protocolo formal con mensajes estrictamente estructurados en XML, diseñado para aplicaciones empresariales complejas.
REST es una arquitectura que usa HTTP y otros estándares de la web para crear servicios simples, ligeros y eficientes, comúnmente utilizados para APIs en aplicaciones web y móviles.


**11.	¿Qué son los headers en un request? ¿Para qué se utiliza el key Content-type en un header?**

Los headers son como "notas" que envías junto con el request para dar más detalles, como el tipo de datos que estás enviando o recibiendo.
El *Content-Type* le dice al servidor qué tipo de datos estás enviando, por ejemplo, *application/json* si mandas datos en formato JSON.

------------

<h2 style="color: #3A67FF;">Ejercicio 3: GET y POST</h2>

[**Paso 1**](https://github.com/LeoLeon1610/SalesForce/blob/main/Ejercicio%203.1.png?raw=true "**Paso 1**")

[**Paso 2**](https://github.com/LeoLeon1610/SalesForce/blob/main/Ejercicio%203.2.png?raw=true "**Paso 2**")

[**Paso 3**](https://github.com/LeoLeon1610/SalesForce/blob/main/Ejercicio%203.3.png?raw=true "**Paso 3**")


**¿Qué diferencias se observan entre las llamadas el punto 1 y 3?**

Antes del POST (punto 1): El GET muestra únicamente los datos que ya estaban presentes en la base de datos.
Después del POST (punto 3): El GET refleja el nuevo contacto que he agregado (mis datos agregados).

------------
<h2 style="color: #3A67FF;">Ejercicio 4: Trailhead</h2>

[Perfil de Trailhead](https://www.salesforce.com/trailblazer/ksjse7uaw79mvhnkto "Perfil de Trailhead")

------------
<h2 style="color: #3A67FF;">Ejercicio 5: Objectos Salesforce</h2> 

**1. Lead:**
Un Lead representa una persona o una empresa que ha mostrado interés en los productos o servicios de una organización, pero aún no ha sido calificada o convertida en una oportunidad de ventas.

*Datos que almacena:*
- Nombre del lead.
- Empresa.
- Información de contacto (email, teléfono).
- Fuente del lead (cómo llegó el prospecto).
- Estado del lead (nuevo, trabajando, cerrado).

**2.	Account:**
Una Account es una organización o empresa con la que se tiene una relación comercial. Representa clientes, socios o incluso competidores.

*Datos que almacena:*
- Nombre de la cuenta (empresa).
- Tipo de cuenta (cliente, competidor, socio).
- Información de la empresa (dirección, industria, tamaño).

**3.	Contact:**
Un Contact es una persona asociada a una Account con la que se tiene una relación comercial.

*Datos que almacena:*
- Nombre del contacto.
- Dirección de correo electrónico, teléfono.
- Cargo en la empresa.
- Relación con la cuenta


**4.	Opportunity:**
Una Opportunity es una oportunidad de venta. Representa el potencial de generar ingresos con una Account.
*Datos que almacena:*
- Nombre de la oportunidad.
- Monto proyectado.
- Fecha de cierre esperada.
- Etapa de la oportunidad.


**5.	Product**
Un Product es un bien o servicio que la empresa ofrece a sus clientes.

*Datos que almacena:*
- Nombre del producto.
- Descripción.
- Precio estándar.
- Código de producto.


**6.	PriceBook:**
Un PriceBook es una lista de productos y los precios asociados a esos productos. Puede haber diferentes listas de precios para diferentes clientes o tipos de ventas.

*Datos que almacena:*
- Nombre del libro de precios.
- Lista de productos con sus precios correspondientes.

**7.	Quote:**
Una Quote es una oferta formal que se envía a un cliente, detallando los productos, servicios y precios ofrecidos para una venta potencial.

*Datos que almacena:*
- Productos y servicios incluidos.
- Precios y descuentos.
- Total de la cotización.
- Fecha de expiración.

**8.	Asset:**
Un Asset representa un producto o servicio que un cliente ya ha comprado y está utilizando. Se utiliza para hacer un seguimiento de los productos instalados o entregados.

*Datos que almacena:*
- Producto asociado.
- Fecha de compra.
- Número de serie o identificación.
- Estado del activo.

**9.	Case:**
Un Case es una solicitud de soporte o una incidencia presentada por un cliente, normalmente relacionada con un problema o consulta sobre un producto o servicio.

*Datos que almacena:*
Descripción del problema.
- Estado del caso.
- Prioridad.
- Fecha de cierre.

**10.	Article:**
Un Article es una pieza de información en la base de conocimientos (Knowledge Base) que ayuda a resolver problemas o responder preguntas frecuentes. Se utiliza comúnmente en el contexto del soporte al cliente.

*Datos que almacena:*
- Título del artículo.
- Contenido.
- Categorías o temas relacionados.
- Fecha de creación.

------------
<h2 style="color: #3A67FF;">Ejercicio 6: Conceptos</h2>
<h3>Soluciones de Salesforce</h3>

**A. ¿Qué es Salesforce?**

Salesforce es una plataforma de gestión de relaciones con clientes (CRM) basada en la nube que ayuda a las empresas a gestionar ventas, servicio al cliente, marketing y más.

**B. ¿Qué es Sales Cloud?**

Sales Cloud es un producto de Salesforce diseñado para mejorar la gestión de ventas, ayudando a los equipos de ventas a gestionar clientes potenciales, oportunidades y cerrar tratos.

**C. ¿Qué es Service Cloud?**

Service Cloud es un producto de Salesforce que permite gestionar el servicio al cliente, ofreciendo herramientas para soporte, gestión de casos y comunicación omnicanal.

**D. ¿Qué es Health Cloud?**
Health Cloud es una solución de Salesforce para la industria de la salud que ayuda a mejorar la atención al paciente y la colaboración entre proveedores.

**E. ¿Qué es Marketing Cloud?**

Marketing Cloud es una solución de Salesforce para la automatización y gestión del marketing digital, facilitando la creación y personalización de campañas en múltiples canales.

<h3>Funcionalidades de Salesforce</h3>

**A. ¿Qué es un RecordType?**

Un RecordType es una funcionalidad en Salesforce que permite crear diferentes tipos de registros dentro de un mismo objeto, con distintos valores de campos, diseños de página y procesos de negocio.

**B. ¿Qué es un ReportType?**

Un ReportType es una plantilla que define la estructura y los datos disponibles para un informe, determinando qué objetos y relaciones se pueden utilizar en dicho informe.

**C. ¿Qué es un Page Layout?**

Un Page Layout es el diseño de página que organiza los campos, botones, enlaces y secciones visibles para los usuarios al ver o editar un registro en Salesforce.

**D.	¿Qué es un Compact Layout?**

Un Compact Layout es un diseño de página reducido que muestra un conjunto clave de campos en el encabezado de registros en dispositivos móviles y en las vistas rápidas de Lightning.

**E. ¿Qué es un Perfil?**

Un Perfil es un conjunto de permisos que define el acceso de los usuarios a objetos, campos, aplicaciones y funciones en Salesforce, controlando lo que cada usuario puede ver o hacer en la plataforma.

**F. ¿Qué es un Rol?**

Un Rol es una jerarquía de acceso a datos que organiza a los usuarios y controla la visibilidad de los registros en función de la estructura organizacional, sin interferir con los permisos de perfil.

**G. ¿Qué es un Validation Rule?**

Una Validation Rule es una regla que verifica que los datos ingresados en un registro cumplan ciertos criterios, asegurando la precisión y consistencia de la información antes de guardarse.

**H. ¿Qué diferencia hay entre una relación Master Detail y Lookup?**

Una relación Master-Detail es una relación fuerte en la que el registro hijo depende del padre, con herencia de permisos y eliminación en cascada. Una relación Lookup es una relación más flexible, donde el registro hijo no depende directamente del padre y no hereda permisos.

**I. ¿Qué es un Sandbox?**

Un Sandbox es un entorno de prueba en Salesforce que permite realizar desarrollos, configuraciones y pruebas sin afectar el entorno de producción.

**J. ¿Qué es un ChangeSet?**

Un ChangeSet es un paquete de cambios configurables en Salesforce que se utiliza para trasladar personalizaciones y desarrollos de un entorno a otro, como de un Sandbox a Producción.

**K. ¿Para qué sirve el import Wizard de Salesforce?**

El Import Wizard es una herramienta de Salesforce que permite importar y actualizar datos (como cuentas, contactos y oportunidades) desde archivos externos, facilitando la carga de datos en la plataforma.

**L. ¿Para qué sirve la funcionalidad Web to Lead?**

Web to Lead es una funcionalidad que permite capturar prospectos desde formularios web y enviar esos datos automáticamente a Salesforce, creando registros de Lead.

**M. ¿Para qué sirve la funcionalidad Web to Case?**

Web to Case es una funcionalidad que permite capturar solicitudes de soporte desde formularios web y crear automáticamente registros de caso en Salesforce.

**N. ¿Para qué sirve la funcionalidad Omnichannel?**

Omnichannel es una herramienta en Salesforce que distribuye automáticamente las solicitudes de clientes, como casos y chats, a los agentes disponibles según la carga de trabajo y habilidades.

**O. ¿Para qué sirve la funcionalidad Chatter?**

Chatter es una herramienta de colaboración en Salesforce que permite a los usuarios comunicarse, compartir archivos y actualizaciones en tiempo real dentro de la plataforma.

<h3>Conceptos generales</h3>

**A. ¿Qué significa SaaS?**

SaaS, o Software as a Service, es un modelo de entrega de software en el que las aplicaciones están alojadas en la nube y se accede a ellas a través de internet, sin necesidad de instalación local.

**B. ¿Salesforce es Saas?**

Sí, Salesforce es SaaS, puesto que ofrece sus aplicaciones a través de la nube y no requiere instalación en servidores locales.

**C. ¿Qué significa que una solución sea Cloud?**

Que una solución sea Cloud significa que sus recursos y datos están alojados en servidores remotos y se accede a ella a través de internet, sin infraestructura física en las instalaciones del cliente.

**D. ¿Qué significa que una solución sea On-Premise?**
Que una solución sea On-Premise significa que se instala y ejecuta en servidores locales, dentro de la infraestructura de la empresa, y es gestionada directamente por ella.

**E. ¿Qué es un pipeline de ventas?**

Un pipeline de ventas es el proceso o flujo de oportunidades de ventas de una empresa, representando las etapas por las que pasa un cliente potencial hasta convertirse en cliente.

**F. ¿Qué es un funnel de ventas?**

Un funnel de ventas es el modelo que ilustra las etapas por las que pasa un cliente en su recorrido de compra, desde la conciencia hasta la decisión de compra.

**G. ¿Qué significa Customer Experience?**

Customer Experience es la percepción global de los clientes sobre la interacción con una empresa, incluyendo sus productos, servicios y la relación en general.

**H. ¿Qué significa omnicanalidad?**
Omnicanalidad es la estrategia que permite a las empresas interactuar con los clientes de forma integrada y consistente a través de múltiples canales, como redes sociales, correo y teléfono.

**I. ¿Qué significa que un negocio sea B2B?¿Qué significa que un negocio sea B2C?**

Un negocio B2B (Business to Business) es uno que vende productos o servicios a otras empresas. Un negocio B2C (Business to Consumer) vende directamente al consumidor final.

**J.¿Qué es un KPI?**

Un KPI (Key Performance Indicator) es un indicador clave de rendimiento que mide el progreso hacia un objetivo estratégico en una empresa.

**K. ¿Qué es una API y en qué se diferencia de una Rest API?**

Una API (Application Programming Interface) es un conjunto de definiciones y protocolos que permiten la comunicación entre diferentes sistemas. Una REST API es un tipo específico de API que utiliza el protocolo HTTP y está diseñada para facilitar la comunicación con arquitecturas web.

**L. ¿Qué es un Proceso Batch?**

Un proceso Batch es una ejecución por lotes que procesa grandes cantidades de datos en conjunto y suele ejecutarse en horarios de bajo uso para optimizar el rendimiento.

**M. ¿Qué es Kanban?**

Kanban es una metodología visual de gestión de tareas que organiza el flujo de trabajo en columnas, lo que permite a los equipos ver el progreso y administrar el trabajo en curso.

**N. ¿Qué es un ERP?**

Un ERP (Enterprise Resource Planning) es un sistema de planificación de recursos empresariales que ayuda a gestionar y automatizar procesos de negocio, como inventario, contabilidad y producción.

**O. ¿Salesforce es un ERP?**

No, Salesforce no es un ERP. Salesforce es una plataforma CRM, aunque puede integrarse con sistemas ERP para brindar una solución empresarial más completa.

------------
<h1 style="color: #3A67FF;">Muchas gracias por su tiempo</h1>



