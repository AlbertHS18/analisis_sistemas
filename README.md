# Proyecto final de analisis de sistemas

## Presentación

+ Materia: Análisis de Sistemas
+ Maestro: Lizandro Ramirez
+ Periodo: P1-2023
  
<br>

## Autores:

+ Albert Francisco Hernández Sánchez 2019-0126
+ Angel Omar Mieses Florentino 2020-0711
  
<br>

# Introducción.
En el presente documento se expondra la  documentación de un programa de aplicación web que ha sido diseñado para almacenar información de usuarios en una base de datos Postgres y Redis, realizar cálculos complejos en un worker y presentar los resultados en una página web mediante el uso de un cliente React. La aplicación ha sido encapsulada en Docker con seis servicios que incluyen: nginx, postgres, api, redis, client-react y worker. La documentación abarcará una introducción a la aplicación y su funcionamiento, un marco teórico que explicará los componentes y tecnologías utilizadas, una prueba de funcionamiento detallada y una conclusión que destacará los resultados y posibles mejoras para el futuro.

<br>

# Marco Teórico.
En este apartado de la documentación estarán las diferentes definiciones de las herramientas o servicios utilizados para que este programa pueda funcionar y que son esenciales para el mismo. Con este marco teórico se tiene como objetivo dejar de forma más precisa los términos usados en este proyecto para el análisis de la app.
  
<br>

## React.
React es una biblioteca o librería de código abierto que está escrita en JavaScript. Fue desarrollada por Facebook en el 2013 con la finalidad de facilitar la creación de componentes reutilizables e interactivos para las interfaces de usuario.
Uno de sus puntos más destacados es que no solo se usa en el lado del cliente, sino que también se puede representar en el servidor y trabajar juntos.
Para comprender cómo funciona React es clave que nos situemos en un contexto, pues cuando se aprende desarrollo web se obtiene conocimiento de tres conceptos básicos:

+ HTML: la semántica, estructura e información de la página web; es decir, su esqueleto.
+ CSS: la apariencia de nuestra página web.
+ JavaScript: básicamente es el cerebro de nuestra página. Determina qué hacer en función de lo que sucede en ella.
  
<br>

## Node.js.
Node.js, Node.js, es un entorno en tiempo de ejecución multiplataforma para la capa del servidor (en el lado del servidor) basado en JavaScript.
Node.js es un entorno controlado por eventos diseñado para crear aplicaciones escalables, permitiéndote establecer y gestionar múltiples conexiones al mismo tiempo. Gracias a esta característica, no tienes que preocuparte con el bloqueo de procesos, pues no hay bloqueos.
El diseño de Node.js está inspirado en sistemas como el Event Machine de Ruby o el Twisted de Python. Sin embargo, Node.js presenta un bucle de eventos como una construcción en tiempo de ejecución en lugar de una biblioteca. Este bucle de eventos es invisible para el usuario.
  
<br>

## API REST.
Las API REST proporcionan una forma flexible y ligera de integrar aplicaciones y se han convertido en el método más común para conectar componentes en arquitecturas de microservicios.

Una API o interfaz de programación de aplicaciones es un conjunto de reglas que definen la forma en que las aplicaciones o los dispositivos pueden conectarse y comunicarse entre sí. Una API REST es una API que se ajusta a los principios de diseño de REST, o el estilo de arquitectura de transferencia de estado representacional. Por esta razón, las API REST a veces se denominan API RESTful.
  
<br>

## Docker.
Docker es un proyecto de código abierto que automatiza el despliegue de aplicaciones dentro de contenedores de software, proporcionando una capa adicional de abstracción y automatización de virtualización de aplicaciones en múltiples sistemas operativos. Docker utiliza características de aislamiento de recursos del kernel Linux, tales como cgroups y espacios de nombres (namespaces) para permitir que "contenedores" independientes se ejecuten dentro de una sola instancia de Linux, evitando la sobrecarga de iniciar y mantener máquinas virtuales. Docker implementa una API de alto nivel para proporcionar contenedores livianos que ejecutan procesos de manera aislada.
  
<br>

## Nginx.
Nginx  es un servidor web/proxy inverso ligero de alto rendimiento y un proxy para protocolos de correo electrónico.  Es software libre y de código abierto, licenciado bajo la Licencia BSD simplificada; también existe una versión comercial distribuida bajo el nombre de Nginx Plus. 
  
<br>

## Worker.
Actúan esencialmente como proxy servers asentados entre las aplicaciones web, el navegador y la red (cuando está accesible). Están destinados, entre otras cosas, a permitir la creación de experiencias offline efectivas, interceptando peticiones de red y realizando la acción apropiada si la conexión de red está disponible y hay disponibles contenidos actualizados en el servidor. También permitirán el acceso a notificaciones tipo push y APIs de sincronización en segundo plano.
Un service worker es un worker manejado por eventos registrado para una fuente y una ruta. Consiste en un fichero JavaScript que controla la página web (o el sitio) con el que está asociado, interceptando y modificando la navegación y las peticiones de recursos, y cacheando los recursos de manera muy granular para ofrecer un control completo sobre cómo la aplicación debe comportarse en ciertas situaciones (la más obvia es cuando la red no está disponible).
  
<br>

## Postgres.
PostgreSQL, también llamado Postgres, es un sistema de gestión de bases de datos relacional orientado a objetos y de código abierto, publicado bajo la licencia PostgreSQL, similar a la BSD o la MIT.
Mediante un sistema denominado MVCC (Acceso concurrente multiversión, por sus siglas en inglés) PostgreSQL permite que mientras un proceso escribe en una tabla, otros accedan a la misma tabla sin necesidad de bloqueos. Cada usuario obtiene una visión consistente.
  
<br>

## Redis.
Redis es un motor de base de datos en memoria, basado en el almacenamiento en tablas de hashes pero que opcionalmente puede ser usada como una base de datos durable o persistente. Está escrito en ANSI C por Salvatore Sanfilippo, quien es patrocinado por Redis Labs.
  
<br>

## Video (Prueba de funcionamiento)

[Haga Clic aquí](https://miucateciedu-my.sharepoint.com/:v:/g/personal/20190126_miucateci_edu_do/EUcgvG1gN_xIvKpfi4IhppMB7XQqbU1zodnu2d5VCYKMWg?e=vFFXfe) 
  
<br>

## Puntos de mejora. 

+ Diseño más amigable y fácil de entender. 
+ Añadir controles para evitar errores.
+ Mejorar distribución de informaciones a mostrar.
+ Mostar mensajes indicadores para el usuario.

<br>

# Conclusión. 
Para concluir, al realizar un análisis a fondo a este programa nos podemos dar cuenta que es muy importante e interesante el saber cómo este está estructurado y todas las herramientas o servicios se relacionan entre sí. Las partes de esta estructura que son de mucha importancia son server, nginx y worker porque son los servicios que dan los controles a la app aparte del diseño que es algo superficial pero el JS que hace los cálculos complejos de Fibonacci son lo más destacable a tener en cuenta para la realización de alguna aplicación como esta.
