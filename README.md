
## Proyecto individual 3 de Julieta Ciare. 

# Introducción.

En este proyecto vamos a elaborar un informe de los datos junto con un dashboard. A continuación le mostraremos el informe.

# Informe.

Al visualizar nuestro datasets que nos proporcionó la OACI notamos que el nombre de las columnas no son muy entendible en respuesta a ello le renombramos y creamos un diccionario.

Diccionario:

* IdAccident: Identificador de los accidentes.
* date : Fecha del accidente
* hour : hora del accidente
* Accident_location: Ubicación del accidente
* operato: Operador de la aeronave
* flight_no : Número de vuelo asignado por el operador de aeronaves
* route: Ruta completa 
* ac_type: Tipo de aeronave
* registration: Registro OACI de la aeronave
* cn_ln: número de la serie 
* all_aboard: Todos a bordo
* Passengers_on_board:Pasajeros a bordo
* crew_aboard	: Tripulación a bordo
* Number_of_deaths: Cantidad de muertos 	
* passenger_fatalities	: Muertes de pasajeros
* crew_fatalities:	Muertes de la tripulación
* ground	: Total de muertos en tierra
* summary: Breve descripción del accidente 

Cambiamos los tipo de datos de la columna Date y hour(le sacamos primero los valores desconocidos) a datatime. Los valores faltantes de las columnas categorías le asignamos "Sin datos" y a las numéricas 0. Volvemos a cambiar el tipo de datos de las columnas restantes a su correspondiente tipo.

Verificamos si hay duplicado y no hay duplicados en el datasets. Visualizamos los Outlier y no damos cuenta que en las columnas de pasajeros a bordos e muertos hay datos que son más grandes de la que debería.

Luego hacemos la conexión a la base de datos y le insertamos el datasets al la tabla creada automáticamente.

Le agregamos el datasets adicional extraída de una página web (https://www144.statcan.gc.ca/nats-stna/documents/tech/td-dt-3-1-esp.htm). Hacemos una transformación a nuestro requerimiento y le insertamos en otra tabla de la misma base de datos que el anterior datasets

Finalmente conectamos Mysql con Power Bi y empezamos a hacer el dashboard. Les dejo el link dashboard(https://app.powerbi.com/links/wHrWLxe-Qg?ctid=fbb23a34-e937-4592-bda7-c8d142c8fe96&pbi_source=linkShare) y les dejo las paginas del dashboard en pdf.