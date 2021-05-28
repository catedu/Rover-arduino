# Cuarto paso: Panel de control del servidor BLYNK instalado localmente

Desde cualquier ordenador conectado en red, ejecutas en un navegador la siguiente dirección:

Si la IP de la Raspberry es 192.168.1.112 entonces entramos en:

https://192.168.1.112:9443/admin

Seguramente te saldrá la siguiente advertencia por el certificado SSL, dale a **Configuración avanzada** y luego a **Acceder a (la ip de tu Raspberry) sitio no seguro**

![](/assets/avanzada20.jpg)

>**tip**
>Si quieres generar certificados SSL propios para que no salga la anterior pantalla consulta [aquí](https://www.sysadminsdecuba.com/2020/04/instalando-blynk-server-localmente/)

Tienes que entrar con el usuario y contraseña fijada en server.properties :

```python
 # Default admin name and password. Will be created on initial server start
admin.email=admin@blynk.cc
admin.pass=admin
```
Nota: Lo he intentado cambiar y no me ha funcionado 🤷‍♂️

Luego entramos

![](/assets/avanzado7.jpg)

Y podemos ver los usuarios creados (los usuarios se crean desde la APP, luego lo vemos)

![](/assets/avanzado8.jpg)

Inncluso podemos ver los **tokens** y los proyectos, entrando en un usario.

![](/assets/avanzado9.jpg)

Útil si falla el envío del email de los tokens
