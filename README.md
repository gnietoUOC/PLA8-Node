# PLA8 (Node-RED)

Aquí están los dos flujos Node-RED de la PLA8. 

## Flujo MQTT -> InfluxDB

El primero de ellos es el que se subscribe al broker Mosquitto y guarda la información recibida a través de los mensajes MQTT como registros en InflusDB.
Tanto los nodos de Mosquitto como InfluxDB han sido configurados para usar SSL/TLS y credenciales.

![Flujo MQTT->InfluxDB](./images/MQTT Flow.png)

## FLujo Dashboard

El segundo de ellos es el flujo para crear un mini dashboard. En realidad este dashboard únicamente muestra dos imágenes SVG usando el componente Template. Se han añadido unas líneas de Javascript para poder actuar cuando se pulse sobre la imagen.

![Flujo MQTT->InfluxDB](./images/DashboardT Flow.png)

El aspecto de ese mini dashboard se muestra a continuación.

![Flujo MQTT->InfluxDB](./images/Dashboard.png)


