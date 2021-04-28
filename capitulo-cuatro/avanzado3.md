# Tercer paso: Instalar Blynk

Crea una carpeta en tu directorio home, por ejemplo Blynk

**mkdir Blynk**

Y descarga Blynk :

wget "https://github.com/blynkkk/blynk-server/releases/download/v0.41.13/server-0.41.13-java8.jar"

## Configurar server.properties

Necesitamos crear un fichero de configuración para las diferentes opciones que queremos en nuestro servidor Blynk.

Entra en la carpeta creada Blynk y crea el fichero *server.properties*.

**cd Blynk**
**sudo nano server.properties**

A continuación se muestra una muestra del posible contenido de server.properties.

´´´python
#http and web sockets port
http.port=8080
#https and web sockets port,
https.port=9443
#application ssl port ESTE ES EL PUERTO QUE TIENES QUE PONER EN LA APP
app.ssl.port=8443
# para permitir administrar la página de administrador fuera, (si no lo haces tiene que ser en https://127.0.0.1:9443/admin) luego
 allowed.administrator.ips=0.0.0.0/0
# es decir si la ip de la raspberry es 192.168.1.112 luego puedo administrarlo fuera en n https://192.168.1.112:9443/admin
admin.rootPath=/admin
# Default admin name and password. Will be created on initial server start
admin.email=admin@blynk.cc
admin.pass=admin

´´´´









## Para saber más :

* [Intalación de Blynk : How to Install a Blynk Local Server on Raspberry Pi](https://circuitdigest.com/microcontroller-projects/how-to-install-a-blynk-local-server-on-raspberry-pi)
