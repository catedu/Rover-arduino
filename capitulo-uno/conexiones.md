# Conexiones.

## Conexiones motores y batería

Este es el esquema de conexión de los motores y de la batería con el Shield :

![](/assets/conexiones.jpg)

Una alternativa a la conexión de la batería es utilizar un PowerBank y diréctamente al NodeMCU como podemos ver en la foto :

![](/assets/powerbank.jpg)

## Conexiones NodeMCU sensores con la Shield.

El sensor de efecto Hall y el sensor DHT22 lo conectaremos a las entradas digitales, nosotros hemos elegido

* DHT22 a D5
* Efecto Hall al D6

Es recomendable no usar D4 pues lo utilizaremos como Led

El sensor de luz LDR al ser analógico, lo conectaremos en la única entrada analógica que tiene esta shield

![](/assets/conexion-sensores.jpg)
