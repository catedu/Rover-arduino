# Tercer paso: Instalar Blynk

## A.- Descarga Blynk

Crea una carpeta en tu directorio home, por ejemplo Blynk

**mkdir Blynk**

Y descarga Blynk :

wget "https://github.com/blynkkk/blynk-server/releases/download/v0.41.13/server-0.41.13-java8.jar"

## B.-Configurar server.properties

Necesitamos crear un fichero de configuración para las diferentes opciones que queremos en nuestro servidor Blynk.

Entra en la carpeta creada Blynk y crea el fichero *server.properties*.

**cd Blynk**

**sudo nano server.properties**

A continuación se muestra un posible contenido de server.properties.

```python
initial.energy=1000000
allow.reading.widget.without.active.app=false
user.message.quota.limit=100
logs.folder=./logs
user.dashboard.max.limit=100
lcd.strings.pool.size=6
server.ssl.key=./server_embedded.key
webhooks.response.size.limit=96
hardware.mqtt.port=8440
table.rows.pool.size=100
terminal.strings.pool.size=25
admin.email=admin@blynk.cc
admin.rootPath=/admin
user.widget.max.size.limit=20
listen.address=
blocking.processor.thread.pool.limit=6
stats.print.worker.period=60000
enable.db=false
force.port.80.for.csv=false
enable.raw.db.data.store=true
restore.host=blynk-cloud.com
csv.export.data.points.max=43200
restore=false
user.profile.max.size=256
allow.store.ip=true
allowed.administrator.ips=0.0.0.0/0,::/0
net.interface=eth
webhooks.frequency.user.quota.limit=1000
http.port=8080
web.request.max.size=524288
user.devices.limit=50
async.logger.ring.buffer.size=2048
user.tags.limit=100
server.ssl.key.pass=
admin.pass=admin
hard.socket.idle.timeout=10
product.name=Blynk
data.folder=/Path
map.strings.pool.size=25
profile.save.worker.period=60000
https.port=9443
log.level=info
server.ssl.cert=./server_embedded.crt
force.port.80.for.redirect=true
notifications.queue.limit=2000
notifications.frequency.user.quota.limit=5
server.host=192.168.137.1
app.ssl.port=8443
hardware.default.port=8442
hardware.ssl.port=8441
hardware.mqtt.port=8440

```
Para la explicación de cada línea, aconsejo consultar esta [página](https://www.sysadminsdecuba.com/2020/04/instalando-blynk-server-localmente/) en el apartado *Configuración avanzada del servidor local*

## C.- Configurar mail.properties

Igualmente hay que crear este fichero para que el servidor envíe por email los tokens de los proyectos

Entra en la carpeta creada Blynk y crea el fichero *mail.properties*.

**cd Blynk**

**sudo nano mail.properties**

A continuación se muestra una muestra del posible contenido de mail.properties :
```python
mail.smtp.auth=true
mail.smtp.starttls.enable=true
mail.smtp.host=smtp.gmail.com
mail.smtp.port=587
mail.smtp.username=Your EMAIL ID
mail.smtp.password=Password
```

Utilizando **Your EMAIL ID** y **Password** los datos de una cuenta de gmail tuya. En esa cuenta tienes que permitir accesos no seguros. Aquí se muestra dónde está en la pantalla de configuración de Gmail :

![](/assets/cuentagoogle.jpg)


## D.- Ejecutar el servidor Blynk local

En la Raspberry por comandos SSH, entramos en la carpeta donde hemos creado el servidor Blynk

**cd Blynk**

Y ejecutamos el servidor Blynk instalado, pero que cargue la configuración de server.properties:

**java -jar server-0.41.13-java8.jar -dataFolder /home/pi/Blynk -serverConfig /home/pi/Blynk/server.properties**

>**tip**
>Para no repetir estos dos comandos cd Blynk y java -jar server-0.41.13-java8.jar -dataFolder /home/pi/Blynk -serverConfig /home/pi/Blynk/server.properties cada vez qye reiniciamos la Raspberry puedes generar un script para que lo ejecute automáticamente, puedes ver buenos tutoriales en Internet.
>Por ejemplo, usar el comando
> **crontab -e**
>y puner al final la siguiente línea
>**@reboot java -jar /home/pi/Blynk/server-0.41.13-java8.jar -dataFolder /home/pi/Blynk -serverConfig /home/pi/Blynk/server.properties**

## E.-Para saber más :

* [Intalación de Blynk : How to Install a Blynk Local Server on Raspberry Pi](https://circuitdigest.com/microcontroller-projects/how-to-install-a-blynk-local-server-on-raspberry-pi)
* [Configuración de server.properties.](https://diyprojects.io/blynk-how-to-install-a-private-local-server-on-raspberry-pi-3-unlimited-energy-test-wemos-dht22/#.YImMULUzY2y)
* [Configuración mail](https://github.com/blynkkk/blynk-server#requirements)
