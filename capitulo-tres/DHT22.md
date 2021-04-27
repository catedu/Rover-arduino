# Ver la temperatura y la humedad

Este caso es distinto, pues el DHT22 está conectado al pin D5 digital, y mide dos variables **Temperatura** Y **Humedad**

>**info**
> ¿Cómo hacemos para medir dos variables que están conectados a un sólo PIN?

#### Solución PINES VIRTUALES:

Utilizando **pines virtuales**.

Vamos a ARDUINOBLOCKS y establecemos dos pines virtuales, uno para la temperatura y otro para la humedad, arbritariamente he puesto V2 y V3 pero puede ser cualquiera.

![](/assets/blynk17.jpg)

Y en Blynk incorporamos un Gauge que sea al PIN VIRTUAL V2.

![](/assets/blynk18.png)

Modificamos también los límites, pues por defecto sale 0 a 1023 y se vería muy bajo la temperatura. Suponemos que en marte hace una temperataura desde -10ºC a 30ºC (realmente llega a -50ºC)

![](/assets/blynk19.png)

Para la humedad hacemos lo mismo:

* Pin virtual V3
* Límites 0 a 100

Resultado :

![](/assets/blynk20.png)

Por cierto para hacer esto, he tenido que borrar el Gauge anterior ¡¡me he quedado sin energía!!.
