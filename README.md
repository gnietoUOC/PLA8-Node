# PLA8 (Node-RED)

Aquí están los dos flujos Node-RED de la PLA8. 

## Flujo MQTT -> InfluxDB

El primero de ellos es el que se subscribe al broker Mosquitto y guarda la información recibida a través de los mensajes MQTT como registros en InflusDB.
Tanto los nodos de Mosquitto como InfluxDB han sido configurados para usar SSL/TLS y credenciales.

![Flujo MQTT->InfluxDB](./images/MQTT%20Flow.png)

## Flujo Dashboard

El segundo de ellos es el flujo para crear un mini dashboard. En realidad este dashboard únicamente muestra dos imágenes SVG usando el componente Template. Se han añadido unas líneas de Javascript para poder actuar cuando se pulse sobre la imagen.

![Flujo Dashboard](./images/Dashboard%20Flow.png)

El aspecto de ese mini dashboard se muestra a continuación.

![Dashboard](./images/Dashboard.png)

Nota: El SVG para la bombilla lo he obtenido en https://www.svgrepo.com/vectors/bulb/14

