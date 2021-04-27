# Intermitente en D4

Nuestro primer programa que vamos a hacer es un intermitente en D4

>**tip**
>¿Por qué con D4 y no con otro?
> Porque D4 tiene un led integrado en la placa, también D0

![](/assets/led.jpg)

>**danger**
>##ATENCIÓN
>Estos leds van al reves, (configuración [pop-down](https://catedu.github.io/programa-arduino-mediante-codigo/resistencias_pullup_y_pulldown.html)) luego **para encender el led, D4 tiene que estar a nivel bajo**, y al revés para apagarlo, D4 en nivel alto.

El programa es muy sencillo y lo completamos que se pueda visualizar por la salida puerto serie, por eso al iniciar ponemos el puerto serie a 9600 baudios.

![](/assets/led2.png)

Le damos a **subir** (teniendo el programa Arduinoblocks conector minimizado, eso lo podemos ver enseguida pues detecta en que COM está conectado, en la figura sale COM5) y en **Cónsola** podemos ver el contenido del puerto serie.

![](/assets/arduinobloks6.jpg)
