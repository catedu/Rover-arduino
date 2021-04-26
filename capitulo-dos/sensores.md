# Sensores

La ventaja de ARDUINOBLOCKS es que tiene ya incorporado una cantidad de bloques con sus librerías y funciones integradas por lo que el alumno no tiene que pelear con códigos y situaciones especiales, simplemente arrastrar el bloque y funcionar:

![](/assets/sensor0.jpg)

## Probando el sensor LDR.

Vamos a probar este sensor que está conectado en una entrada analógica, para ello simplemente que escriba su valor en el puerto, y veremos cómo va cambiando.

El siguiente código lee el sensor cada 2 seg. y lo vemos por el puerto serie. Podemos comprobar que **cuanto más luz, la lectura es menor.**

![](/assets/sensor1.png)

## Probando el sensor DHT22.

Vamos a probar este sensor, que mide a la vez temperatura y humedad. Con el bloque correspondiente, [nos ahorramos bastante código](https://catedu.github.io/programa-arduino-mediante-codigo/control_de_temperatura_y_humedad.html).

![](/assets/sensor3.png)

## Probando el sensor Hall.

Este sensor tiene también su bloque :

![](/assets/sensor2.jpg)

Podemos construir un programa análogo al anteior y veremos que su salida es simplemente 0 o 1 depende si acercamos o no un imán.
