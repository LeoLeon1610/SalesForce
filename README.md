##Evaluación práctica para el rol de administrador
Me presento, mi nombre es Leonardo León, candidato a la vacante del rol de administrador dentro de la empresa Procontacto.
###Ejercicio 1: Instalación del ambiente
Adjunto la evidencia de la intalación de las programas requeridos, mediante una captura de pantalla del barra de tareas de mi ordenador.
###Ejercicio 2: Comprensión del protocolo HTTP
**1.	¿Qué es un servidor HTTP? **
Un servidor HTTP es un software que recibe y responde solicitudes que le llegan a través del protocolo HTTP. Cuando entras a una página web, el navegador se comunica con un servidor HTTP para pedirle que te envíe el contenido de la página.

**2.	¿Qué son los verbos HTTP? Mencionar los más conocidos
**
Son acciones que el navegador o alguna app le pide al servidor. Los más conocidos son:
- GET: para obtener datos.
- POST: para enviar datos.
- PUT: para actualizar datos.
- DELETE: para borrar datos.

**3.	¿Qué es un request y un response en una comunicación HTTP? ¿Qué son los headers?
**
**Request**: es la solicitud que tu navegador (o app) le manda al servidor para pedir algo, como una página web.
**Response**: es la respuesta que el servidor te envía, por ejemplo, el contenido de la página o un mensaje de error.
**Headers**: son datos extra que se envían junto con el request o el response, como el tipo de contenido que esperas recibir o el lenguaje,  (JSON, HTML, XML, etc.).

**4.	¿Qué es un queryString? (En el contexto de una url)
**
Es la parte de la URL que empieza después de un signo de interrogación ?. Se usa para enviar parámetros adicionales al servidor. Por ejemplo: ?user=leonardo&age=23, donde "user" y "age" son los parámetros.


**5.	¿Qué es el responseCode? ¿Qué significado tiene los posibles valores devueltos?
**
Es un código numérico que el servidor envía en la respuesta para decir cómo fue la operación:
- 1xx Informativo
- 2xx Éxito
- 3xx Redirección
- 4xx Errores del cliente(uno muy común 404; la página no se encontró)
- 5xx Error del servidor


**6.	¿Cómo se envía la data en un Get y cómo en un POST? 
**
La data se envía de la siguiente manera según el verbo utilizado:
- En GET, la data va en la URL como parámetros (query string).
- En POST, la data va en el cuerpo del request, no en la URL, lo que permite enviar más información o datos sensibles.

**7.	¿Qué verbo http utiliza el navegador cuando accedemos a una página?
**
Generalmente usa GET para pedir el contenido de la página.

**8.	Explicar brevemente qué son las estructuras de datos JSON y XML dando ejemplo de estructuras posibles.
**
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
**9.	Explicar brevemente el estándar SOAP
**
SOAP es un protocolo de comunicación que usa XML para enviar mensajes entre servidores y clientes. Es más estricto y formal que REST.
**10.	Explicar brevemente el estándar REST Full
**
REST es un estilo de arquitectura que permite comunicarte con servidores usando URLs y verbos HTTP (GET, POST, etc.). Es más ligero que SOAP y se utiliza mucho en aplicaciones web.

*Diferencias clave:
*
SOAP es un protocolo formal con mensajes estrictamente estructurados en XML, diseñado para aplicaciones empresariales complejas.
REST es una arquitectura que usa HTTP y otros estándares de la web para crear servicios simples, ligeros y eficientes, comúnmente utilizados para APIs en aplicaciones web y móviles.


**11.	¿Qué son los headers en un request? ¿Para qué se utiliza el key Content-type en un header?
**
Los headers son como "notas" que envías junto con el request para dar más detalles, como el tipo de datos que estás enviando o recibiendo.
El *Content-Type* le dice al servidor qué tipo de datos estás enviando, por ejemplo, *application/json* si mandas datos en formato JSON.

###Ejercicio 3: GET y POST
**Paso 1**
**Paso 2**
**Paso 3**
**¿Qué diferencias se observan entre las llamadas el punto 1 y 3?
**
Antes del POST (punto 1): El GET muestra únicamente los datos que ya estaban presentes en la base de datos.
Después del POST (punto 3): El GET refleja el nuevo contacto que he agregado (mis datos agregados).
