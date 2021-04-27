# Primer programa con Blynk: Encender D0 : ARDUINOBLOCKS

Ahora le tenemos que decir a nuestro NodeMCU la configuración de la Wifi, y el Token uqe hemos recibido, ¿cómo? muy fácil, con ARDUINOBLOCKS

Abrimos un proyecto y ponemos estra instrucción :

![](/assets/blynk13.jpg)

Donde :

* **WIFI SSID** el nombre de la Wifi donde queremos que se conecte nuestro rover
* **WIFI CLAVE** la contraseña de la WIFI
* **IP Servidor** de momento ponemos 0.0.0.0 puerto 8080 pues vamos a utilizar el servidor Blynk oficial que hay en Internet, luego veremos en 4 AVANZADO que podemos cambiar este número por un servidor local.
* Codigo Auth es el código de autentificación para que haga caso a nuestro proyecto BLYNK que acabamos de hacer, es decir [el Token que hemos recibido](https://catedu.github.io/Rover-arduino/capitulo-tres/encenderled.html).

## ¿Nada más?

Nada más !! así de sencillo. Le damos a **subir** (teniendo el programa Arduinoblocks conector minimizado, eso lo podemos ver enseguida pues detecta en que COM está conectado, en la figura sale COM5)

![](/assets/arduinobloks6.jpg)

Vamos a la APP de BLYNK, Pulsamos al botón de play ▶ de arriba arriba. Luego al botón:

![](/assets/blynk10.png)

 Y podemos ver cómo se enciende y apaga el led D0

![](/assets/led.jpg)

## Recuerda : Un proyecto en BLYNK = Un Token
