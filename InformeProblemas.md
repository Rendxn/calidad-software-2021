 # Informe de problemas
 
Para el reporte, seguimiento y resolución de problemas se utilizara la aplicacion Sentry.io la cual permite solucionar problemas en produccion a traves de todas las aplicaciones de una organizacion.
 
Una vez implementado Sentry captura todas las excepciones no manejadas, estos errores individuales son agrupados en problemas mas grandes los cuales permiten consultar informacion sobre el impacto, examinar el stacktrace, obtener contexto adicional sobre el estado de la aplicacion, y conectar el error con el commit (actualizacion en la aplicacion enviada al controlador de versiones) en el que mas problamente se introdujo el error.

## Centralizacion de la informacion
 
Permite conexion con repositorios en Github, Gitlab y Jira, adicionalmente es un software full stack por lo que permite encontrar errores tanto en el front como en el back de cualquier aplicacion y relacionarlos. Estos errores pueden ser asignados a grupos o integrantes para un mejor control del avance en la resolucion de los mismos.

Sentry posee un editor de codigo y un filtro de errores que permite realizar modificaciones directamente desde el software sin necesidad de abrir ningun otro tipo de editor de codigo ni ir al repositorio.

## Problemas de rendimiento

Sentry posee un centro de alertas de rendimiento que permiten comparar si hubo declives en el rendimiento en los entornos de produccion permite analizar el trafico de extremo a extremo ademas de analizar individualmente las diferentes llamadas a API que se estan llevando a cabo durante el proceso, linea de tiempo grafica que permite apreciar los cambios, porcentajes de rendimientos vitales que se dividen en 3 factores, buen rendimiento, rendimiento bajo y rendimiento comprometido, los cuales tienen prioridad de manejo ya que pueden ocasionar tiempos de espera largos, e incluso caidas del sistema. Los informes generados contienen informacion acerca de el ID de los eventos, la ramificacion de los eventos, eventos de span, las funciones individuales ejecutadas en un evento y los tiempos de ejecucion de las mismas, ademas del sistema operativo del cliente en el cual se ejecutaron y su navegador, adicionalmente posee un codigo de colores que permite analizar de que parte del sistema provienen los tiempos de ejecucion, estos pueden varias desde bases de datos hasta solicitudes http.

## Problemas introducidos en el desarrollo

Posee una linea de tiempo que permite analizar los eventos realizados en el tiempo anterior al tiempo en el que surgio un nuevo error, esta linea de tiempo contiene informacion de cuales pudieron ser los posibles cambios que introdujeron el error, estos se presentan en una tabla que posee informacion sobre el tipo de la accion realizada (Accion del usuario, solicitud http, navegacion, etc) ademas de una corta descripcion de la misma (click, solicitud POST, solicitud GET, etc) y el tiempo en el que fueron realizados, al final de la tabla se encuentra el error junto con el mensaje de error.

Adicionalmente posee un centro de control de versiones utilizando git para centralizar la informacion del repositorio y otros errores de desarrollo en un solo lugar, con esta herramienta se reemplaza el uso de Github issues, este centro de control de versiones presenta una tabla con informacion de las versiones lanzadas en orden cronologico adicionalmente del nombre de la rama en la que fueron subidas, junto con el numero de commits hechos durante la nueva version, los autores de los mismos y los nuevos problemas introducidos, aunque estos problemas pueden referirse a advertencias sin implicaciones tecnicas.

Finalmente hay un centro de control en el que se puede asignar los errores que deben corregirse y los desarrolladores que deben encargarse de correguirlos, esto con el fin de evitar ambiguedades en la resolucion de problemas.

## Problemas en tiempo real

Un constructor de queries que permite el monitoreo de data en tiempo real haciendo uso de eventos. Estos eventos pueden ser personalizados y la informacion de estos es presentada en un grafico que toma los tiempos de los eventos y los compara con cada una de las columnas de informacion retornadas por el evento, adicionalmente los datos se presentan en una tabla que puede ser exportada a formato *.csv.

## Problemas encontrados por los usuarios

Centro de alertas que permite ver los problemas que necesitan resolverse inmediatamente, retroalimentacion de usuario que contiene los comentarios hechos por el usuario reportando informacion adicional en caso de problemas, bugs, bloqueos, que pueda ayudar a los desarrolladores a debuggear mas rapidamente los desarrollos, adicionalmente se puede pedir al usuario un medio de contacto el cual permitira no solo adquirir mas informacion acerca del problema en caso de que sea necesario o de que el problema se repita sino a su vez reafirmarle al usuario que estos problemas que esta reportando estan siendo tenidos en cuenta y se esta trabajando para solucionarlos y darle la mejor experiencia lo mas rapido posible, lo cual construye una red de confianza con los clientes, ideal para mantener su fidelidad y evitar que se transfieran a utilizar otros softwares o cancelen los servicios adquiridos.

## Estadisticas

Sentry posee un centro de estadisticas que permite analizar como se estan llevando a cabo los procesos en periodos de tiempos definidos y asi analizar si se estan tomando las acciones correctas para resolver los problemas encontrados, o si deben hacerse modificaciones, finalmente Sentry nos otorga una seccion de dashboard (tablero) que puede ser modificada por el usuario de la manera que prefiera y le permita ver la informacion mas relevante acerca de todo el proceso del desarrollo en todo momento.