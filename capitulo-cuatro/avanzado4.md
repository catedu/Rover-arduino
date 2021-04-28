# Cuarto paso: Ejecutar

## Ejecutar el servidor Blynk local
En la Raspberry por comandos, entramos en el fichero donde hemos creado el servidor Blynk

**cd Blynk**

Y ejecutamos el servidor Blynk instalado, pero que cargue la configuración de server.properties:

**java -jar server-0.41.13-java8.jar -dataFolder /home/pi/Blynk -serverConfig /home/pi/Blynk/server.properties**

## Panel de control del servidor blynk

Desde cualquier ordenador conectado en red, ejecutas en un navegador la siguiente dirección:

Si la IP de la Raspberry es 192.168.1.112 entonces entramos en:

https://192.168.1.112:9443/admin

Y podemos ver los usuarios creados

Inncluso podemos ver los **tokens** de los proyectos si falla el envío del email

##¿Y en la APP?
