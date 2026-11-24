# Diario de clase - UD3: Apache
## 1. ¿Qué he aprendido?

He aprendido a instalar, configurar y administrar un servidor web Apache en un entorno Ubuntu Server utilizando una máquina virtual. Durante esta práctica he conocido cómo funciona un servidor web, cómo crear una página personalizada mediante HTML y CSS y cómo configurar un Virtual Host para gestionar su contenido. Además, he aprendido a establecer un sistema de autenticación básica mediante usuario y contraseña para restringir el acceso a una página web. 

Posteriormente, he profundizado en la seguridad de los servidores web mediante la implementación del protocolo HTTPS. He aprendido cómo funcionan las conexiones seguras entre un navegador y un servidor y por qué es importante utilizar HTTPS para proteger la información transmitida mediante mecanismos de cifrado. También he conocido las diferencias entre los certificados SSL/TLS autofirmados y los emitidos por autoridades certificadoras de confianza, como Let's Encrypt.

En la parte práctica de HTTPS he generado mi propio certificado autofirmado utilizando OpenSSL, he habilitado los módulos SSL y headers de Apache y he configurado un VirtualHost para permitir conexiones seguras mediante el puerto 443. Además, he aprendido a establecer una redirección automática de HTTP a HTTPS para que las peticiones realizadas mediante una conexión no segura se redirijan al protocolo seguro.

Durante las diferentes prácticas también he utilizado comandos de terminal como systemctl, apache2ctl y curl, además de herramientas como OpenSSL, para comprobar el funcionamiento del servidor, detectar errores y verificar que las configuraciones se habían realizado correctamente. Por último, he podido realizar pruebas desde el navegador y desde otro equipo de la red, lo que me ha permitido comprender mejor cómo se accede a un servidor desde diferentes dispositivos y la importancia de proteger los recursos mediante mecanismos de autenticación y conexiones seguras.

![Apache Servidor Web](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcTlkfctqacl2_D_vlDi4-LCzr0j1TiYRj62hJKPSeB9Gg&s=10)

## 2. ¿Qué no entiendo?

Una de las partes que más dudas me ha generado ha sido la configuración de Apache, especialmente el funcionamiento de los Virtual Hosts. Al principio me resultó complicado comprender por qué, al acceder a la dirección IP del servidor, aparecía la página predeterminada de Apache en lugar de la página personalizada que había creado. Tuve que utilizar diferentes comandos para comprobar los archivos de configuración, identificar qué sitio estaba habilitado y averiguar cuál se estaba utilizando como predeterminado. Aunque finalmente conseguí solucionar el problema, todavía me gustaría comprender mejor cómo Apache selecciona el Virtual Host que debe mostrar en función de las peticiones recibidas.

También me gustaría profundizar en el funcionamiento de la autenticación básica y en las diferentes opciones que ofrece Apache para gestionar los permisos y restringir el acceso a determinados recursos.

Por otro lado, la implementación de HTTPS me ha generado algunas dudas relacionadas con los certificados SSL/TLS y cómo se establece la confianza entre el navegador y el servidor. Aunque he conseguido generar un certificado autofirmado y configurarlo correctamente en Apache, todavía me gustaría entender mejor cómo funcionan las autoridades certificadoras y cómo comprueban que un certificado pertenece realmente al dominio correspondiente.

Además, durante las pruebas con Firefox apareció una advertencia de seguridad al utilizar el certificado autofirmado. He comprendido por qué ocurre, pero me gustaría profundizar en cómo se establece la cadena de confianza y cómo se puede conseguir que los navegadores reconozcan un certificado como válido.

![Virtual Host](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcS_HNccKztVLqdfrQhsOesaDJrHbrRSP9Ymt0TuRDw9wA&s=10)

## 3. ¿Qué es lo que más me ha gustado? ¿Y es lo que menos?

En cuanto a la práctica de Apache, lo que más me ha gustado ha sido poder crear mi propia página web y comprobar cómo se mostraba a través del servidor que había configurado. También me ha parecido interesante incorporar la autenticación mediante usuario y contraseña, ya que he podido comprobar de forma práctica cómo se puede restringir el acceso a una página web y permitirlo únicamente a determinados usuarios.

Por otro lado, lo que menos me ha gustado ha sido la parte de configuración y resolución de problemas, especialmente cuando Apache no mostraba la página que había creado y tenía que investigar cuál era el origen del error. En algunos momentos resultó bastante complicado identificar qué archivo o configuración estaba provocando el problema. Sin embargo, también considero que esta parte ha sido útil, porque me ha permitido aprender a utilizar comandos de diagnóstico y a buscar soluciones por mi cuenta.

Además, me ha gustado poder ampliar el servidor que había configurado anteriormente implementando HTTPS y comprobar que podía acceder a la página web mediante una conexión segura. Me ha parecido especialmente interesante generar mi propio certificado y observar cómo cambiaba el comportamiento del navegador al utilizar HTTPS en lugar de HTTP.

Me ha gustado realizar las comprobaciones mediante curl, ya que he podido verificar que el servidor respondía con un código 200 OK al acceder mediante HTTPS y que las peticiones HTTP recibían una respuesta 301 Moved Permanently para redirigirse a HTTPS.

También me ha resultado algo complicada la configuración de los certificados y la advertencia de seguridad que apareció en Firefox. Al principio puede resultar confuso que el navegador muestre un aviso cuando aparentemente todo está configurado correctamente. Sin embargo, considero que estas dificultades me han ayudado a comprender mejor el funcionamiento de Apache y la importancia de comprobar cada configuración antes de dar por finalizada una implementación.

![Autenticación y Contraseña](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSIBCJujCzpD-OhB5mYgjbfShfID8ERUBE_CvjADXGbtQ&s=10)

## 4. ¿Qué más me gustaría saber relacionado con la unidad?

En relación con Apache, me gustaría profundizar en la configuración de servidores web y conocer otros mecanismos que permitan mejorar su seguridad. Especialmente, me interesa aprender a configurar HTTPS mediante certificados SSL/TLS emitidos por autoridades certificadoras de confianza, utilizando herramientas como Let's Encrypt y Certbot. Considero que sería interesante realizar una implementación con un dominio real y comprobar cómo se obtiene, instala y renueva automáticamente un certificado válido.

También me gustaría conocer otras posibilidades de Apache, como la configuración de diferentes sitios web dentro de un mismo servidor, la gestión de permisos más avanzados y el uso de otros métodos de autenticación.

Por último, me gustaría profundizar en las diferentes configuraciones de seguridad que ofrece Apache para proteger las conexiones HTTPS, como las cabeceras de seguridad, las versiones de TLS y las opciones de cifrado. Considero que aprender estos aspectos me ayudaría a comprender mejor cómo funcionan los servidores web en entornos reales y cómo se administran y protegen los servicios que ofrecen.

![Certificados SSL/TLS](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQH_g7-S1A6BQKlDW6qlPd9cl1vVSvu9FeczPLeBEuLLg&s=10)
