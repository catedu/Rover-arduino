# Cuarto paso: Panel de control del servidor BLYNK instalado localmente

Desde cualquier ordenador conectado en red, ejecutas en un navegador la siguiente dirección:

Si la IP de la Raspberry es 192.168.1.112 entonces entramos en:

https://192.168.1.112:9443/admin

Con el usuario y contraseña fijada en server.properties :

```python
 # Default admin name and password. Will be created on initial server start
admin.email=admin@blynk.cc
admin.pass=admin
```
*Nota: Lo he intentado cambiar y no me ha funcionado 🤷‍♂️*

Luego entramos

![](/assets/avanzado7.jpg)

Y podemos ver los usuarios creados (los usuarios se crean desde la APP, luego lo vemos)

![](/assets/avanzado8.jpg)

Inncluso podemos ver los **tokens**, entrando en un usario, vemos los proyectos y podemos ver el tokens

![](/assets/avanzado9.jpg)

Útil si falla el envío del email de los tokens
