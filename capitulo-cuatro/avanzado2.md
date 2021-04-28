# Segundo paso: Instalar Java en la raspberry

Por el momento, para instalar Blynk, se necesita la **versión 8 de Java**

Primero actualicemos nuestro raspberry

Entramos en la ventana de comandos SSH y ejecutamos las siguientes órdenes, si en algún momento nos pide confirmación [Y/n] es porque faltan descargar paquetes o confirmación de instalación, por lo tanto aceptamos.

Con esta orden busca las actualizaciones

**sudo apt-get update**

y con esta las instalar

**sudo apt-get dist-upgrade**

Para instalar la versión 8 de java ejecutamos

**sudo apt install openjdk-8-jdk**

Por último una vez finalizado, comprobamos la versión que coje por defecto

**java –version**

Tiene que salir
Openjdk version 1.8.0 etc...

## Si no sale esa versión, sale una más actualicemos

Suele pasar que tenga ya instalado la versión 11, tenemos que obligar a que sea la 8 por defecto, para ello ejecutamos

**sudo update-alternatives --config java**

![](/assets/avanzado5.jpg)

Si seleccionamos el 2 podemos comprobar que ya nos sale la versión con la orden :

**java –version**

Pero esto no nos sirve, pues al reiniciar la Raspberry volverá a la versión 11.

Para ponerlo por defecto, edita el fichero *environment*

**sudo nano /etc/environment**

Y si en la orden **sudo update-alternatives --config java** salía que la carpeta donde está la versión 8 es *OpenJDK 8 path – /usr/lib/jvm/java-8-openjdk-armhf/jre/bin/java*  luego tenemos que poner en el fichero *environment* :

**JAVA_HOME="/usr/lib/jvm/java-8-openjdk-armhf/jre/bin/java"**

Guardar, reiniciar

**sudo reboot**

Y comprueba

**java –version**
